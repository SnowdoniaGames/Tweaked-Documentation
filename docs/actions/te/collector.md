#te.collector

Tweaks involving the Insightful Condenser from Thermal Expansion.

!!! note
	The [collector](/commands/te/#te-collector) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.collector.add : <a href="/arguments/item/">item</a> item, <a href="/arguments/integer/">integer</a> xp, <a href="/arguments/integer/">integer</a> multiplier</pre>

Adds a catalyst to the Insightful Condensor with provided experience bonus and production multiplier.

The production multiplier works in the form : 1 + (multiplier / 100), so for example 150 would give a multiplier of 2.5x.

!!! example
	```python
	#adds diamond to the catalysts, with 500 xp and x4 multiplier
	te.collector.add : item(minecraft:diamond), 500, 300;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.collector.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.collector.remove : <a href="/arguments/item/">item</a> item</pre>

Remove all or selected items.

!!! example
	```python
	#disable all catalysts
	te.collector.remove : *;
	
	#disable the catalyst for diamond
	te.collector.remove : item(minecraft:diamond);
	```

<br>