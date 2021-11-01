# Create dynamic lists with RecyclerView   

![images](https://i.ytimg.com/vi/EyUjw6b5gXE/maxresdefault.jpg)
> RecyclerView makes it easy to efficiently display large sets of data. You supply the data and define how each item looks, and the RecyclerView library dynamically creates the elements when they're needed.

## Key classes
1. RecyclerView is the ViewGroup that contains the views corresponding to your data.

2. Each individual element in the list is defined by a view holder object. 

3. The RecyclerView requests those views, and binds the views to their data, by calling methods in the adapter.

4. The layout manager arranges the individual elements in your list.

## Steps for implementing your RecyclerView

Using a RecyclerView has the following key steps:
- Define a model class to use as the data source.
- Add a RecyclerView to your activity to display the items.
- Create a custom row layout XML file to visualize the item.
- Create a RecyclerView.
- Bind the adapter to the data source to populate the RecyclerView.

## Plan your layout

- LinearLayoutManager

- GridLayoutManager

- StaggeredGridLayoutManager

## Implementing your adapter and view holder


- onCreateViewHolder()

- onBindViewHolder()

- getItemCount()

