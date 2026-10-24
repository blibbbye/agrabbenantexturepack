# Agrabbenan texture pack — Minecraft Java 26.3

## Custom item visuals

| Item | Intended base item | Model ID |
|---|---|---|
| Black Requiem | Spear | `minecraft:black_requiem` |
| Iron Dagger | Sword | `minecraft:iron_dagger` |
| Warbane | Sword | `minecraft:warbane` |
| Nightblight | Sword | `minecraft:nightblight` |
| Rimethaw | Bow | `minecraft:rimethaw` |
| Horse | Paper (scroll) | `minecraft:horse` |
| Rage | Paper (scroll) | `minecraft:rage` |
| Snowstorm | Paper (scroll) | `minecraft:snowstorm` |
| Wraithcall | Paper (scroll) | `minecraft:wraithcall` |

## Model updates

- **Black Requiem:** uses the normal texture for inventory/GUI and the separate `blackrequiem_in_hand.png` texture for held display. The held model is a thin, extruded 3D sprite, with transparent edges. It is a starting point, not a fully sculpted spear made from separate blade and shaft geometry.
- **Iron Dagger, Warbane and Nightblight:** use Minecraft's `handheld` model parent, which supplies the usual sword-style held transforms.
- **Rimethaw:** uses Minecraft's vanilla bow and bow-pulling model parents so the item can use the normal bow hold transforms and pulling-state model selection. All three pulling states currently reuse the same custom texture, so there is no separate drawn artwork yet.
- **Scrolls:** remain flat generated sprites.
- **No in-game test has been run yet.** Resource-pack behavior and item IDs should be checked in the exact Minecraft 26.3 build.

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

- This resource pack changes appearance only; it does not add right-click abilities to the scrolls.
- Confirm the base spear item ID on your exact 26.3 build. If it differs, replace `minecraft:netherite_spear` in the command with the correct spear item ID.
