# ore ![](/img/version_1.12.png)![](/img/version_1.14.png)

An ore is a special command used to represent all items/blocks referenced by an ore dictionary entry.

The ore dictionary allows groups of items to be represented by a single identifier.

An ore is a type of [ingredient](/arguments/ingredient/) and can therefore be used in any method as one.

## Argument

<pre>ore(identifier)</pre>

An ore is created by simply specifying the ore dictionary identifier.

!!! example
	```python
	#specifies all dictionary items registered under gemDiamond
	ore(gemDiamond)
	```
<br>
