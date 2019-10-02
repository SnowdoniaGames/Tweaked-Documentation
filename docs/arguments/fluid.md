# fluid ![](/img/version_1.12.png)![](/img/version_1.14.png)

A fluid can be used to specify any minecraft liquid.

!!! note
	The [fluid command](/commands/fluid/) can be used to get a list of registered fluid names.

## Argument
A fluid is specified using the "fluid" keyword.

<pre>fluid(name)</pre>

!!! example
	```python
	#creates a fluid of type water
	fluid(water)
	```

<br>

## Modifiers

### Count ![](/img/version_1.12.png)![](/img/version_1.14.png)

Specifies the amount of the fluid in mb, by default this is 1000.

<pre>.count(amount)</pre>
<pre>.c(amount)</pre>

<br>

### Meta ![](/img/version_1.12.png)

Specifies the metadata value assigned to the fluid.

<pre>.meta(value)</pre>
<pre>.m(value)</pre>

<br>

### NBT ![](/img/version_1.12.png)![](/img/version_1.14.png)

Specifies any NBT information assigned to the fluid.

<pre>.nbt(value)</pre>
<pre>.n(value)</pre>