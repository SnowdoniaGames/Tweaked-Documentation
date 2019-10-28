#te.pulverizer

Tweaks involving the Pulverizer from Thermal Expansion.

!!! note
	The [pulverizer](/commands/te/#te-pulverizer) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.pulverizer.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy</pre>
<pre>te.pulverizer.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/item/">item</a> secondaryOutput, <a href="/arguments/integer/">integer</a> secondaryChance, <a href="/arguments/integer/">integer</a> energy</pre>

Adds a recipe to the Pulverizer.

!!! example
	```python
	#convert diamond to emerald, with a 50% chance of getting coal
	te.pulverizer.add : item(minecraft:emerald), item(minecraft:diamond), item(minecraft:coal), 50, 2000;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.pulverizer.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.pulverizer.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all or selected items.

!!! example
	```python
	#disable all recipes
	te.pulverizer.remove : *;
	
	#disable the recipe for diamond
	te.pulverizer.remove : item(minecraft:diamond);
	```

<br>