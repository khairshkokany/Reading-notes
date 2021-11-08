# Add relationships between types

![images](https://www.vippng.com/png/detail/360-3609058_the-circles-in-the-graph-are-called-nodes.png)

- The @connection directive enables you to specify relationships between @model types.
  - one-to-one
  - one-to-many
  - many-to-one
  - many-to-many

- Relationships between types are specified by annotating fields on an @model object type with the @connection directive.

- The fields argument can be provided and indicates which fields can be queried by to get connected objects.
- The keyName argument can optionally be used to specify the name of secondary index (an index that was set up using @key) that should be queried from the other type in the relationship.

- A Has One @connection can only reference the primary index of a model (ie. it cannot specify a "keyName" as described below in the Has Many section).

```
type Project @model {
  id: ID!
  name: String
  team: Team @connection
}

type Team @model {
  id: ID!
  name: String!
}

```
- A many-to-many You can implement many to many using two 1-M @connections, an @key, and a joining @model. For example:


```
type Post @model {
  id: ID!
  title: String!
  editors: [PostEditor] @connection(keyName: "byPost", fields: ["id"])
}

# Create a join model and disable queries as you don't need them
# and can query through Post.editors and User.posts
type PostEditor
  @model(queries: null)
  @key(name: "byPost", fields: ["postID", "editorID"])
  @key(name: "byEditor", fields: ["editorID", "postID"]) {
  id: ID!
  postID: ID!
  editorID: ID!
  post: Post! @connection(fields: ["postID"])
  editor: User! @connection(fields: ["editorID"])
}

type User @model {
  id: ID!
  username: String!
  posts: [PostEditor] @connection(keyName: "byEditor", fields: ["id"])
}

```