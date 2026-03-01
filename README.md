# Enhanced Firearms
A mod for the game Vintage Story.


```mermaid
---
config:
  theme: neo-dark
---
flowchart TD
    %% Existing Items
    salt[["Salt"]]
    flax[["Flax"]]
    fat[["Lump of Fat"]]
    saltpeter[["Saltpeter"]]
    brassPlate[["Brass Plate"]]
    hammer[[Hammer]]
    knife[[Knife]]
    shears[[Shears]]
    saltpeter[["Saltpeter"]]
    
    
    %% Existing Fluids
    sulfuric((("Sulfuric Acid")))
    slakedLime((("Slaked Lime")))
    water((("Water")))
    
    %% New Fluids
    nitroglycerine(("Nitroglycerine"))
    sodiumHydroxide(("Sodium Hydroxide"))
    nitratingMix(("Nitrating Mixture"))
    
    

    
    %% New Items
    sodiumCarb["Sodium Carbonate"]
    glycerol["Glycerol"]
    nitroJelly["Nitroglycerine Gelatin"]
    cartridgeLoad["Cartridge Loads"]
    emptyCases["Empty Cases"]
    cartridge["Cartridge"]
    bullet["Bullet"]
    bulletDie["Bullet Die"]
    processingDie["Processing Die"]
    sodiumSulfate["Sodium Sulfate"]
    blackAsh["Black Ash"]
    sodaAshWet["Soda Ash *Wet*"]
    degummedFlax["Degummed Flax"]
    nitroBundle["Nitrocellulose Bundle"]
    nitroUnits["Nitrocellulose Units"]
    
    
    %% Processes
    salt-- Cook --> sodiumSulfate
    sulfuric -- Cook --> sodiumSulfate
    sodiumSulfate -- Cook --> blackAsh
    blackAsh -- Barrel --> sodaAshWet
    sodaAshWet -- Drying--> sodiumCarb
    sodiumCarb -- Barrel --> sodiumHydroxide
    slakedLime -- Barrel --> sodiumHydroxide
    flax -- Barrel --> degummedFlax
    sodiumHydroxide -- Barrel --> degummedFlax
    degummedFlax -- Cook --> nitroBundle
    sulfuric -- Cook --> nitroBundle
    saltpeter -- Cook --> nitroBundle
    nitroBundle --> nitroUnits
    fat -- Cook --> glycerol
    sodiumHydroxide -- Cook --> glycerol
    saltpeter -- Cook --> nitratingMix
    water-- Cook --> nitratingMix
    sulfuric -- Cook --> nitratingMix
    glycerol -- Cook --> nitroglycerine
    nitratingMix -- Cook --> nitroglycerine
    nitroUnits --> cartridgeLoad
    nitroglycerine --> nitroJelly
    nitroJelly --> cartridgeLoad
    brassPlate --> emptyCases
    bullet --> cartridge
    cartridgeLoad --> cartridge
    emptyCases --> cartridge
    hammer --> cartridge
    knife --> cartridgeLoad
    shears --> nitroUnits
    bulletDie --> emptyCases
    processingDie --> cartridgeLoad
```
