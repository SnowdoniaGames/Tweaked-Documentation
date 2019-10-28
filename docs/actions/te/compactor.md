#te.compactor

Tweaks involving the Compactor from Thermal Expansion.

!!! note
	The [compactor](/commands/te/#te-compactor) command can be used to view recipes.

<br>

---
## plate.add ![](/img/version_1.12.png)

<pre>te.compactor.plate.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy</pre>

Adds a plate recipe to the compactor.

!!! example
	```python
	#convert diamond into emerald
	te.compactor.plate.add : item(minecraft:emerald), item(minecraft:coal), 500;
	```

<br>

---
## gear.add ![](/img/version_1.12.png)

<pre>te.compactor.gear.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy</pre>

Adds a gear recipe to the compactor.

!!! example
	```python
	#convert diamond into emerald
	te.compactor.gear.add : item(minecraft:emerald), item(minecraft:coal), 500;
	```

<br>

---
## coin.add ![](/img/version_1.12.png)

<pre>te.compactor.coin.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/item/">item</a> input, <a href="/arguments/integer/">integer</a> energy</pre>

Adds a coin recipe to the compactor.

!!! example
	```python
	#convert diamond into emerald
	te.compactor.coin.add : item(minecraft:emerald), item(minecraft:coal), 500;
	```

<br>

---
## all.remove ![](/img/version_1.12.png)

<pre>te.compactor.all.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.compactor.all.remove : <a href="/arguments/item/">item</a> input</pre>

Removes a recipe from the compactor.

!!! note
	The 'all' list is a special list that is added to the plate list on runtime, it does not add to all categories like expected.

!!! example
	```python
	#disable all recipes
	te.compactor.all.remove : *;
	
	#disable the diamond recipe
	te.compactor.all.remove : item(minecraft:diamond);
	```

<br>

---
## plate.remove ![](/img/version_1.12.png)

<pre>te.compactor.plate.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.compactor.plate.remove : <a href="/arguments/item/">item</a> input</pre>

Removes a plate recipe from the compactor.

!!! note
	Some items (for instance blaze rods) are added to the 'all' list and not the plate list, use the all.remove command if this fails to work. 

!!! example
	```python
	#disable all recipes
	te.compactor.plate.remove : *;
	
	#disable the diamond recipe
	te.compactor.plate.remove : item(minecraft:diamond);
	```

<br>

---
## gear.remove ![](/img/version_1.12.png)

<pre>te.compactor.gear.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.compactor.gear.remove : <a href="/arguments/item/">item</a> input</pre>

Removes a gear recipe from the compactor.

!!! example
	```python
	#disable all recipes
	te.compactor.gear.remove : *;
	
	#disable the diamond recipe
	te.compactor.gear.remove : item(minecraft:diamond);
	```

<br>

---
## coin.remove ![](/img/version_1.12.png)

<pre>te.compactor.coin.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.compactor.coin.remove : <a href="/arguments/item/"></a> input</pre>

Removes a coin recipe from the compactor.

!!! example
	```python
	#disable all recipes
	te.compactor.coin.remove : *;
	
	#disable the diamond recipe
	te.compactor.coin.remove : item(minecraft:diamond);
	```

<br>