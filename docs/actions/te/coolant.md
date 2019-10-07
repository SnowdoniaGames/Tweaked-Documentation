#te.coolant

Tweaks involving Coolants for the Thermal Mediator from Thermal Expansion.

<br>

---
## add ![](/img/version_1.12.png)

<pre>te.coolant.add : <a href="/arguments/fluid/">fluid</a> coolant, <a href="/arguments/integer/">integer</a> thermal capacity, <a href="/arguments/integer/">integer</a> factor</pre>

Adds a fluid to the coolant list with specified thermal capacity and coolant factor.

!!! example
	```python
	#adds lava to coolants, with thermal capacity of 1 million and 80% coolant factor
	te.coolant.add : fuid(lava), 1000000, 80;
	```

<br>

---
## remove ![](/img/version_1.12.png)

<pre>te.coolant.remove : <a href="/arguments/all/">all</a> *</pre>
<pre>te.coolant.remove : <a href="/arguments/fluid/">fluid</a> fluid</pre>

Remove all or selected items.

!!! example
	```python
	#disable all coolants
	te.coolant.remove : *;
	
	#disable water
	te.coolant.remove : fluid(water);
	```

<br>