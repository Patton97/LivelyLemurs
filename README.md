# LivelyLemurs
SEP Project

Known Issues:

Standalone ranger generates an error message about textures | Solved on my end, will upload at some point

Ranger kicks back when firing | Pending fix

Ranger sometimes slides during firing animation | Pending fix

How to set this up on a fresh project:

1.Open Project settings

2.Go to Engine->Collision

3.Create New Object Channel, named Projectile and leave default response as block

4.Create new Preset, named Projectile, set CollisionEnabled to Query Only, set Object Type to Projectile, Leave all settings at block 

5.except for projectile which you should change to Ignore

6.Settings should look like this

![Settings](https://i.imgur.com/3K3p4un.jpg)

7.Close Project

8.Add Animation starter pack from Unreal asset store

9.Copy paste folders to Content -> TopDownBP

10. Pull desired STK_Char, RNG_Char and FLR_Char into map

Notes:

TopDownCharacter included uses an int variable "Health" for health and a CheckHP event is called when AI deal damage to it, has functionality to deal damage to nearby AI by pressing F, useful for testing

AI also use an int variable for health named "HP", an event "CheckAIHP" should be called whenever they are dealt damage

Follower runs up to player and tries to punch him, deals damage within 200 Units [May add directional component later]

Stalker runs to a distance away from the player and spawns a damaging circle when the player turns his back to it

Ranger also stays at a distance and fires shots between movements

Projectiles are medium sized and slow, allowing for many on screen to be dodged if necessary.

Material files are taken from the GamesTextures Material Pack from the Unreal asset store, they have been packaged with the AI and should work standalone.

Turret Added:

Turret uses starter content materials for head and base so make sure that's included, otherwise should work fine. Requires projectile from the ranger class and the aforementioned projectile Object Type and Preset in collision.
