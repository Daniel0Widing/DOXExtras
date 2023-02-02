# DOXExtras
Adds missing features and dinos to the DinoOverhaulX (DOX) mod. All craftable items are crafted in the DOX Extras Workbench, which can be unlocked at level 100. For best results place this mod directly after DOX in load order.

## Added Dinos:
### Andrewsarchus: 
The upgraded Andrewsarchus focuses on **Health** and **Minigun Damage**. Its regular attacks are lack luster compared to other upgraded dinosaurs, so its best place is either far away firing with its minigun, or upclose soaking up hits. All saddles for upgraded **Andrewsarchuses use Advanced Element Bullets**.

<details><summary>Prime:</summary>
	
```
Color: Lime
Base Health: 800
Scale: 1.1
Extra Tamed Speed Multiplier: 2.0 
Base Melee Damage: 96 | 64
Minigun Damage: 333
Minigun Range: 25000
Minigun Fire Interval: 0.1
Saddle Armor: 150
+ Minigun Partial Armor Piercing
```
_Spawner:_
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Prime/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_Prime.PrimalItem_DinoSpawner_Andrewsarchus_Prime'" 1 0 false
```
_Saddle:_
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Prime/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusPrimeSaddle.PrimalItemArmor_AndrewsarchusPrimeSaddle'" 1 0 false
```
</details>
	
<details><summary>Prime Unique:</summary>
	
```
Color: Yellow
Base Health: 1000
Scale: 1.15
Extra Tamed Speed Multiplier: 2.25 
Base Melee Damage: 144 | 96
Minigun Damage: 420
Minigun Range: 27500
Minigun Fire Interval: 0.08
Saddle Armor: 200
+ Minigun Slow Effect
```
_Spawner:_
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/PrimeUnique/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_PrimeUnique.PrimalItem_DinoSpawner_Andrewsarchus_PrimeUnique'" 1 0 false
```
_Saddle:_
```	
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/PrimeUnique/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusPrimeUniqueSaddle.PrimalItemArmor_AndrewsarchusPrimeUniqueSaddle'" 1 0 false
```
</details>
	
<details><summary>Prime Ancient:</summary>
	
```
Color: Magenta / Yellow
Base Health: 1200
Scale: 1.2
Extra Tamed Speed Multiplier: 2.5 
Base Melee Damage: 200 | 144
Minigun Damage: 500
Minigun Range: 30000
Minigun Fire Interval: 0.075
Saddle Armor: 250
+ Minigun Full Piercing
+ Minigun Torpor
+ Minigun AoE
```
_Spawner:_
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/PrimeAncient/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_PrimeAncient.PrimalItem_DinoSpawner_Andrewsarchus_PrimeAncient'" 1 0 false
```
_Saddle:_
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/PrimeAncient/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusPrimeAncientSaddle.PrimalItemArmor_AndrewsarchusPrimeAncientSaddle'" 1 0 false
```
</details>
	
<details><summary>Primal:</summary>
	
```
Color: DarkLavender / Glacial
Base Health: 1500
Scale: 1.25
Extra Tamed Speed Multiplier: 3.0 
Base Melee Damage: 300 | 200
Minigun Damage: 666
Minigun Range: 35000
Minigun Fire Interval: 0.05
Saddle Armor: 350
+ Minigun Stacking & Slowing Bleed
```
_Spawner:_
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Primal/Andrewsarchus/Spawner/PrimalItem_DinoSpawner_Andrewsarchus_Primal.PrimalItem_DinoSpawner_Andrewsarchus_Primal'" 1 0 false
```
_Saddle:_
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Dinos/Primal/Andrewsarchus/Saddle/PrimalItemArmor_AndrewsarchusPrimalSaddle.PrimalItemArmor_AndrewsarchusPrimalSaddle'" 1 0 false
```
</details>
	
## Added Items:
### Structures:
#### DOX Extras Workbench:
Used to craft all items from DOX Extras. Engram can be unlocked at level 100.
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Structures/DOXExtrasWorkbench/PrimalItemStructure_DOXExtrasWorkbench.PrimalItemStructure_DOXExtrasWorkbench'" 1 0 false
```

### Ammo:
#### Advanced Element Ammo:
An advanced bullet that uses element instead of gunpowder. 
```
cheat giveitem "Blueprint'/Game/Mods/DOXExtras/Items/Ammo/AdvancedElementBullet/PrimalItemAmmo_AdvancedElementBullet.PrimalItemAmmo_AdvancedElementBullet'" 1000 0 false
```
