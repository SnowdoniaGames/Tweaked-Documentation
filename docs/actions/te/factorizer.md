#te.factorizer

Tweaks involving the Factorizer from Thermal Expansion.

!!! note
	The [factorizer](/commands/te/#te-factorizer) command can be used to view recipes.

<br>

---
## split.add ![](/img/version_1.12.png)

<pre>te.factorizer.split.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/input/">input</a> input</pre>

Add a split recipe to the factorizer.

!!! example
	```python
	#split emerald into 9 diamonds
	te.factorizer.split.add : item(minecraft:diamond).count(9), item(minecraft:emerald);
	```

<br>

---
## split.remove ![](/img/version_1.12.png)

<pre>te.factorizer.split.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.factorizer.split.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all split recipes or recipes with the specified input.

!!! example
	```python
	#disable all split recipes
	te.factorizer.split.remove : *;
	
	#disable splitting emerald
	te.factorizer.split.remove : item(minecraft:emerald);
	```

<br>

---
## combine.add ![](/img/version_1.12.png)

<pre>te.factorizer.combine.add : <a href="/arguments/item/">item</a> output, <a href="/arguments/input/">input</a> input</pre>

Add a combine recipe to the factorizer.

!!! example
	```python
	#combine 9 diamonds into and emerald
	te.factorizer.combine.add : item(minecraft:emerald), item(minecraft:diamond).count(9);
	```

<br>

---
## combine.remove ![](/img/version_1.12.png)

<pre>te.factorizer.combine.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.factorizer.combine.remove : <a href="/arguments/item/">item</a> input</pre>

Remove all combine recipes or recipes with the specified input.

!!! example
	```python
	#disable all combine recipes
	te.factorizer.combine.remove : *;
	
	#disable combining diamonds
	te.factorizer.combine.remove : item(minecraft:diamond).count(9);
	```

<br>