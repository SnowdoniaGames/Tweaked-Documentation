#te.furnace

Tweaks involving the Redstone Furnace from Thermal Expansion.

!!! note
	The [furnace](/commands/te/#te-furnace) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.furnace.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy, <a href="/arguments/boolean/">boolean</a> isFood</pre>

Adds a recipe to the Redstone Furnace.

The isFood setting determines whether the item is added to the list of foods for the Trivection Chamber augment.

!!! example
	```python
	#convert diamond to emerald
	te.furnace.add : item(emerald), item(minecraft:diamond), 4000, false;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.furnace.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.furnace.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all or selected items.

!!! example
	```python
	#disable all recipes
	te.furnace.remove : *;
	
	#disable the recipe for diamond
	te.furnace.remove : item(minecraft:diamond);
	```

<br>

---
## food.remove ![](/img/version_1.12.png)

<pre>te.furnace.food.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.furnace.food.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all or selected items from the list of foods for the Trivection Chamber augment.

!!! example
	```python
	#disable all food recipes
	te.furnace.food.remove : *;
	```

<br>

---
## pyro.add ![](/img/version_1.12.png)

<pre>te.furnace.pyro.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy, <a href="/arguments/integer/">integer</a> creosote</pre>

Adds a recipe to the Redstone Furnace when using the Pyrolytic Conversion augment.

The creosote argument determines the amount of Creosote created.

!!! example
	```python
	#convert diamond to emerald and 1 bucket of creosote
	te.furnace.pyro.add : item(emerald), item(minecraft:diamond), 4000, 1000;
	```

<br>

---
## pyro.remove ![](/img/version_1.12.png)

<pre>te.furnace.pyro.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.furnace.pyro.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all or selected items when using the Pyrolytic Conversion augment.

!!! example
	```python
	#disable all pyrolosis recipes
	te.furnace.pyro.remove : *;
	```

<br>