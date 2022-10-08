# OptiFine 替代品

## 为什么需要替代 OptiFine？

OptiFine最初是一个伟大的MOD, 最开始时它为玩家提供了许多游戏的优化。然而，随着时间的推移，它带来的好处越来越少，并给MOD作者们带来了许多问题。这是因为Minecraft的代码库多年来一直在改进，而OptiFine时常替换掉整段Minecraft 的代码，同时又是闭源的，因此很难弄清楚为什么OptiFine会与另一个作者制作的MOD不兼容。
另外值得注意的是，OptiFine本身并不支持Fabric，而且OptiFabric是很难维护的。

在现在的Minecraft时代，在Fabric的社区努力下，MOD作者们已经开始为OptiFine的大部分功能创建替代品，让玩家保持更好的性能，更好的MOD兼容性，以及更好的支持。

[OptiFabric：一篇关于1.16崩溃的笔记(OptiFabric: A note about the 1.16 crashes)][optifabric_issue]

[optifabric_issue]: https://github.com/modmuss50/OptiFabric/issues/242

## This list

This list will list recommended OptiFine alternatives by me (LambdAurora), so it has some requirements for mods to be listed here:

 - They must be publicly available - if they're only available on request they are not eligible.
 - Mods must respect the Mojang EULA.
 - “PVP” clients (Badlion / Lunar / etc.) and cheat clients are not considered mods.
 - Mods must not refer to cheat clients.
 - Mods that change gameplay in a way (e.g. zoom) that have a way for servers to disable them will be favored.
 - Free and open-source mods are favored.

This list now has a fancy URL: https://lambdaurora.dev/optifine_alternatives

### Contribute

You can contribute to this list by opening a pull request on the `data` branch via [GitHub](https://github.com/LambdAurora/optifine_alternatives).

## Alternatives

### Performance

#### Client

- [Cull Leaves] - Adds culling to leaf blocks, providing a huge performance boost over vanilla. Similar to OptiFine's Smart Leaves feature.  
  - Available for: quilt: 1.17 -> 1.19, fabric: 1.16 -> 1.19  
- [Cull Particles] - Don't render particles that can't be seen. Unneeded with Sodium.  
  - Available for: fabric,quilt: 1.15 -> 1.19  
- [Dynamic FPS] - Improve performance when Minecraft is in the background.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.14 -> 1.19  
- [Enhanced Block Entities] - Reduce FPS lag with block entities, as well as customize them with resource packs.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.19  
- [EntityCulling] - Using async path-tracing to hide (Block-)Entities that are not visible.  
  - Available for: fabric,quilt: 1.16 -> 1.19, forge: 1.8.9, forge: 1.16 -> 1.19  
- [Sodium] - Modern rendering engine and client-side optimization mod for Minecraft.  
  - Available for: fabric,quilt: 1.16 -> 1.19  

#### General

- [LazyDFU] - Makes the initialization of DataFixerUpper "lazy". DataFixerUpper (or DFU for short) is the system used by Minecraft to convert old worlds to the current version you're running, in Vanilla it's initialized at startup and is slow (and eats a lot of resources). This mod delays the initialization of DFU by initializing only when needed, if you're playing only on multiplayer it'll never get initialized for example.  
  - Available for: fabric,quilt: 1.14 -> 1.19, forge: 1.16 -> 1.19  
- [Lithium] - No-compromises game logic/server optimization mod.  
  - Available for: fabric,quilt: 1.15 -> 1.19  
- [Phosphor] - No-compromises lighting engine optimization mod. Incompatible with Starlight.  
  - Available for: fabric,quilt: 1.15 -> 1.19  
- [Starlight] - Rewrites the light engine to fix lighting performance and lighting errors. Uses a custom format for light storage. Incompatible with Phosphor.  
  - Available for: fabric,quilt,forge: 1.17 -> 1.19  

### Cosmetic

- [Animatica] - A mod implementing the OptiFine/MCPatcher animated texture format.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.17 -> 1.19  
- [Chime] - Adds predicates for more interactive item models, CIT replacement with a custom format.  
  - Available for: fabric: 1.16, fabric,quilt: 1.18 -> 1.19  
- [CIT Resewn] - Re-implements MCPatcher's CIT (custom item textures from optifine resource packs)  
  - Available for: fabric,quilt: 1.17 -> 1.19  
- [Clear Skies] - Horizon and fog match the sky color. True blue skies!  
  - Available for: fabric,quilt: 1.15 -> 1.19, forge: 1.16  
- [Colormatic] - An independent implementation of the custom colors mod for Minecraft.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.14 -> 1.19  
- [Connected Block Textures] - An implementation of the MCPatcher/Optifine connected textures format on the Fabric modloader. Unmaintained.  
  - Available for: fabric: 1.16  
  - Requires [Fabric Renderer API](#compatibility "More information.")  
- [Continuity] - A Fabric mod that allows for efficient connected textures. Support emissive textures.  
  - Available for: fabric,quilt: 1.17 -> 1.19  
  - Requires [Fabric Renderer API](#compatibility "More information.")  
- [Custom Entity Models (CEM)] - An implementation of custom entity models heavily based off of Optifine's format that aims to achieve feature parity with Optifine's custom entity models.  
  - Available for: fabric,quilt: 1.16 -> 1.19  
- [Custom GUI] - A mod allowing to animate GUI textures or replace container textures with minimal predicates.  
  - Available for: fabric: 1.16 -> 1.17  
- [Entity Texture Features] - A Fabric mod implementing randomized & emissive texture support for mobs set by the resourcepack. Fully compatible with the Optifine format & Sodium.  
  - Available for: quilt: 1.18 -> 1.19, fabric,forge: 1.16 -> 1.19  
- [FabricSkyboxes] - Allows resource packs to define custom skyboxes. OptiFine format is not compatible by default, converters are available.  
  - Available for: fabric,quilt: 1.16 -> 1.19  
- [JMX] - JMX adds support for FREX Rendering API features to Minecraft JSON model loading. It can also be configured to load all JSON models as FREX meshes, which may offer a modest reduction in memory usage due to more efficient data structures.  
  - Available for: fabric,quilt: 1.16 -> 1.19  
- [JsonEM (Json Entity Models)] - Data driven entity model library, should work with most entities. Does not support OptiFine's format.  
  - Available for: quilt,fabric: 1.18 -> 1.19  
- [LambdaBetterGrass] - Adds better grass and snow to the game.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.19  
  - Requires [Fabric Renderer API](#compatibility "More information.")  
- [LambDynamicLights] - Adds dynamic lighting to the game.  
  - Available for: quilt: 1.17 -> 1.19, fabric: 1.15 -> 1.19  
- [More Block Predicates] - Allows resource packs to change block models depending on new conditions! Custom format.  
  - Available for: fabric,quilt: 1.17 -> 1.19  
- [MoreMcmeta] - Animate almost any Minecraft texture with more options.  
  - Available for: fabric,quilt: 1.16 -> 1.19, forge: 1.16 -> 1.19  
- [Transparent] - Allows resource packs to make entities support transparency.  
  - Available for: fabric,quilt,forge: 1.15 -> 1.19  
- [Varied Mob Textures] - This mod allows the resource packs creator to have multiple randomized textures for the same mob. Uses custom format, OptiFine-based resource packs will need conversion.  
  - Available for: fabric: 1.16  

#### Splash Screen

- [Custom Splash Screen] - Change Minecraft's loading screen to your liking! Completely configurable!  
  - Available for: quilt: 1.18, fabric: 1.16 -> 1.18  
- [Dark Loading Screen] - A simple mod to make the loading screen darker.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.15 -> 1.19  
- [Quilt Loading Screen] - A loading screen based off of The Quilt Community's server banner.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.18  
- [Splash] - Splash is a Fabric mod that allows you to customize the colors of your splash screen.  
  - Available for: fabric: 1.16 -> 1.17  

### Shaders

- [Canvas Renderer] - A new rendering engine. Incompatible with Sodium.  
  - Available for: fabric,quilt: 1.17 -> 1.19, fabric: 1.16  
- [Iris] - A new shaders mod for Minecraft intended to be compatible with existing ShadersMod/Optifine shaders.  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.16 -> 1.19  

### Fog

- [ClearView] - Controls which kinds of fogs are shown.  
  - Available for: fabric: 1.15 -> 1.16  
- [Custom Fog] - A mod allowing you to customize the appearance of fog in your world.  
  - Available for: fabric,quilt: 1.15 -> 1.18  
- [Fog Control] - Allows the user to adjust the (client) distance at which fogs render or disable them completely.   
  - Available for: fabric: 1.17  
- [FogYeet] - Small mod for 1.15 to remove fog.  
  - Available for: fabric: 1.15  
- [NoFog] - A simple client-side mod supporting both forge and fabric that removes all fog. (ARR)  
  - Available for: fabric,quilt: 1.16 -> 1.19, forge: 1.10.2 -> 1.19  

### Utility

- [Fabrishot] - Take insanely large screenshots because why not?  
  - Available for: fabric,quilt: 1.16 -> 1.19  
- [Resolution Control] - Allows you to set render resolutions and take large screenshots.  
  - Available for: fabric: 1.14 -> 1.16  
- [ResolutionControl+] - Allows you to set render resolutions and take large screenshots.  
  - Available for: fabric: 1.16 -> 1.17, fabric: 1.19  

#### Cloud Height

- [Raised Clouds] - Allows changing the height at which clouds appear.  
  - Available for: fabric,quilt: 1.16 -> 1.19  
- [Soaring Clouds] - Allows changing the height at which clouds appear.  
  - Available for: fabric: 1.15 -> 1.16  

#### Zoom

- [Camera Utils] - Additional features concerning the player's camera.  
  - Available for: fabric,quilt: 1.17 -> 1.19  
- [Logical Zoom] - Super simple zoom key for Minecraft.  
  - Available for: fabric,quilt: 1.15 -> 1.19  
- [Ok Zoomer] - Adds a highly-configurable zoom key for Fabric. The zoom is yours!  
  - Available for: quilt: 1.18 -> 1.19, fabric: 1.14 -> 1.18  
- [Quick Spyglasser] - Adds a client-side keybind for using a spyglass anywhere in your inventory.  
  - Available for: fabric: 1.17  
- [Zoomify] - A rather simple zoom mod with moderate customizability.  
  - Available for: fabric,quilt: 1.18 -> 1.19  

[Cull Leaves]: https://modrinth.com/mod/cull-leaves "Cull Leaves Modrinth page"
[Cull Particles]: https://curseforge.com/minecraft/mc-mods/cull-particles-fabric "Cull Particles CurseForge page"
[Dynamic FPS]: https://modrinth.com/mod/dynamic-fps "Dynamic FPS Modrinth page"
[Enhanced Block Entities]: https://modrinth.com/mod/ebe "Enhanced Block Entities Modrinth page"
[EntityCulling]: https://modrinth.com/mod/entityculling "EntityCulling Modrinth page"
[Sodium]: https://modrinth.com/mod/sodium "Sodium Modrinth page"
[LazyDFU]: https://modrinth.com/mod/lazydfu "LazyDFU Modrinth page"
[Lithium]: https://modrinth.com/mod/lithium "Lithium Modrinth page"
[Phosphor]: https://modrinth.com/mod/phosphor "Phosphor Modrinth page"
[Starlight]: https://modrinth.com/mod/starlight "Starlight Modrinth page"
[Animatica]: https://modrinth.com/mod/animatica "Animatica Modrinth page"
[Chime]: https://modrinth.com/mod/chime "Chime Modrinth page"
[CIT Resewn]: https://modrinth.com/mod/cit-resewn "CIT Resewn Modrinth page"
[Clear Skies]: https://modrinth.com/mod/clear-skies "Clear Skies Modrinth page"
[Colormatic]: https://modrinth.com/mod/colormatic "Colormatic Modrinth page"
[Connected Block Textures]: https://github.com/TwilightFlower/connected-block-textures "Connected Block Textures GitHub page"
[Continuity]: https://modrinth.com/mod/continuity "Continuity Modrinth page"
[Custom Entity Models (CEM)]: https://modrinth.com/mod/cem "Custom Entity Models (CEM) Modrinth page"
[Custom GUI]: https://modrinth.com/mod/customgui "Custom GUI Modrinth page"
[Entity Texture Features]: https://modrinth.com/mod/entitytexturefeatures "Entity Texture Features Modrinth page"
[FabricSkyboxes]: https://modrinth.com/mod/fabricskyboxes "FabricSkyboxes Modrinth page"
[JMX]: https://modrinth.com/mod/imx "JMX Modrinth page"
[JsonEM (Json Entity Models)]: https://modrinth.com/mod/jsonem "JsonEM (Json Entity Models) Modrinth page"
[LambdaBetterGrass]: https://modrinth.com/mod/lambdabettergrass "LambdaBetterGrass Modrinth page"
[LambDynamicLights]: https://modrinth.com/mod/lambdynamiclights "LambDynamicLights Modrinth page"
[More Block Predicates]: https://modrinth.com/mod/mbp "More Block Predicates Modrinth page"
[MoreMcmeta]: https://modrinth.com/mod/moremcmeta "MoreMcmeta Modrinth page"
[Transparent]: https://modrinth.com/mod/transparent "Transparent Modrinth page"
[Varied Mob Textures]: https://curseforge.com/minecraft/mc-mods/varied-mob-textures "Varied Mob Textures CurseForge page"
[Custom Splash Screen]: https://modrinth.com/mod/custom-splash-screen "Custom Splash Screen Modrinth page"
[Dark Loading Screen]: https://curseforge.com/minecraft/mc-mods/dark-loading-screen "Dark Loading Screen CurseForge page"
[Quilt Loading Screen]: https://modrinth.com/mod/quilt-loading-screen "Quilt Loading Screen Modrinth page"
[Splash]: https://curseforge.com/minecraft/mc-mods/splash "Splash CurseForge page"
[Canvas Renderer]: https://modrinth.com/mod/canvas "Canvas Renderer Modrinth page"
[Iris]: https://modrinth.com/mod/iris "Iris Modrinth page"
[ClearView]: https://curseforge.com/minecraft/mc-mods/clearview "ClearView CurseForge page"
[Custom Fog]: https://modrinth.com/mod/custom-fog "Custom Fog Modrinth page"
[Fog Control]: https://modrinth.com/mod/fog-control "Fog Control Modrinth page"
[FogYeet]: https://modrinth.com/mod/fogyeet "FogYeet Modrinth page"
[NoFog]: https://modrinth.com/mod/no_fog "NoFog Modrinth page"
[Fabrishot]: https://modrinth.com/mod/fabrishot "Fabrishot Modrinth page"
[Resolution Control]: https://curseforge.com/minecraft/mc-mods/resolution-control "Resolution Control CurseForge page"
[ResolutionControl+]: https://modrinth.com/mod/resolution-control-plus "ResolutionControl+ Modrinth page"
[Raised Clouds]: https://curseforge.com/minecraft/mc-mods/raised-clouds "Raised Clouds CurseForge page"
[Soaring Clouds]: https://curseforge.com/minecraft/mc-mods/soaring-clouds "Soaring Clouds CurseForge page"
[Camera Utils]: https://modrinth.com/mod/camera-utils "Camera Utils Modrinth page"
[Logical Zoom]: https://modrinth.com/mod/logical-zoom "Logical Zoom Modrinth page"
[Ok Zoomer]: https://modrinth.com/mod/ok-zoomer "Ok Zoomer Modrinth page"
[Quick Spyglasser]: https://curseforge.com/minecraft/mc-mods/quick-spyglasser "Quick Spyglasser CurseForge page"
[Zoomify]: https://modrinth.com/mod/zoomify "Zoomify Modrinth page"


### Extras

The mods listed below are not part of the OptiFine alternatives directly but those are still nice to have.

- [Ears] - Faithful fancy fashion features for fuzzy folk. It offers a lot of skin customization options, directly encoded into the skin file uploaded to Mojang. A very good alternative to express yourself than restrictive capes.
  - Available for: b1.7.3, 1.2.5, 1.4.7 -> 1.19, Not so Seecret Saturday (a1.1.2), New Frontier Craft (b1.7.3)
- [DashLoader] - Attempts to improve loading times by caching the game's content. May be incompatible with some of the mods in this list.
  - Available for: 1.16 -> 1.19
- [Entity View Distance] - This mods allows more precise manipulation of entity view distance on client and server 
  - Available for: 1.17 -> 1.19
- [FerriteCore] - Memory usage optimizations.
  - Available for: [1.16 -> 1.19][FerriteCore], [1.16 -> 1.19 (Forge)](https://www.curseforge.com/minecraft/mc-mods/ferritecore)
- [Hydrogen] - Reduces the memory usage of the game in more modded scenarios.
  - Available for: 1.16 -> 1.17
- [Krypton] - A mod to optimize the Minecraft networking stack
  - Available for: 1.16 -> 1.19
- [Overworld Two] provides an alternative optimized world generator for overworld and nether. Much faster than Vanilla but isn't identical to Vanilla.
  - Available for: 1.16
- [Sodium Extra] - Adds features that should not be in Sodium.
  - Available for: 1.16 -> 1.19
- [Reese's Sodium Options] - Alternative Options Menu for Sodium with intention of improving UX.
  - Available for: 1.16 -> 1.19

[Ears]: https://ears.unascribed.com/ "Ears Website"
[FerriteCore]: https://modrinth.com/mod/ferrite-core "FerriteCore Modrinth page"
[Entity View Distance]: https://modrinth.com/mod/entity-view-distance "Entity View Distance Curseforge page"
[Hydrogen]: https://modrinth.com/mod/hydrogen "Hydrogen Modrinth page"
[Krypton]: https://modrinth.com/mod/krypton "Krypton Modrinth page"
[DashLoader]: https://modrinth.com/mod/dashloader "DashLoader Modrinth page"
[Overworld Two]: https://www.curseforge.com/minecraft/mc-mods/overworld-two "Overworld Two Curseforge Page"
[Sodium Extra]: https://modrinth.com/mod/sodium-extra "Sodium Extra Modrinth page"
[Reese's Sodium Options]: https://modrinth.com/mod/reeses-sodium-options "Reese's Sodium Options Modrinth page"

### No Dynamic FOV

**As of 1.16.2 and above, this is now a vanilla feature under the accessibility settings. If you are playing in 1.16.2 or above, the mods for this feature are irrelevant.**

These are client-only mods that prevent Minecraft from changing the FOV in all situations.

- [motioNO] - disables dynamic FOV.
- [FovLock] - adds dynamic FOV lock button.

[motioNO]: https://www.curseforge.com/minecraft/mc-mods/motiono "MotioNo CurseForge page"
[FovLock]: https://github.com/ChloeDawn/FovLock "FovLock GitHub page"

## Compatibility

Sodium and Canvas Renderer are incompatible.

Some mods require the Fabric Renderer API to work, Canvas supports it, but Sodium will not support it by default, [Indium] is required to support it.

- [Indium] - Adds support of the Fabric Renderer API to [Sodium](https://modrinth.com/mod/sodium).
  - Available for: 1.16 -> 1.19

[Indium]: https://modrinth.com/mod/indium "Indium Modrinth Page"

## Missing

- Custom entity models (might come in Vanilla to an unknown date?)
  currently incompletely replaced: current existing implementations are very hardcoded to Vanilla entities

## Need help?

If you need help about Sodium, Lithium, Phosphor (any of CaffeineMC's mod to be short), [please check out CaffeineMC's discord server](https://jellysquid.me/discord).

If you need help related to LambDynamicLights, LambdaBetterGrass, or Inspecio, if you don't want to post in the comments a suggestion you can check out [my own discord server](https://discord.lambdaurora.dev)

## Other lists

 - [Useful Fabric server-side mods](https://github.com/comp500/fabric-serverside-mods/blob/main/README.md)
