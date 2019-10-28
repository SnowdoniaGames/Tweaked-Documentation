#te.insolator

Tweaks involving the Phytogenic Insolator from Thermal Expansion.

!!! note
	The [insolator](/commands/te/#te-insolator) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.insolator.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB, <a href="/arguments/integer/">integer</a> energy, <a href="/arguments/integer/">integer</a> water</pre>
<pre>te.insolator.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB, <a href="/arguments/item/">item</a> secondaryOutput, <a href="/arguments/integer/">integer</a> secondaryChance, <a href="/arguments/integer/">integer</a> energy, <a href="/arguments/integer/">integer</a> water</pre>

Adds a recipe to the Phytogenic Insolator.

!!! example
	```python
	#convert diamond, coal and 200mb of water to emerald, with a 50% chance of getting an apple
	te.insolator.add : item(minecraft:emerald), item(minecraft:diamond), item(minecraft:coal), item(minecraft:apple) 50, 2000, 200;
	```

<br>

---
## tree.add ![](/img/version_1.12.png)

<pre>te.insolator.tree.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB, <a href="/arguments/integer/">integer</a> energy, <a href="/arguments/integer/">integer</a> water</pre>
<pre>te.insolator.tree.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB, <a href="/arguments/item/">item</a> secondaryOutput, <a href="/arguments/integer/">integer</a> secondaryChance, <a href="/arguments/integer/">integer</a> energy, <a href="/arguments/integer/">integer</a> water</pre>

Adds a recipe to the Phytogenic Insolator when using the Sapling Infuser augment.

!!! example
	```python
	#convert diamond, coal and 200mb of water to emerald, with a 50% chance of getting an apple
	te.insolator.tree.add : item(minecraft:emerald), item(minecraft:diamond), item(minecraft:coal), item(minecraft:apple) 50, 2000, 200;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.insolator.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.insolator.remove : <a href="/arguments/item/">item</a> inputA, <a href="/arguments/item/">item</a> inputB</pre>

Remove all or selected items.

!!! example
	```python
	#disable all recipes
	te.insolator.remove : *;
	
	#disable the recipe for diamond and coal
	te.insolator.remove : item(minecraft:diamond), item(minecraft:coal);
	```

<br>