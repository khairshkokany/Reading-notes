# RESTful web API design
## What does REST stand for?
Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.
## REST APIs are designed around a RESOURCES
## What is an identifer of a resource? Give an example.
A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:
HTTP:
Copy
https://adventure-works.com/orders/1
## What are the most common HTTP verbs?
1. GET methods: A successful GET method typically returns HTTP status code 200 (OK).
2. POST methods: The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.
3. PUT methods: Consider implementing bulk HTTP PUT operations that can batch updates to multiple resources in a collection. The PUT request should specify the URI of the collection, and the request body should specify the details of the resources to be modified. This approach can help to reduce chattiness and improve performance.
4. PATCH methods: With a PATCH request, the client sends a set of updates to an existing resource, in the form of a patch document. The server processes the patch document to perform the update
5. DELETE methods: If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled, but that the response body contains no further information.
## What should the URIs be based on?
is a unique sequence of characters that identifies a logical or physical resource used by web technologies. URIs may be used to identify anything, including real-world objects, such as people and places, concepts, or information resources such as web pages and books.
## Give an example of a good URI:
Keywords in the URL aid SEO and give users an idea of what the page is about. This is true for both static and dynamic URLs.
The consensus is that a lowercase slug, separated by dashes, is the best.
Search engines index dynamic URIs (e.g. index.php?page=about) just fine.
Using ID numbers in URLs is much easier/faster for grabbing the content from the database.
Search Engines prefer unique URLs, so it's best to avoid having parts of the URL with no bearing on what is displayed if possible.
Use rel="canonical" if you can't avoid possible duplicates. example.com/1234/my-page in theory should be different to example.com/1234/my-pgae but for most practical purposes they end up returning the same content, like on this site.
## What status code does an unsuccessful GET request return?
If the resource cannot be found, the method should return 404 (Not Found).
## What status code does a successful POST request return?
If a POST method creates a new resource, it returns HTTP status code 201 (Created). The URI of the new resource is included in the Location header of the response. The response body contains a representation of the resource.
If the method does some processing but does not create a new resource, the method can return HTTP status code 200 and include the result of the operation in the response body. Alternatively, if there is no result to return, the method can return HTTP status code 204 (No Content) with no response body.
## What status code does a successful DELETE request return?
If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled, but that the response body contains no further information.