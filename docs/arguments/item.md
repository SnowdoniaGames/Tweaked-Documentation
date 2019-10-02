# item ![](/img/version_1.12.png)![](/img/version_1.14.png)

An item can be used to specify any minecraft item or block.

An item is a type of [ingredient](/arguments/ingredient/) and can therefore be used as one in any argument.

!!! note
	The [hand command](/commands/hand/) can be used to easily get the resourceLocation of an item.

## Argument
An item is specified using the "item" keyword.

<pre>item(resourceLocation)</pre>

!!! example
	```python
	#creates an item of type diamond
	item(minecraft:diamond)
	```

<br>

## Modifiers

### Count ![](/img/version_1.12.png)![](/img/version_1.14.png)

Specifies the number of the the item, by default this is 1.

<pre>.count(amount)</pre>
<pre>.c(amount)</pre>

<br>

### Meta ![](/img/version_1.12.png)

Specifies the metadata value assigned to the item.

<pre>.meta(value)</pre>
<pre>.m(value)</pre>

<br>

### NBT ![](/img/version_1.12.png)![](/img/version_1.14.png)

Specifies any NBT information assigned to the item.

<pre>.nbt(value)</pre>
<pre>.n(value)</pre>

<br>

### Enchant ![](/img/version_1.12.png)![](/img/version_1.14.png)

Helper that can assign an enchantment to the item.

<pre>.enchant(name:level)</pre>
<pre>.e(name:level)</pre>

!!! example
	```python
	#adds the Protection 4 enchantment to a diamond sword
	item(minecraft:diamond_sword).enchant(minecraft:protection:4)
	```