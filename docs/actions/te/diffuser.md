#te.diffuser

Tweaks involving the Decoctive Diffuser from Thermal Expansion.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.diffuser.add : <a href="/arguments/item/">item</a> item, <a href="/arguments/integer/">integer</a> amplitude, <a href="/arguments/integer/">integer</a> duration</pre>

Adds a reagent to the Decoctive Diffuser with provided amplitude and duration bonuses.

The amplitude and duration multiply the values for each count, so 1 will double it, 2 will triple it and so on.

!!! example
	```python
	#adds diamond to the reagents, doubling both amplitude and duration
	te.diffuser.add : item(minecraft:diamond), 1, 1;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.diffuser.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.diffuser.remove : <a href="/arguments/item/">item</a> item</pre>

Remove all or selected items.

!!! example
	```python
	#disable all reagents
	te.diffuser.remove : *;
	
	#disable the reagent for diamond
	te.diffuser.remove : item(minecraft:diamond);
	```

<br>