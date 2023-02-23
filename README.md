# DOX Extras
Adds extra features and dinos to the DinoOverhaul X (DOX) mod. All craftable items are crafted in the [DOX Extras Workbench](https://github.com/Daniel0Widing/DOXExtras#dox-extras-workbench). All recipes are automatically available in the DOX Extras Workbench to prevent engram spam.

## Installing the Mod
Log into Steam, go to [DOX Extras](https://steamcommunity.com/sharedfiles/filedetails/?id=2927749831), and subscribe to the mod. While you're at it, you should also subscribe to [DinoOverhaul X](https://steamcommunity.com/sharedfiles/filedetails/?id=710880648) since it doesn't make sense to use this mod without it. Then launch ARK and the mods should automatically download. When you create your world/server, place this mod directly after DOX in the mod load order for best results.

## GameUserSettings.ini Configuration
Add the following section to the bottom of your GameUserSettings.ini file and change the settings you want changed. The names should all be self-explanatory.

```
[DOXExtras]
CanSacrificeClones=False
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

## Damage
Damage in ARK generally works by multiplying incoming damage by all resistance modifiers.
```
Recieved Damage = Incoming Damage * Resistance Modifiers
```
where
```
Resistance Modifiers = Armor multiplier * Bone multiplier * Buff multiplier(s) * Inate multiplier(s)
```
These resistance modifiers in more detail are:
| Type | Explaination | Examples |
| --- | --- | --- |
| Armor | Resistance that scales with the equipped armor rating | Saddles, equipped armor |
| Bone | Resistance based on where the damage impact was | Turtle shell, Trike head |
| Buff | Resistance that is active as long as the buff is | Yuty Courage buff, Imprinting buff |
| Inate | Resistance to certain damage types built into some dinos | Many dinos take reduced damage from ranged attacks |

How resistance modifiers affect damage is based on the damage type of the damage. The following are the _general_ categories damage types fall into:
| Type | Affected by | Examples |
| --- | --- | --- |
| Normal | Armor, all modifiers | Dilo bite, Rex bite, Firearms |
| Piercing | all/most modifiers | Manta attacks, Theri slashes, Turrets |
| Passive | Inate modifiers | Wyverns/Basalisk poison |
| True | Nothing | Hellbound Hog bites, (does not exist in vanilla ARK) |

On top of this, damage can also be adjusted after all modifiers are taken into account but before it is applied. This adjustment is generally pretty rare, but is very dynamic. Some adjustments involve limiting maximum damage taken (tiered Andrewsarchus), or adding additional damage-type agnostic multipliers (Stego Hardened Plate mode). As this adjustment takes place after resistance calculations, it is capable of reducing true damage.

_Disclaimer: This is my current understanding of how damage works in ARK from going through the source files and working on this mod. If you see something incorrect with this understanding, please let me know._

## Added Dinos:
### Andrewsarchus
<details><summary>------- Info ---------</summary>
	
The upgraded Andrewsarchus focuses on **Health** and **Support**. Its damage output is lack luster compared to similar level tames, so it's best used to soak up damage while other dinos dish out damage. Many of its attacks, especially at higher tiers, inflict debuffs on enemies hit, and all tiers provide AOE healing to nearby friendlies. It also has a scaling damage cap which makes it excellent for tanking very powerful attacks without getting 1-shot.
	
All saddles for upgraded Andrewsarchuses use [Advanced Element Bullets](https://github.com/Daniel0Widing/DOXExtras#advanced-element-bullets).

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
| AOE Healing | 250 HP/s |
| Damage Cap | 100000 |
| Torpor Cap | 125000 |

\+ Minigun Deals Piercing Damage
	
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
| AOE Healing | 500 HP/s |
| Damage Cap | 75000 |
| Torpor Cap | 100000 |

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
| AOE Healing | 750 HP/s |
| Damage Cap | 50000 |
| Torpor Cap | 75000 |

\+ Minigun Deals Passive Damage

\+ Minigun Torpor

\+ Minigun AoE

\+ Fall Damage Immunity

\+ **Hog Hiatus** Buff:
```
When the Andrewsarchus's health drops dangerously low (15%), it prepares to flee: 
- All active buffs are cleared and no new buffs can be applied for the duration (30 sec). 
- All speed boosts are recharged, but cannot be activated until buff expires.
- Stamina becomes infinite.
- Speed (+50%) and damage reduction (+99.5%) increase, but attack damage sharply decreases (-95%).
- Heals 25% of max HP over duration
After the buff runs out, the Andrewsarchus cannot activate the buff again until it recovers (15 min).
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
| AOE Healing | 1250 HP/s |
| Damage Cap | 25000 |
| Torpor Cap | 50000 |

\+ Minigun Stacking & Slowing Bleed Effect

\+ **Halcyon Hog** Buff replaces **Hog Hiatus** Buff:
```
When the Andrewsarchus's health drops dangerously low (15%), it enters a serene state, strengthening its mind and body and emboldening its allies: 
- All active buffs are cleared and no new buffs can be applied for the duration (45 sec). 
- All speed boosts are recharged, but cannot be activated until buff expires.
- Stamina becomes infinite.
- Speed (+25%) increases slightly. 
- Heals 33% of max HP instantly
- Damage reduction (+98%) and melee damage (+150%) greatly increase.
- Main melee attack inflicts damage in a larger area (+200%) with more knockback (+200%).
- AOE Healing buff (+5000 HP/s) to all nearby friendlies (and self) for duration 
After the buff runs out, the Andrewsarchus cannot activate the buff again until it recovers (15 min).
```
	
\+ **Hellbound Hog** Ability:
```
When the Andrewsarchus reaches death's door, it takes its final stand before crossing the threshold:
- All active buffs are cleared and no new buffs can be applied.
- Stamina becomes infinite.
- Speed (+37.5%) greatly increases.
- Melee damage (+500%) massively increases
- Main attack deals true damage within a massive range (+300%) and a powerful DOT
- Becomes immune to all damage.
- Cannot be cryopoded during this state.
After this state runs out (60 sec), the Andrewsarchus's body turns to fire and plumets into hell, leaving behind a gravestone with its items where it hits the ground. (｀д´)ゝ 🫡
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
	
Similar to the DOX Sacrifice Elixir, but an upgraded version:
- Works on both DOX and DOX Extras dinos
- Force feed to dinos to sacrifice them
- Gives a number of Prime Hearts based on the tier of the sacrificed dino
- For dinos from crafted spawners, gives the number of Prime Hearts used to craft the spawner
- Does not work on cloned dinosaurs (can be enabled in config)

Crafting is more expensive early game, but less grindy late game.
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Consumables/DOXExtrasSacrificePotion/PrimalItemConsumable_DOXExtrasSacrificePotion.PrimalItemConsumable_DOXExtrasSacrificePotion'" 100 0 false
```
</details>

#### Armor Repair Kit
<details><summary>------- Info ---------</summary>
	
Instantly repairs an armor piece equipped or in your inventory when used, but consumes the kit on use and only works in player inventories.
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Consumables/ArmorRepairKit/PrimalItemConsumable_ArmorRepairKit.PrimalItemConsumable_ArmorRepairKit'" 40 0 false
```
</details>

#### V-Mate
<details><summary>------- Info ---------</summary>
	
Are your dinos feeling lonely because they don't have a mate? Worry not, for we have the technology! The patent-pending V-Mate provides your lonely dinosaurs with their very own virtual mate! Just use it on a dinosaur and watch them recieve all the benefits of a mate, without actually needing one!

Works on all dinosaur genders (or lack thereof), because everyone deserves love!
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Consumables/V-Mate/PrimalItemConsumable_V-Mate.PrimalItemConsumable_V-Mate'" 1 0 false
```
</details>

### Resources:
#### Primal Remnants
<details><summary>------- Info ---------</summary>
	
The condensed energy left behind by a Primal dinosaur when it is sacrificed. Used for crafting DOX Extras Primal spawners. One for each type of DOX Primal.

Created by using a DOX Extras Sacrifice Potion on a **DOX** Primal dinosaur.
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Resources/DOXPrimalRemnants/Dragon/PrimalItemResource_DragonPrimalRemnant.PrimalItemResource_DragonPrimalRemnant'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Resources/DOXPrimalRemnants/Gorilla/PrimalItemResource_GorillaPrimalRemnant.PrimalItemResource_GorillaPrimalRemnant'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Resources/DOXPrimalRemnants/Manticore/PrimalItemResource_ManticorePrimalRemnant.PrimalItemResource_ManticorePrimalRemnant'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Resources/DOXPrimalRemnants/RockGolem/PrimalItemResource_GolemPrimalRemnant.PrimalItemResource_GolemPrimalRemnant'" 1 0 false
```
</details>

