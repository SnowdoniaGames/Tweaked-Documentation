# Your First Script

This is a short tutorial that will take you through some of the basics of scripting.

<br>

---
## Creating the script file

Create a new file named `test.tweak` inside the `/Tweaked/Scripts` directory

For this example we will print a message to the log file. `print` is a special action that we can use to do this.

Inside `test.tweak` paste the following code :  
```
print : "Test Message";
```

Now run minecraft and once it's loaded look inside the `tweaked.log` file. You should see that your script has output the specified message.

<br>

---
## Modifying crafting recipes

Next, lets try modifying some default recipes.

We will change the amount of torches in the vanilla torch recipe to give 16 torches rather than 4.

First we will use [recipes.remove](/actions/vanilla/recipes/#remove) to remove the default torch recipe, add the following code :
```python
recipes.remove : item(minecraft:torch);
```

And now we can use [recipes.shaped](/actions/vanilla/recipes/#shaped) to add the replacement recipe, add the following code :
```python
recipes.shaped : "bonus_torch", item(minecraft:torch).count(16), null, item(minecraft:coal), null, null, ore(stickWood);
```

![](/img/crafting.png)

<br>