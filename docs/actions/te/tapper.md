#te.tapper

Tweaks involving the Arboreal Extractor from Thermal Expansion.

!!! note
	The [tapper](/commands/te/#te-tapper) command can be used to view recipes.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.tapper.add : <a href="/arguments/item/">item</a> log, <a href="/arguments/fluid/">fluid</a> fluid</pre>

Adds a fluid output based on the block being tapped.

!!! note
	In order for custom logs to work, make sure their leaves are also registered

!!! example
	```python
	#causes tapping oak logs to produce lava
	te.tapper.add : item(minecraft:log), fluid(lava);
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.tapper.remove : <a href="/arguments/all/">all</a> *</pre>

Remove all logs.

!!! example
	```python
	#disable all reagents
	te.tapper.remove : *;
	```

<br>

---
## leaf.add  ![](/img/experimental.png) ![](/img/version_1.12.png)

<pre>te.tapper.leaf.add : <a href="/arguments/item/">item</a> log, <a href="/arguments/item/">item</a> leaf</pre>

Registers a leaf to a provided log. The Arboreal Extractor will only work on trees with a correct leaves attached.

This means that when adding a custom tree, the correct leaves will need to be registered to its log type.

<br>

---
## fertilizer.add ![](/img/version_1.12.png)

<pre>te.tapper.fertilizer.add : <a href="/arguments/item/">item</a> item, <a href="/arguments/integer/">integer</a> multiplier</pre>

Adds a fertilizer with the specified multiplier.

!!! example
	```python
	#adds diamond to the fertilizers with x5 multiplier
	te.tapper.fertilizer.add : item(minecraft:diamond), 5;
	```

<br>

---
## fertilizer.remove ![](/img/version_1.12.png)

<pre>te.tapper.fertilizer.remove : <a href="/arguments/all/">all</a> *</pre>

Remove all fertilizers.

!!! example
	```python
	#disable all fertilizers
	te.tapper.fertilizer.remove : *;
	```

<br>
