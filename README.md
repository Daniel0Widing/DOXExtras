# DOX Extras
Adds extra features and dinos to the DinoOverhaul X (DOX) mod. All craftable items are crafted in the [DOX Extras Workbench](https://github.com/Daniel0Widing/DOXExtras#dox-extras-workbench). All recipes are automatically available in the DOX Extras Workbench to prevent engram spam.

## Installing the Mod
Log into Steam, go to [DOX Extras](https://steamcommunity.com/sharedfiles/filedetails/?id=2927749831), and subscribe to the mod. While you're at it, you should also subscribe to [DinoOverhaul X](https://steamcommunity.com/sharedfiles/filedetails/?id=710880648) since it doesn't make sense to use this mod without it. Then launch ARK and the mods should automatically download. When you create your world/server, place this mod directly after DOX in the mod load order for best results.

## Tiers
In DOX, Dino tiers go from Normal\*, to Apex, to Prime, to Ancient, to Primal.
But then there's also Alpha Apex, Apex Prime Unique, X, Y, and probably some I'm missing. I spent about about an hour going through the in-game documentation, online GoogleSheets database, spawn codes, and compiled mod files, and I'm still fairly certain I don't have the tiers in the right order.

So for DOX Extras, the dinosaur tiers are streamlined and consistant, while still trying to stay as close to DOX as possible. The tiers, in order, are:

**Prime -> Unique -> Ancient -> Primal**

Each tier has its own saddle and dinosaur spawner item, along with a corresponding color scheme which is applied to all matching dinosaurs, saddles, and spawners of each tier. The colors are:

| Tier | Color |
| --- | --- |
| Prime | Lime |
| Unique | Yellow |
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
| Base Torpor | 800 |
| Scale | 1.1 |
| Extra Tamed Speed Multiplier | 2.0 |
| Base Melee Damage | 96 / 64 |
| Minigun Damage | 333 |
| Minigun Range | 25000 |
| Minigun Fire Interval | 0.1 |
| Saddle Armor | 150 |

\+ Minigun Partial Armor Piercing
	
**Unique:**
| Stat | Data |
| --- | --- |
| Base Health | 1200 |
| Base Torpor | 1600 |
| Scale | 1.15 |
| Extra Tamed Speed Multiplier | 2.25 |
| Base Melee Damage | 144 / 96 |
| Minigun Damage | 420 |
| Minigun Range | 27500 |
| Minigun Fire Interval | 0.08 |
| Saddle Armor | 200 |

\+ Minigun Slow Effect

**Ancient:**
| Stat | Data |
| --- | --- |
| Base Health | 1600 |
| Base Torpor | 2400 |
| Scale | 1.2 |
| Extra Tamed Speed Multiplier | 2.5 |
| Base Melee Damage | 200 / 144 |
| Minigun Projectile Damage | 250 direct, 250 AOE |
| Minigun Projectile AOE Radius | 300 |
| Minigun Range | 30000 |
| Minigun Fire Interval | 0.075 |
| Saddle Armor | 250 |

\+ Minigun Full Piercing

\+ Minigun Torpor

\+ Minigun AoE	
	
**Primal:**
| Stat | Data |
| --- | --- |
| Base Health | 2000 |
| Base Torpor | 3200 |
| Scale | 1.25 |
| Extra Tamed Speed Multiplier | 3.0 |
| Base Melee Damage | 300 / 200 |
| Minigun Projectile Damage | 666 AOE |
| Minigun Projectile AOE Radius | 600 |
| Minigun Range | 35000 |
| Minigun Fire Interval | 0.05 |
| Saddle Armor | 350 |

\+ Minigun Stacking & Slowing Bleed

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
**Unique:**
```
cheat spawndino "Blueprint'/Game/Mods/DOXExtras/Dinos/Unique/Andrewsarchus/Andrewsarchus_Unique_Character_BP.Andrewsarchus_Unique_Character_BP'" 10 0 0 1269
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Unique/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_Unique.PrimalItem_DinoSpawner_Andrewsarchus_Unique'" 1 0 false
```
```	
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Unique/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusUniqueSaddle.PrimalItemArmor_AndrewsarchusUniqueSaddle'" 1 0 false
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
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Ammo/AdvancedElementBullet/PrimalItemAmmo_AdvancedElementBullet.PrimalItemAmmo_AdvancedElementBullet'" 1000 0 false
```
</details>
