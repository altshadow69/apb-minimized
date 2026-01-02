## Extension between HUDIcon / HUDTexture

"HUDIcon" Usage for the In "Generic_Icons_Master" can be seems [Here!](https://i.imgur.com/E506K3r.png) and others stuffs as Labeled as Icon could work

"HUDTexture" Usage for the In Game Hud Textures Images, For Example\
`Icon_Locker_Generic_Token` `Vehicle_PatriotVegasG20` `Weapon_Pistol_FBW` / `KillIcon_Pistol_FBW`

## HUDIcon

if the HUDIcon text is in, User Interface Element. / "APBUserInterface.GER" etc.\
then use `<APB_Images:APBCash;HUDIcon=TRUE>`

if the HUDIcon text is in, Hud Message Element. / "HUDMessages.GER"\
then use `<hudicon:APBCash>`

## HUDTexture

if the HUDTexture text is in, User Interface Element.\
then use `<APB_Images:Icon_Locker_Generic_Token;HUDTexture=TRUE>`

if the HUDTexture text is in, Hud Message Element.\
then use `<hudtexture:Icon_Locker_Generic_Token>`

## Resizing HUDIcon

if you want to resize the Icon Image\
then use "XL=16 YL=16" and then add "Resize=TRUE" next to it\
`<APB_Images:APBCash;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>`

it can also works in the Hud Message Element.\
`<hudicon:APBCash;XL=16 YL=16 Resize=TRUE>`

## Resizing HUDTexture

Resize HUDTexture In User Interface Element.\
then use\
`<APB_Images:Icon_Locker_Generic_Token;XL=16 YL=16 Resize=TRUE HUDTexture=TRUE>`

Resize HUDTexture In The Hud Message Element. <br/>then add "HUDIcon=TRUE"\
`<hudtexture:Icon_Locker_Generic_Token;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>`

> [!IMPORTANT]
> Resize for the HUDTexture can also work But it will randomly bug out to a original size. to prevent it,\
> Add ``<Color:R=1 G=1 B=1>*then some text*`` to stop resizing to original size. it will kinda works if you know what your doing (In User Interface Element)

# Icons Listing WIP

```
---  Icons

<APB_Images:APBCash;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Icon_JokerTickets;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Rating;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

<APB_Images:Contact;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Checkpoint;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Checkpoint_Occ;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Target;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Target_Occ;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Item;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Item_Occ;;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Target_VIP;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE> 

<APB_Images:SpawnZone;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Mailbox;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:PlayerVehicle;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:VehicleSpawn;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:VehicleRepair;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Elective_Corpse;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Waypoint_Leader;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:DisplayPoint;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:MobileRadarTower;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:AmmoVending;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:MarketplaceZone;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:InteractionPoint_SymbolEditor;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:InteractionPoint_Wardrobe;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:InteractionPoint_Garage;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

<APB_Images:OppositionPlayer;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE> : Shows Nothing?

<APB_Images:Faction_Criminal;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Faction_Enforcer;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

::: Reskins Heres

<APB_Images:GroupPlayer;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:PlayerVehicleWithTaskItem;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Task_Item_Vehicle;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:StashDropOff;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:OpenWorldDropOff_Small;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

<APB_Images:PDA;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

---  Taggers
 
<APB_Images:Spotter;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
 
<APB_Images:Tagger_Default;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Duck;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Valentines;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

<APB_Images:Tagger_Suit_Clubs;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Suit_Diamond;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Suit_Hearts;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Suit_Spades;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Suit_Joker;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

<APB_Images:Tagger_PurpleCat;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Cat;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Rapid99;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Sluttles;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Tagger_Reaper;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

---  Events

<APB_Images:Minigame_Survival_Cash;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Minigame_GunGame_Joker;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Minigame_GunGame;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Minigame_SlayBells_FrozenBlock;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

<APB_Images:Minigame_Survival_WeaponSecondaryUnlock
<APB_Images:Minigame_Survival_WeaponLegendary;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Minigame_Survival_Bomb;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>
<APB_Images:Minigame_Survival_Hazmat;XL=16 YL=16 Resize=TRUE HUDIcon=TRUE>

:::  Others stuff

<APB_Images:Icon_Locker_Generic_Token;XL=16 YL=16 Resize=TRUE HUDTexture=TRUE> 
```
