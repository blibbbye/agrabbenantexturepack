# Agrabbenan texture pack — Minecraft Java 26.3

## Custom item visuals

The nine images from `texturesforthepack` have been copied into the resource-pack texture folder, with one item-definition JSON and one model JSON per item.

| Item | Intended base item | Model ID |
|---|---|---|
| Black Requiem | Netherite spear | `minecraft:black_requiem` |
| Iron Dagger | Iron sword | `minecraft:iron_dagger` |
| Warbane | Iron sword | `minecraft:warbane` |
| Nightblight | Iron sword | `minecraft:nightblight` |
| Rimethaw | Bow | `minecraft:rimethaw` |
| Horse | Paper (scroll) | `minecraft:horse` |
| Rage | Paper (scroll) | `minecraft:rage` |
| Snowstorm | Paper (scroll) | `minecraft:snowstorm` |
| Wraithcall | Paper (scroll) | `minecraft:wraithcall` |

## Give commands

Run these in Minecraft Java 26.3 with cheats enabled and this pack enabled. The `item_model` component selects the matching item definition.

```mcfunction
give @p minecraft:netherite_spear[minecraft:item_model="minecraft:black_requiem",minecraft:custom_name='{"text":"Black Requiem","italic":false}'] 1
give @p minecraft:iron_sword[minecraft:item_model="minecraft:iron_dagger",minecraft:custom_name='{"text":"Iron Dagger","italic":false}'] 1
give @p minecraft:iron_sword[minecraft:item_model="minecraft:warbane",minecraft:custom_name='{"text":"Warbane","italic":false}'] 1
give @p minecraft:iron_sword[minecraft:item_model="minecraft:nightblight",minecraft:custom_name='{"text":"Nightblight","italic":false}'] 1
give @p minecraft:bow[minecraft:item_model="minecraft:rimethaw",minecraft:custom_name='{"text":"Rimethaw","italic":false}'] 1
give @p minecraft:paper[minecraft:item_model="minecraft:horse",minecraft:custom_name='{"text":"Horse","italic":false}'] 1
give @p minecraft:paper[minecraft:item_model="minecraft:rage",minecraft:custom_name='{"text":"Rage","italic":false}'] 1
give @p minecraft:paper[minecraft:item_model="minecraft:snowstorm",minecraft:custom_name='{"text":"Snowstorm","italic":false}'] 1
give @p minecraft:paper[minecraft:item_model="minecraft:wraithcall",minecraft:custom_name='{"text":"Wraithcall","italic":false}'] 1
```

## Important limits

- This resource pack handles appearance only. The JSON models use each PNG as a generated flat item sprite; they do not create fully 3D spear, sword, bow, or scroll geometry.
- The scroll right-click abilities need a datapack or server plugin. No ability effects were specified yet, so these items are currently visual scrolls only.
- The base item names in the give commands should be checked in-game on the exact 26.3 build. If that build uses a different spear item ID, replace `minecraft:netherite_spear` with the correct vanilla spear ID.
