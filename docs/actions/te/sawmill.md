#te.sawmill

Tweaks involving the Sawmill from Thermal Expansion.

!!! note
	The [sawmill](/commands/te/#te-sawmill) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.sawmill.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy</pre>
<pre>te.sawmill.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/item/">item</a> secondaryOutput, <a href="/arguments/integer/">integer</a> secondaryChance, <a href="/arguments/integer/">integer</a> energy</pre>

Adds a recipe to the Sawmill.

!!! note
	Resin Funnel augment recipes are controlled by [te.tapper](/actions/te/tapper/#add).

!!! example
	```python
	#convert diamond to emerald, with a 50% chance of getting coal
	te.sawmill.add : item(minecraft:emerald), item(minecraft:diamond), item(minecraft:coal), 50, 2000;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.sawmill.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.sawmill.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all or selected items.

!!! example
	```python
	#disable all recipes
	te.sawmill.remove : *;
	
	#disable the recipe for diamond
	te.sawmill.remove : item(minecraft:diamond);
	```

<br>