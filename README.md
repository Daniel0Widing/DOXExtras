# DOX Extras
Adds extra features and dinos to the DinoOverhaul X (DOX) mod. All craftable items are crafted in the [DOX Extras Workbench](https://github.com/Daniel0Widing/DOXExtras#dox-extras-workbench). All recipes are automatically available in the DOX Extras Workbench to prevent engram spam.

## Installing the Mod
Log into Steam, go to [DOX Extras](https://steamcommunity.com/sharedfiles/filedetails/?id=2927749831), and subscribe to the mod. While you're at it, you should also subscribe to [DinoOverhaul X](https://steamcommunity.com/sharedfiles/filedetails/?id=710880648) since it doesn't make sense to use this mod without it. Then launch ARK and the mods should automatically download. When you create your world/server, place this mod directly after DOX in the mod load order for best results.

## GameUserSettings.ini Configuration
Add the following section to the bottom of your GameUserSettings.ini file and change the settings you want changed. The names should all be self-explanatory.

```
[DOXExtras]
CanSacrificeClones=false
```

## Tiers
In DOX, dino tiers go from Normal\*, to Apex, to Prime, to Unique/Ancient, to Primal, with some special cases sprinkled in.

For DOX Extras, dino tiers are entirely linear. This means each tier is better than the previous tier and worse than the next tier. The tiers, in order, are:

**Prime -> Rare -> Ancient -> Primal**

These tiers line up with the standard DOX tiers, with Rare falling in-between Prime and Ancient, and Unique being left out.

Each tier has its own saddle and dinosaur spawner item, along with a corresponding color scheme which is applied to all matching dinosaurs, saddles, and spawners of each tier. The colors are:

| Tier | Color |
| --- | --- |
| Prime | Lime |
| Rare | Yellow |
| Ancient | Magenta & Yellow |
| Primal | DarkLavender & Glacial |

_If the color names look strange, that's because they are the color code names used in ARK's code_

## Added Dinos:
### Andrewsarchus
<details><summary>------- Info ---------</summary>
	
The upgraded Andrewsarchus focuses on **Health** and **Minigun Damage**. Its regular attacks are lack luster compared to other upgraded dinosaurs, so its best place is either far away firing with its minigun, or upclose soaking up hits. All saddles for upgraded Andrewsarchuses use [Advanced Element Bullets](https://github.com/Daniel0Widing/DOXExtras#advanced-element-bullets).

**Prime:**
| Stat | Data |
| --- | --- |
| Base Health | 800 |
| Base Stamina | 400 |
| Base Torpor | 800 |
| Base Melee Damage Bonus | 1.5 |
| Base Speed Multiplier Bonus | 0.5 |
| Scale | 1.1 |
| Speed Boosts | 6 |
| Minigun Damage | 333 |
| Minigun Range | 25000 |
| Minigun Fire Interval | 0.1 |
| Saddle Armor | 150 |

\+ Minigun Partial Armor Piercing
	
\+ Fall Damage Reduced by 75%
	
\+ Provides Insulation to Rider
	
**Rare:**
| Stat | Data |
| --- | --- |
| Base Health | 1200 |
| Base Stamina | 500 |
| Base Torpor | 1600 |
| Base Melee Damage Bonus | 2.5 |
| Base Speed Multiplier Bonus | 0.75 |
| Scale | 1.15 |
| Speed Boosts | 8 |
| Minigun Damage | 420 |
| Minigun Range | 27500 |
| Minigun Fire Interval | 0.08 |
| Saddle Armor | 200 |

\+ Minigun Slow Effect

**Ancient:**
| Stat | Data |
| --- | --- |
| Base Health | 1800 |
| Base Stamina | 625 |
| Base Torpor | 3200 |
| Base Melee Damage Bonus | 4.5 |
| Base Speed Multiplier Bonus | 1.0 |
| Scale | 1.2 |
| Speed Boosts | 10 |
| Minigun Projectile Damage | 250 direct, 250 AOE |
| Minigun Projectile AOE Radius | 300 |
| Minigun Range | 30000 |
| Minigun Fire Interval | 0.075 |
| Saddle Armor | 250 |

\+ Minigun Full Piercing

\+ Minigun Torpor

\+ Minigun AoE

\+ Fall Damage Immunity

\+ **Hog Hiatus** Buff: _(NYI)_
```
When the Andrewsarchus's health drops dangerously low, it prepares to flee: 
- All active buffs are cleared and no new buffs can be applied for the duration. 
- All speed boosts are recharged.
- Stamina is completely refilled.
- Speed, handling, and damage reduction increase, but attack damage sharply decreases.
After the buff runs out, the Andrewsarchus cannot activate the buff again or be cryopoded until it calms down.
```
	
**Primal:**
| Stat | Data |
| --- | --- |
| Base Health | 2700 |
| Base Stamina | 781.25 |
| Base Torpor | 6400 |
| Base Melee Damage Bonus | 8 |
| Base Speed Multiplier Bonus | 1.25 |
| Scale | 1.25 |
| Speed Boosts | 12 |
| Minigun Projectile Damage | 666 AOE |
| Minigun Projectile AOE Radius | 600 |
| Minigun Range | 35000 |
| Minigun Fire Interval | 0.05 |
| Saddle Armor | 350 |

\+ Minigun Stacking & Slowing Bleed

\+ **Halcyon Hog** Buff replaces **Hog Hiatus** Buff: _(NYI)_
```
When the Andrewsarchus's health drops dangerously low, it enters a serene state, strengthening its mind and body: 
- All active buffs are cleared and no new buffs can be applied for the duration. 
- All speed boosts are recharged.
- Stamina is completely refilled.
- Speed and handling slightly increase.
- Damage reduction and melee damage greatly increase.
- Melee attacks inflict damage in a larger area with more knockback.
After the buff runs out, the Andrewsarchus cannot activate the buff again or be cryopoded until it recovers its morale.
```
	
\+ **Hog of Havoc** Ability: _(NYI)_ _(Under consideration)_
```
When the Andrewsarchus's life ends, it channels its inner beast and rampages:
- All active buffs are cleared and no new buffs can be applied.
- All speed boosts are recharged.
- Stamina becomes infinite.
- Speed and handling greatly increase.
- Melee attacks rapidly deal massive amounts of true damage in a large area.
- Becomes immune to all damage.
- Cannot be cryopoded during this state.
After this state runs out, the Andrewsarchus disintegrates, leaving nothing but its legacy behind.
```

<details><summary>---- Spawn Codes: ------</summary>

**Prime:**
```
cheat spawndino "Blueprint'/Game/Mods/DOXExtras/Dinos/Prime/Andrewsarchus/Andrewsarchus_Prime_Character_BP.Andrewsarchus_Prime_Character_BP'" 10 0 0 1269
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Prime/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_Prime.PrimalItem_DinoSpawner_Andrewsarchus_Prime'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Prime/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusPrimeSaddle.PrimalItemArmor_AndrewsarchusPrimeSaddle'" 1 0 false
```
**Rare:**
```
cheat spawndino "Blueprint'/Game/Mods/DOXExtras/Dinos/Rare/Andrewsarchus/Andrewsarchus_Rare_Character_BP.Andrewsarchus_Rare_Character_BP'" 10 0 0 1269
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Rare/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_Rare.PrimalItem_DinoSpawner_Andrewsarchus_Rare'" 1 0 false
```
```	
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Rare/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusRareSaddle.PrimalItemArmor_AndrewsarchusRareSaddle'" 1 0 false
```
**Ancient:**
```
cheat spawndino "Blueprint'/Game/Mods/DOXExtras/Dinos/Ancient/Andrewsarchus/Andrewsarchus_Ancient_Character_BP.Andrewsarchus_Ancient_Character_BP'" 10 0 0 1269
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Ancient/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_Ancient.PrimalItem_DinoSpawner_Andrewsarchus_Ancient'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Ancient/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusAncientSaddle.PrimalItemArmor_AndrewsarchusAncientSaddle'" 1 0 false
```
**Primal:**
```
cheat spawndino "Blueprint'/Game/Mods/DOXExtras/Dinos/Primal/Andrewsarchus/Andrewsarchus_Primal_Character_BP.Andrewsarchus_Primal_Character_BP'" 10 0 0 1269
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Primal/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_Primal.PrimalItem_DinoSpawner_Andrewsarchus_Primal'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Primal/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusPrimalSaddle.PrimalItemArmor_AndrewsarchusPrimalSaddle'" 1 0 false
```
</details>
</details>

## Added Items:
### Structures:
#### DOX Extras Workbench
<details><summary>------- Info ---------</summary>
	
Used to craft all items from DOX Extras. Engram can be unlocked at level 100.
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Structures/DOXExtrasWorkbench/PrimalItemStructure_DOXExtrasWorkbench.PrimalItemStructure_DOXExtrasWorkbench'" 1 0 false
```
</details>

### Ammo:
#### Advanced Element Bullets
<details><summary>------- Info ---------</summary>
	
An advanced bullet that uses element instead of gunpowder. 

**Each craft gives 100 bullets by default.**
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Ammo/AdvancedElementBullet/PrimalItemAmmo_AdvancedElementBullet.PrimalItemAmmo_AdvancedElementBullet'" 1000 0 false
```
</details>


### Consumables:
#### DOX Extras Sacrifice Potion
<details><summary>------- Info ---------</summary>
	
Serves the same role as DOX Sacrifice Elixir, with a few tweaks:
- Only works on DOX Extras dinos
- Force feed to dinos to sacrifice them
- Gives back 1 Prime Heart, or however many Prime Hearts were used to craft the spawner for the sacrificed dinos
- Does not work on cloned dinosaurs (can be enabled in config)

Crafted from DOX Sacrifice Elixir.
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Consumable/DOXExtrasSacrificePotion/PrimalItemConsumable_DOXExtrasSacrificePotion.PrimalItemConsumable_DOXExtrasSacrificePotion'" 100 0 false
```
</details>

#### Armor Repair Kit
<details><summary>------- Info ---------</summary>
	
Instantly repairs an armor piece equipped or in your inventory when used, but consumes the kit on use and only works in player inventories.
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Consumable/ArmorRepairKit/PrimalItemConsumable_ArmorRepairKit.PrimalItemConsumable_ArmorRepairKit'" 40 0 false
```
</details>
