#te.fisher

Tweaks involving the Aquatic Entangler from Thermal Expansion.

!!! note
	The [fisher](/commands/te/#te-fisher) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.fisher.add : <a href="/arguments/item/">item</a> item, <a href="/arguments/integer/">integer</a> weight</pre>

Adds an item to the catch list with the specified weight.

Higher weights give a better chance to be caught. Default rates range between 4 and 120.

!!! example
	```python
	#adds emerald to the fish list, with a weight of 100
	te.fisher.add : item(minecraft:emerald), 100;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.fisher.remove : <a href="/arguments/all/">all</a> *</pre>

Remove all items.

!!! example
	```python
	#disable all fish
	te.fisher.remove : *;
	```

<br>

---
## bait.add ![](/img/version_1.12.png)

<pre>te.fisher.bait.add : <a href="/arguments/item/">item</a> item, <a href="/arguments/integer/">integer</a> multipier</pre>

Adds an item to the bait list with the specified multiplier.

!!! example
	```python
	#adds diamond to the bait list, with a multiplier of 5
	te.fisher.bait.add : item(minecraft:diamond), 5;
	```

<br>

---
## bait.remove ![](/img/version_1.12.png)

<pre>te.fisher.bait.remove : <a href="/arguments/all/">all</a> *</pre>

Remove all items.

!!! example
	```python
	#disable all bait
	te.fisher.bait.remove : *;
	```

<br>