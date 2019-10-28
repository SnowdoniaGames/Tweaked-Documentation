#te.crucible

Tweaks involving the Magma Crucible from Thermal Expansion.

!!! note
	The [crucible](/commands/te/#te-crucible) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.crucible.add : <a href="/arguments/fluid/">fluid</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy</pre>

Adds a recipe to the Magma Crucible.

!!! example
	```python
	#convert diamond to lava
	te.crucible.add : fluid(lava), item(minecraft:diamond), 4000;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.crucible.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.crucible.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all or selected items.

!!! example
	```python
	#disable all recipes
	te.crucible.remove : *;
	
	#disable the recipe for diamond
	te.crucible.remove : item(minecraft:diamond);
	```

<br>