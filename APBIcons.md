Images Icons can be embed 

## Extension between HUDIcon / HUDTexture

"HUDIcon" Usage for "Generic_Icons_Master" Texture Sheet can be seems [Here!](https://i.imgur.com/E506K3r.png) and others stuffs as Labeled as Icon could work

"HUDTexture" Usage for the In Game Hud Textures Images, For Example\
`Icon_Locker_Generic_Token` `Vehicle_PatriotVegasG20` `Weapon_Pistol_FBW` / `KillIcon_Pistol_FBW`

## HUDIcon

if the HUDIcon text is in, **User Interface Element.** / _"APBUserInterface.INT"_ etc.\
`<APB_Images:APBCash;HUDIcon=TRUE>`

if the HUDIcon text is in, **HUD Message Element.** / _"HUDMessages.INT"_\
`<hudicon:APBCash>`

## HUDTexture

if the HUDTexture text is in, **User Interface Element.**\
`<APB_Images:Icon_Locker_Generic_Token;HUDTexture=TRUE>`

if the HUDTexture text is in, **HUD Message Element.**\
`<hudtexture:Icon_Locker_Generic_Token>`

## Resizing HUDIcon

if you want to resize the Icon Image\
then use "XL=16 YL=16" and then add "Resize=TRUE" next to it\
`<APB_Images:APBCash;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>`

it can also works in the **HUD Message Element.**\
`<hudicon:APBCash;XL=16 YL=16 Resize=TRUE>`

## Resizing HUDTexture

Resize HUDTexture In **User Interface Element.**\
`<APB_Images:Icon_Locker_Generic_Token;XL=16 YL=16 Resize=TRUE HUDTexture=TRUE>`

Resize HUDTexture In The **HUD Message Element.** <br/>then add "HUDIcon=TRUE"\
`<hudtexture:Icon_Locker_Generic_Token;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>`

> [!IMPORTANT]
> Resize for the HUDTexture can also work But it will randomly bug out to a original size. to prevent it,\
> Add `<Color:R=1 G=1 B=1>*then some text*` to stop resizing to original size. it will kinda works if you know what your doing
\

## Icons Listing WIP

```

	--- Icons

	APBCash
	Icon_JokerTickets
	Rating

	Contact
	Task_Checkpoint
	Task_Checkpoint_Occ
	Task_Target
	Task_Target_Occ
	Task_Item
	Task_Item_Occ;
	Task_Target_VIP 

	SpawnZone
	Mailbox
	PlayerVehicle
	VehicleSpawn
	VehicleRepair
	Elective_Corpse
	Waypoint_Leader
	DisplayPoint
	MobileRadarTower
	AmmoVending
	MarketplaceZone
	InteractionPoint_SymbolEditor
	InteractionPoint_Wardrobe
	InteractionPoint_Garage

	Faction_Criminal
	Faction_Enforcer

	::: Reskins Heres

	GroupPlayer
	PlayerVehicleWithTaskItem
	Task_Item_Vehicle
	StashDropOff
	OpenWorldDropOff_Small

	OppositionPlayer ::: Shows Nothing?
	PDA

	--- Taggers

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

	---  Events

	Minigame_Survival_Cash
	Minigame_GunGame_Joker
	Minigame_GunGame
	Minigame_SlayBells_FrozenBlock

	Minigame_Survival_WeaponSecondaryUnlock
	Minigame_Survival_WeaponLegendary
	Minigame_Survival_Bomb
	Minigame_Survival_Hazmat

	:::  Textures stuff

	Icon_Locker_Generic_Token

		Look up into "apbdb.com" "InventoryItemTypes.INT" or "Ellix Images Assets Rip" for references. thats my method.
		
		Vehicle_*
		Weapon_*
		KillIcon_*



```
