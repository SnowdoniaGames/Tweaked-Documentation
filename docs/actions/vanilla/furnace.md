#furnace

Tweaks involving changing of Vanilla furnace recipes and fuels.

<br>

---
## add

<pre>furnace.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input</pre>
<pre>furnace.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/float/">float</a> experience</pre>

Adds a recipe to the furnace with the option to specify the experience dropped.

!!! example
	```python
	#add recipe to turn diamonds into emeralds
	furnace.add : item(minecraft:emerald), item(minecraft:diamond), 4.0;
	```

<br>

---
## remove

<pre>furnace.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>furnace.remove : <a href="/arguments/item/">item</a> output</pre>

Remove all or a recipe specified by its output.

!!! example
	```python
	#disable all furnace recipes
	furnace.remove : *;
	
	#disable the vanilla stone recipe
	furnace.remove : item(minecraft:stone);
	```

<br>

---
## fuel.add

<pre>furnace.fuel.add : <a href="/arguments/item/">item</a> fuel, <a href="/arguments/integer/">integer</a> burnTime)</pre>

Adds a new fuel type, burning for the specified time.

!!! example
	```python
	#add diamonds as a fuel, burning 10 times longer than coal
	furnace.fuel.add : item(minecraft:diamond), 8000;
	```

<br>

---
## fuel.remove

<pre>furnace.fuel.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>furnace.fuel.remove : <a href="/arguments/item/">item</a> fuel</pre>

Removes all or a specified fuel.

!!! example
	```python
	#remove all fuels.
	furnace.fuel.remove : *;
	
	#remove coal as a fuel.
	furnace.fuel.remove : item(minecraft:coal);
	```

<br>