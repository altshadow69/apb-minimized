 
## Guide

Icon images can be easily embedded within the localization file this guide shows you how to do it step by step.  

> [!NOTE]
> The HUDIcon and HUDTexture, can not be overlaped or underlaped it will treat as a text.

Keep in mind that i create it this guide through trial and error.  
Freely contact me for suggestions or information.

## Extension between HUDIcon / HUDTexture

`HUDIcon` Usage for "Generic_Icons_Master" Texture Sheet Only! can be seems [Here!](https://i.imgur.com/E506K3r.png)

`HUDTexture` Usage for the In Game Hud Textures Images, for examples `KillIcon_Pistol_FBW` `Weapon_Pistol_FBW`

<details>
<summary> $${\color{blue}[‎ ‎ ‎ examples‎of‎HUDTextures‎can‎be‎seem‎here.‎Click‎Here!‎ ‎ ‎ ]</Click>}$$ :dizzy:</summary>
	
```
  Icon_Locker_Generic_Token
  Weapon_Pistol_FBW
  KillIcon_Pistol_FBW
  Clothing_M_Hairwear_Hat_TopHatTall
  Contact_YoDawg
  Vehicle_PatriotVegasG20
```	
</details>

## Intimidation

| Command | Description |
| :--- | :--- |
| *HUDIcon* | |
| ```<APB_Images:APBCash;HUDIcon=TRUE>``` | if the HUDIcon text is in, User Interface Element. — _"APBUserInterface.INT"_  etc. |
| ```<hudicon:APBCash>``` | if the HUDIcon text is in, HUD Message Element. — _"HUDMessages.INT"_ |
| *HUDTexture* | |
| ```<APB_Images:Ceremony_Cash;HUDTexture=TRUE>``` | if the HUDTexture text is in, User Interface Element. — _"APBUserInterface.INT"_  etc. |
| ```<hudtexture:Ceremony_Cash>``` | if the HUDTexture text is in, HUD Message Element. — _"HUDMessages.INT"_ |

## Resizing

if you want to resize the Icon Image then use "XL=16 YL=16" and then add "Resize=TRUE" next to it
| Command | Description |
| :--- | :--- |
| *HUDIcon* | |
| ```<APB_Images:APBCash;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>``` | Resizeing HUDIcon text in, User Interface Element.|
| ```<hudicon:APBCash;XL=16 YL=16 Resize=TRUE>``` | Resizeing HUDIcon text in, HUD Message Element.|  
| *HUDTexture* | |
| ```<APB_Images:Ceremony_Cash;XL=16 YL=16 Resize=TRUE HUDTexture=TRUE>``` | Resizeing HUDTexture In User Interface Element. |
| ```<hudtexture:Ceremony_Cash;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>``` | Make sure to add "HUDIcon=TRUE" to enable it |

> [!IMPORTANT]
> Resizing the HUDTexture might work, but it will specifically bug out and revert to its original size.  
> Mixing hudicon with hudtexture will not prevent the bug related to the original size

---

## Listing [ Icon / Texture ]

The naming must be specific. this listing is working progress

```
/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /

 •  —  —  —  —  —  —  —  —  —  Icons
	
  None   >   Shows Nothing

  APBCash
  Icon_JokerTickets
  Rating
	
  Status_None
  Status_Ready
  Status_AFK
  Status_DND
  Status_Busy   >   Not Working
  Status_Arrested
  Status_Stunned
  Status_Dead
  Status_Driving
  Status_Crown
  Status_TaskParticipant   >   Shows Nothing ( Note: Probably its the weird thumbs up icon in the texture sheet, but never used. )
  Status_NonTaskParticipant
  Status_Disconnected   >   Not Working
  Status_OutOfDistrict   >   Not Working

  VOIP_Active_High
  VOIP_Active_Medium
  VOIP_Active_Low
  VOIP_InChannel
  VOIP_Muted
  VOIP_NotInChannel

  Task_Checkpoint
  Task_Checkpoint_Occ
  Task_Target
  Task_Target_Occ
  Task_Item
  Task_Item_Occ   >   Reskins
  Task_Target_VIP 
  Task_Item_Vehicle   >   Reskins

  AmmoVending
  Contact
  Waypoint
  Waypoint_Leader
  DisplayPoint
  SpawnZone
  Mailbox
  PlayerVehicle
  PlayerVehicleWithTaskItem   >   Reskin
  VehicleSpawn
  VehicleRepair
  MobileRadarTower
  Elective_Corpse   >   Reskin

  Faction_Criminal
  Faction_Enforcer

  GroupPlayer
  GroupLeader   >   White Covered
  OppositionPlayer   >   RTW / Shows Nothing

  StashDropOff   >   White Covered
  OpenWorldDropOff_Small   >   White Covered

  MarketplaceZone
  InteractionPoint_MusicStudio   >   Not Working
  InteractionPoint_SymbolEditor
  InteractionPoint_Wardrobe
  InteractionPoint_Garage
  InteractionPoint_Vault
  
  PDA   >   RTW / Shows Nothing

 +  —  —  —  Taggers

  Spotter

  Tagger_Default
  Tagger_Duck
  Tagger_Valentines
	
  Tagger_Suit_Clubs
  Tagger_Suit_Diamond
  Tagger_Suit_Hearts
  Tagger_Suit_Spades
  Tagger_Suit_Joker

  Tagger_PurpleCat
  Tagger_Cat
  Tagger_Rapid99
  Tagger_Sluttles
  Tagger_Reaper


 +  —  —  —  Events

  Minigame_GunGame
  Minigame_GunGame_Joker

  Minigame_Mugging_Item_Egg
  Minigame_Mugging_Protagonist_Easter
  Minigame_Mugging_Carrier_Easter
  
  Minigame_Mugging_Item
  Minigame_Mugging_Protagonist
  Minigame_Mugging_Carrier
  Minigame_Mugging_NPC

  Minigame_GoldenWeapon_Easter_Protagonist
  Minigame_GoldenWeapon_Explosive
	
  Minigame_Infection_Survivor
  Minigame_Infection_Pumpkin
  Minigame_Infection_Headless
  
  Minigame_SlayBells_FrozenBlock
  Minigame_SnowballFight
	
  Minigame_Epidemic_Warehouse
  Minigame_Epidemic_Hazmat
  Minigame_Epidemic_Zombicine
  Minigame_Epidemic_Undedox
  Minigame_Epidemic_Necrocite
  Minigame_Epidemic_Barrel
  Minigame_Epidemic_BarrelStack

  Minigame_Survival_Cash
  Minigame_Survival_WeaponSecondaryUnlock
  Minigame_Survival_WeaponLegendary
  Minigame_Survival_Bomb
  Minigame_Survival_Hazmat

/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /

 •  —  —  —  —  —  —  —  —  —  Textures

  Icon_Locker_Generic_Token
  Icon_Locker_Generic_Symbols
  Icon_Reward_Emote
  Icon_Reward_Vinyl
  Icon_Reward_Bio   >   Not Working
  Icon_GenericBundle_Sack
  Icon_GenericBundle_Crate
  Icon_Scoreboard_Generic_Clan
  Icon_Scoreboard_Generic_Player
  Icon_Medal_Default
	
  Icon_Title_Question
  Icon_Title_Symbol_Save
  Icon_Title_Rename
  Icon_Title_Destroy
  
  CharacterCreation

  Ceremony_GenericUnlock
  Ceremony_WinStreak
  Ceremony_KillStreak
  Ceremony_ArrestStreak
  Ceremony_TutorialComplete
  Ceremony_NewWeapons
  Ceremony_NewVehiclesParts
  Ceremony_NewThemesInstruments
  Ceremony_NewUpgrades
  Ceremony_NewSymbols
  Ceremony_NewSong
  Ceremony_NewPrimitives
  Ceremony_NewSlot
  Ceremony_NewEquipment
  Ceremony_NewEmotes
  Ceremony_NewClothing
  Ceremony_MissionStarted   >   Not Working
  Ceremony_LeagueWinner
  Ceremony_BountyClaimed
  Ceremony_Bounty
  Ceremony_BadShot
  Ceremony_Cash
  
  Contact_Up
	
 +  —  —  —  Category
	
  * Note: Use "https://apbdb.com" / "InventoryItemTypes.INT" / "Ellix Assets Rip" for references. thats my method.

  Weapon_*             >   Example  ` Weapon_Pistol_FBW `
  KillIcon_*           >   Example  ` KillIcon_Pistol_FBW ` `KillIcon_AssaultRifle_NTEC-5_Stock`
  Clothing_*           >   Example  ` Clothing_M_Hairwear_Hat_TopHatTall `
  Contact_*            >   Example  ` Contact_YoDawg `
  Vehicle_*            >   Example  ` Vehicle_PatriotVegasG20 `

  Icon_Achievement_*   >   Example  ` Icon_Achievement_KillStats_FromBehind ` / [https://apbdb.com/achievements]
		
  Icon_Achievement_Christmas_Frozen
  Icon_Achievement_Christmas_GunRunner
  Icon_Achievement_Christmas_SantaSlayer
  icon_achievement_gotnewstuff
		
/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /
```
