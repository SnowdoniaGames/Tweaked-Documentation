# Your First Script

This is a short tutorial that will provide a practical use of for loops.

<br>

---
## Without using a for loop

For this example assume that we want to both remove recipes and hide a list of five items.

Normally the script to do this would look like :

```python
recipes.remove : item(minecraft:torch);
recipes.remove : item(minecraft:stone);
recipes.remove : item(minecraft:cobblestone);
recipes.remove : item(minecraft:coal);
recipes.remove : item(minecraft:diamond);

jei.hide : item(minecraft:torch);
jei.hide : item(minecraft:stone);
jei.hide : item(minecraft:cobblestone);
jei.hide : item(minecraft:coal);
jei.hide : item(minecraft:diamond);
```

While this code would work fine, when dealing with potentially hundreds of items it can become unwieldy.

<br>

---
## Using a for loop

A better way to achieve the same result as above is to use a for loop.

First we place the items we want to remove and hide in a list, then we add a for loop that runs actions on each item :

```python
define remove : [
	item(minecraft:torch),
	item(minecraft:stone),
	item(minecraft:cobblestone),
	item(minecraft:coal),
	item(minecraft:diamond)
]

for var(remove) {
	recipes.remove : var;
	jei.hide : var;
}
```

This would have exactly the same effect as the above script, except being more compact and easier to modify later.

<br>