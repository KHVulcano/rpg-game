# RPG iron tool colors

Iron swords, axes, pickaxes, shovels, and hoes read the first entry in the item's `minecraft:custom_model_data.colors` list and apply it to the iron parts. The handle remains unchanged. Without a color entry, the model renders in its original colors.

Example, give an iron pickaxe with red iron parts:

```mcfunction
/give @s minecraft:iron_pickaxe[minecraft:custom_model_data={colors:[16711680]}]
```

Use a packed RGB integer for the desired color (for example, `16711680` is `#FF0000`). Change the vanilla item definitions under `assets/minecraft/items/` only if you want to adjust the tint source; the split textures and models are in the `rpg` namespace.
