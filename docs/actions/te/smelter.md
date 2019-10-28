#te.smelter

Tweaks involving the Induction Smelter from Thermal Expansion.

!!! note
	The [smelter](/commands/te/#te-smelter) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.smelter.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB, <a href="/arguments/integer/">integer</a> energy</pre>
<pre>te.smelter.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB, <a href="/arguments/item/">item</a> secondaryOutput, <a href="/arguments/integer/">integer</a> secondaryChance, <a href="/arguments/integer/">integer</a> energy</pre>

Adds a recipe to the Induction Smelter.

!!! example
	```python
	#convert diamond and coal to emerald, with a 50% chance of getting an apple
	te.smelter.add : item(minecraft:emerald), item(minecraft:diamond), item(minecraft:coal), item(minecraft:apple) 50, 2000;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.smelter.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.smelter.remove : <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB</pre>

Remove all or selected items.

!!! example
	```python
	#disable all recipes
	te.smelter.remove : *;
	
	#disable the recipe for diamond and coal
	te.smelter.remove : item(minecraft:diamond), item(minecraft:coal);
	```

<br>