#recipes

Tweaks involving crafting table recipes.

## remove ![](/img/version_1.12.png)

<pre>recipes.remove : <a href="/arguments/string/">string</a> name</pre>

Disable the specific recipe that matches the provided name

!!! note
	The [recipes command](/commands/recipes/) can be used to get a list of recipes for an item.

!!! example
	```python
	#remove the default crafting recipe for a torch
	recipes.remove : "minecraft:torch";
	```
<br>

<pre>recipes.remove : <a href="/arguments/item/">item</a> output</pre>

Disable all crafting recipes that match the provided output

!!! example
	```python
	#remove all crafting recipes for torches
	recipes.remove : item(minecraft:torch);
	```
<br>

---
## shaped ![](/img/version_1.12.png)

<pre>recipes.shaped : <a href="/arguments/string/">string</a> name, <a href="/arguments/item/">item</a> output, <a href="/arguments/ingredient/">ingredient</a> inputA, <a href="/arguments/ingredient/">ingredient</a> inputB, <a href="/arguments/ingredient/">ingredient</a> inputC ...</pre>

Adds a new shaped crafting recipe.

Can be supplied with up to 9 [ingredients](/arguments/ingredient/) inputs, each corresponding to a spot in the crafting table. 

Produces the crafting table recipe of :  
A  |  B  |  C  
D  |  E  |  F  
G  |  H  |  I

Trailing nulls can be omitted in order to save space.

!!! example
	```python
	#vanilla crafting table
	recipes.shaped : "crafting_table_copy", item(minecraft:crafting_table), ore(plankWood), ore(plankWood), null, ore(plankWood), ore(plankWood);

	#vanilla stone slab
	recipes.shaped : "slab_copy", item(minecraft:stone_slab).count(3), item(minecraft:stone), item(minecraft:stone), item(minecraft:stone);

	#vanilla torch
	recipes.shaped : "torch_copy", item(minecraft:torch).count(4), null, item(minecraft:coal), null, null, ore(stickWood);
	```
<br>

---
## shapeless ![](/img/version_1.12.png)

<pre>recipes.shapeless : <a href="/arguments/string/">string</a> name, <a href="/arguments/stack/">stack</a> output, <a href="/arguments/ingredient/">ingredient</a> inputA, <a href="/arguments/ingredient/">ingredient</a> inputB, <a href="/arguments/ingredient/">ingredient</a> inputC ...</pre>

Adds a new shapeless crafting recipe

Can have between 1 and 9 [ingredients](/arguments/ingredient/) inputs that can be arranged in any order.

!!! example
	```python
	#adds a shaped recipe that turns 1 stone into diamond
	recipes.shapeless : "cheat_diamond", item(minecraft:diamond), item(minecraft:stone);
	```