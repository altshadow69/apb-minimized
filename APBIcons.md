 
## Guide

Icon images can be easily embedded within the localization file this guide shows you how to do it step by step.  

> [!NOTE]
> Text images, can not be overlaped or underlaped it will treat as a text.

Keep in mind that i create it this guide through trial and error.  
Freely contact me for suggestions or information.

## Extension APB_Images / Images

 `APB_Images:` Uses for a specific naming tag, such as `Icon_JokerTickets` for the HUDIcon. `Weapon_Pistol_FBW` for the HUDTexture.

 with in the usage of APB_Images `HUDIcon` is for "Generic_Icons_Master" Texture sheet only! can be seems [Here!](https://i.imgur.com/E506K3r.png)  

 and with in the usage of APB_Images `HUDTexture` specific name tag for the APB_Images Textures Images, for examples `Weapon_Pistol_FBW` `KillIcon_Pistol_FBW`  

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

---

 `Images:` Usage for a file path naming scheme with in UPK.file `APBMenus_Art_Achievements.AchievementComplete` example  
 And it is not required to be specific upper/lower casing, or needed for to enable a tag HUDTexture set to True.  
 If the path name includes with the group name, add group name in the middle of path file name `APBMenus_Art_Icons.Reward.Icon_Reward_Emote` example  
 
> [!IMPORTANT]
> `Images:` Only works in User Interface Element, and not HUD Message Element.

## Intimidation

| Command | Description |
| :--- | :--- |
| *HUDIcon* | |
| ```<APB_Images:APBCash;HUDIcon=TRUE>``` | if the HUDIcon text is in, User Interface Element. · _"APBUserInterface.INT"_ etc. |
| ```<hudicon:APBCash>``` | if the HUDIcon text is in, HUD Message Element. · _"HUDMessages.INT"_ |
| *HUDTexture* | |
| ```<APB_Images:Ceremony_Cash;HUDTexture=TRUE>``` | if the HUDTexture text is in, User Interface Element. · _"APBUserInterface.INT"_ etc. |
| ```<hudtexture:Ceremony_Cash>``` | if the HUDTexture text is in, HUD Message Element. · _"HUDMessages.INT"_ |
| *Images* | |
| ```<Images:APBMenus_Art_Achievements.AchievementComplete>``` | if the Image Texture text is in, User Interface Element. · _"APBUserInterface.INT"_ |
| ```<img:None>``` `unused` | code of it exist but with oddities, it uses the APB_Images template but the HUDIcon has been set to false, and it just simply print out the code line.  |

## Sizing

> [!IMPORTANT]
> Resizing the HUDTexture might work, but it will specifically bug out and revert to its original size.  
> Mixing hudicon with hudtexture will not prevent the bug related to the original size
> Only 'Images:' won't be affected by this bug.

 if you want to resize the Icon Image then use "XL=16 YL=16" and then add "Resize=TRUE" next to it

| Command | Description |
| :--- | :--- |
| *HUDIcon* | |
| ```<APB_Images:***;Resize=TRUE XL=16 YL=16 HUDIcon=TRUE>``` | Resizeing HUDIcon text in, User Interface Element.|
| ```<hudicon:***;Resize=TRUE XL=16 YL=16>``` | Resizeing HUDIcon text in, HUD Message Element.|  
| *HUDTexture* | |
| ```<APB_Images:***;Resize=TRUE XL=16 YL=16 HUDTexture=TRUE>``` | Resizeing HUDTexture In User Interface Element. |
| ```<hudtexture:***;Resize=TRUE XL=16 YL=16 HUDIcon=TRUE>``` | Make sure to add "HUDIcon=TRUE" to enable it |
| *Images* | |
| ```<Images:***;Resize=TRUE XL=16 YL=16>``` | Only have Resize set to True. |
| Unavailable! | |

## Coloring

> [!IMPORTANT]
> If `APB_Images` is applied, the game will automatically generate the white color from the first line of code following the `APB_Images` command. and cannot be overridden.  

> [!WARNING]
> Some UI Element like in, Shop UI / Mission Titles-Description UI, will render the color alpha has `A=0` and it will appear as nothing, to enable it just set the ImageColour as `<ImageColour:A=1>`  

> [!NOTE]
> ImageColour only works in User Interface Element, and Not the HUD Message Element.  

| Command | Description |
| :--- | :--- |
| *Images* | |
| ```<ImageColour:R=1 G=1 B=1 A=1><Images:***;Resize=TRUE XL=16 YL=16>``` | "<ImageColour:R=1 G=1 B=1 A=1>" |

---

## Listing [ HUDIcon / HUDTexture / Images ]

The naming must be specific. this listing is working progress

```
/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /

 •  —  —  —  —  —  —  —  —  —  Icons
	
  APBCash
  AmmoVending					   >   White Covered
  Contact
  DisplayPoint
  Elective_Corpse				   >   Reskin
  Elective_VehicleSpawn
  Faction_Criminal
  Faction_Enforcer
  GMPlayer						   >   RTW / Shows Nothing
  GroupLeader					   >   White Covered
  GroupPlayer
  Icon_JokerTickets
  InteractionPoint_Garage		   >   White Covered
  InteractionPoint_MusicStudio	   >   Not Working
  InteractionPoint_SymbolEditor	   >   White Covered
  InteractionPoint_Vault
  InteractionPoint_Wardrobe		   >   White Covered
  Mailbox
  MarketplaceZone				   >   White Covered
  MobileRadarTower
  None							   >   Shows Nothing
  OpenWorldDropOff_Small		   >   White Covered
  OppositionPlayer				   >   RTW / Shows Nothing
  PDA							   >   RTW / Shows Nothing
  PlayerVehicle
  PlayerVehicleWithTaskItem		   >   Reskin
  Rating
  SpawnZone
  SpawnZone_Criminal			   >   Reskin
  SpawnZone_Enforcer			   >   Reskin
  SpawnZone_Factionless			   >   Reskin
  StashDropOff					   >   White Covered
  Status_AFK
  Status_Arrested
  Status_Busy					   >   Not Working
  Status_Crown
  Status_DND
  Status_Dead
  Status_Disconnected			   >   Not Working
  Status_Driving
  Status_NonTaskParticipant
  Status_None
  Status_OutOfDistrict			   >   Not Working
  Status_Ready
  Status_Stunned
  Status_TaskParticipant   >   Shows Nothing ( Note: Probably its the weird thumbs up icon in the texture sheet, but never used. )
  Task_Checkpoint
  Task_Checkpoint_Occ
  Task_Item
  Task_Item_Occ					   >   Reskins
  Task_Item_Vehicle				   >   Reskins
  Task_Target
  Task_Target_Occ
  Task_Target_VIP 
  TestItem						   >   RTW / Reskin / White Covered
  VOIP_Active_High
  VOIP_Active_Low
  VOIP_Active_Medium
  VOIP_InChannel
  VOIP_Muted
  VOIP_NotInChannel
  VehicleRepair
  VehicleSpawn
  Waypoint
  Waypoint_Leader

 +  —  —  —  Taggers

  Spotter
  Tagger_Cat
  Tagger_Default
  Tagger_Duck
  Tagger_PurpleCat
  Tagger_Rapid99
  Tagger_Reaper
  Tagger_Sluttles
  Tagger_Suit_Clubs
  Tagger_Suit_Diamond
  Tagger_Suit_Hearts
  Tagger_Suit_Joker
  Tagger_Suit_Spades
  Tagger_Valentines

 +  —  —  —  Events

  Minigame_Epidemic_Barrel
  Minigame_Epidemic_BarrelStack
  Minigame_Epidemic_Hazmat
  Minigame_Epidemic_Necrocite
  Minigame_Epidemic_Undedox
  Minigame_Epidemic_Warehouse
  Minigame_Epidemic_Zombicine
  Minigame_GoldenWeapon_Easter_Protagonist
  Minigame_GoldenWeapon_Explosive
  Minigame_GunGame
  Minigame_GunGame_Joker
  Minigame_Infection_Headless
  Minigame_Infection_Pumpkin
  Minigame_Infection_Survivor
  Minigame_Mugging_Carrier
  Minigame_Mugging_Carrier_Easter
  Minigame_Mugging_Item
  Minigame_Mugging_Item_Egg
  Minigame_Mugging_NPC
  Minigame_Mugging_Protagonist
  Minigame_Mugging_Protagonist_Easter
  Minigame_SlayBells_FrozenBlock
  Minigame_SnowballFight
  Minigame_Survival_Bomb
  Minigame_Survival_Cash
  Minigame_Survival_Hazmat
  Minigame_Survival_WeaponLegendary
  Minigame_Survival_WeaponPrimary
  Minigame_Survival_WeaponSecondary
  Minigame_Survival_WeaponSecondaryUnlock

/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /

 •  —  —  —  —  —  —  —  —  —  Textures

  Ceremony_ArrestStreak
  Ceremony_BadShot
  Ceremony_Bounty
  Ceremony_BountyClaimed
  Ceremony_Cash
  Ceremony_GenericUnlock
  Ceremony_KillStreak
  Ceremony_LeagueWinner
  Ceremony_MissionStarted		   >   Not Working
  Ceremony_NewClothing
  Ceremony_NewEmotes
  Ceremony_NewEquipment
  Ceremony_NewPrimitives
  Ceremony_NewSlot
  Ceremony_NewSong
  Ceremony_NewSymbols
  Ceremony_NewThemesInstruments
  Ceremony_NewUpgrades
  Ceremony_NewVehiclesParts
  Ceremony_NewWeapons
  Ceremony_TutorialComplete
  Ceremony_WinStreak
  CharacterCreation
  Contact_Up
  Icon_GenericBundle_Crate
  Icon_GenericBundle_Sack
  Icon_Locker_Generic_Symbols
  Icon_Locker_Generic_Token
  Icon_Medal_Default
  Icon_Reward_Bio				   >   Not Working
  Icon_Reward_Emote
  Icon_Reward_Vinyl
  Icon_Scoreboard_Generic_Clan
  Icon_Scoreboard_Generic_Player
  Icon_Title_Destroy
  Icon_Title_Question
  Icon_Title_Rename
  Icon_Title_Symbol_Save

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
Images Here ( ONLY IN USER INTERFACE ELEMENT )
```
/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /

APBMenus_Art.GenericIcons.PlayPosition_Bar
APBMenus_Art.WindowComponents.APB_ListItem_CheckEnabled
APBMenus_Art.WindowComponents.List_Item_New_01
APBMenus_Art_Adam.icon_clock_32
APBMenus_Art_ChatInterface.Close_Tab_Icon
APBMenus_Art_ClothingCustomisation.SideArrowShow
APBMenus_Art_DistrictMap.Arrowhead
APBMenus_Art_DistrictMap.SliderMarker
APBMenus_Art_EquipmentIcons.Icon_Equipment_CrowBarLV0
APBMenus_Art_GameFlowScenes.worldselecticon
APBMenus_Art_InfoBrowser.Unlocked
APBMenus_Art_InfoBrowserIcons.Ammo_Terminal
APBMenus_Art_InfoBrowserIcons.Arson
APBMenus_Art_InfoBrowserIcons.Audio_Display_Point
APBMenus_Art_InfoBrowserIcons.Bomb
APBMenus_Art_InfoBrowserIcons.BombDefusal
APBMenus_Art_InfoBrowserIcons.Burglary
APBMenus_Art_InfoBrowserIcons.Designer_Terminal
APBMenus_Art_InfoBrowserIcons.Door
APBMenus_Art_InfoBrowserIcons.Enemy_Vehicle
APBMenus_Art_InfoBrowserIcons.Enforcer_Investigate
APBMenus_Art_InfoBrowserIcons.Fence
APBMenus_Art_InfoBrowserIcons.ForcedEntry
APBMenus_Art_InfoBrowserIcons.Friendly_Vehicle
APBMenus_Art_InfoBrowserIcons.Garage_Terminal
APBMenus_Art_InfoBrowserIcons.Graffiti_Display_Point
APBMenus_Art_InfoBrowserIcons.LCPedestrian
APBMenus_Art_InfoBrowserIcons.Mailbox
APBMenus_Art_InfoBrowserIcons.Marketplace_Terminal
APBMenus_Art_InfoBrowserIcons.Music_Studio_Terminal
APBMenus_Art_InfoBrowserIcons.Neutral_Vehicle
APBMenus_Art_InfoBrowserIcons.Persona_Terminal
APBMenus_Art_InfoBrowserIcons.Scan
APBMenus_Art_InfoBrowserIcons.Statue_Display_Point
APBMenus_Art_InfoBrowserIcons.Stolen_Vehicle
APBMenus_Art_InfoBrowserIcons.Valid_Ram-Raid_Garage_Door
APBMenus_Art_InfoBrowserIcons.Valid_Ram-Raid_Shopfront
APBMenus_Art_InfoBrowserIcons.Vehicle_Display_Point
APBMenus_Art_InfoBrowserIcons.Vehicle_Spawn_Terminal
APBMenus_Art_InfoBrowserIcons.Wardrobe_Terminal
APBMenus_Art_Jeshua.Slider_Arrow_Horizontal_Down_Active
APBMenus_Art_Jeshua.Slider_Arrow_Horizontal_Up_Active
APBMenus_Art_Jonathan.APB_Button_SortList_ArrowDown_3
APBMenus_Art_Jonathan.APB_Button_SortList_ArrowUp_3
APBMenus_Art_Mail.Reward_Package
APBMenus_Art_PopUpMenu.hUIButton_MenuButton
APBMenus_Art_Reticule.Speaker
APBMenus_Art_Social.District_Available
APBMenus_Art_Social.District_Full
APBMenus_Art_VendingIcons.icon_manufactured

/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /
```
Animated Material Images Here ( ONLY IN USER INTERFACE ELEMENT )
```
/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /

APBR_UI_HUD_Minigame.MAT_Halloween_Epidemic_Waiting
APBMenus_Art_GameFlowScenes.LoadingArrows
APBMenus__Art_CrimeEventAlert.MT_HUD_MissionStartedRays
APBMenus__Art_CrimeEventAlert.CEA_Reminder_Mat
APBMenus__Art_CrimeEventAlert.CEA_Main
APBMenus__Art_CrimeEventAlert.CEA_HUB
APBMenus__Art_CrimeEventAlert.CEA_BG_Red_Mat
APBMenus__Art_CrimeEventAlert.CEA_BG_03_Mat
APBMenus_Art.WindowComponents.GlossyBLink
Prestige_Attained_Material
Notoriety_Attained_Material

/ / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / / /
```
