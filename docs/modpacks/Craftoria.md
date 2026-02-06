# Craftoria
![Craftoria Cover](img/Craftoria start.png)

<div class="grid cards" markdown>
- :material-format-list-group: __Mod List__ [Craftoria MODLIST.md](https://github.com/TeamAOF/Craftoria7/blob/main/MODLIST.md)
- :simple-curseforge: __CurseForge__ [Craftoria](https://www.curseforge.com/minecraft/modpacks/craftoria)
- :fontawesome-brands-discord: __Discord Channel__ [\#craftoria](https://discord.com/channels/570630340075454474/1252708934729470094)
- :fontawesome-brands-github: __GitHub__ [Craftoria on GitHub](https://github.com/TeamAOF/Craftoria)
</div>

## Hype

### Let's Play Series

<center markdown>
=== "[ChosenArchitect](https://www.youtube.com/@ChosenArchitect)"
    <iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?si=FSk4Ks-IF2U2PU5-&amp;list=PL_ipI8CnaNIa5vyojV7RdUVrp7QETcvMx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

=== "[Jangro](https://www.youtube.com/@jangrogames)"
    <iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?si=PaDnrqa8badVmois&amp;list=PLONH6gx1GJLm5SDuuQlaK3wQi4Yc6BmJc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

=== "[Keno](https://www.youtube.com/@KenoGarage)"
    <iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?si=1yMcmQQtGDWYdjTn&amp;list=PLUsekSl0l8yyY98CAACrRjItnzC3fH6Gx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

=== "[Kmbles](https://www.youtube.com/@kmbles)"
    <iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?si=qyX0REsoTIV9njvA&amp;list=PLf-9vmpCe61pConmM7Qla18UIck-avHkV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</center>

## Craftoria FAQ

### Setup / Performance

* Use Java 21
* ~8GB RAM (too much invites longer GC pauses)
* Try these args: `-XX:+UseZGC -XX:+ZGenerational`

### Pack Content
Mods, so many mods!
Quests!
Dimensions!

#### Major Dimensions

1. Vanilla: Overworld, Nether, and The End
2. The Bumblezone
3. Eternal Starlight
4. Deeper & Darker: The Otherside
5. Twilight Forest

#### Utility Dimensions

1. Void (@JAVD)
2. Compact Machines
3. Mining dims matching the vanilla ones (@JAMD)
4. Spatial Storage (AE2)

### Other FAQ

#### Team chat
Team chat is bound to `u` by default. (`y` in earlier versions). If no one can see your messages, you may have this toggled on.

#### JDT Upgrades
Use a smithing table to apply them.

#### JDT Paxels
Assemble a JDT pickaxe, axe, and shovel in a smithing table.
!!! success "Fixed: EMI properly displays the JDT paxel recipe in recent pack versions."

#### Obtaining Hazen Items
Most of the items are craftable, but there's a list of ones that are not:

* Arbitrium Armor (Creative only)
* Excalibur Fragment (Obtained by Killing the Dead King)
* Fireblossom (Found in Crimson Forests in the Nether)
* Rod Of Discord & Starfury (Rare drop from Endermen)
* Overgrown/Charred bones (Dropped from Bogged and Wither Skeletons respectively)

#### World Tiers
The *Apotheosis* mod has a mechanic called "World Tiers."

* Use the default keybind (++"Ctrl"++ + ++"T"++) to see the display of world tiers and what each entails.
* Check the advancement tab (default: ++"L"++) labeled *Apothic World Tiers* to see how to unlock the next world tier.

Each world tier unlocks the spawning of higher level mob bosses and the chance to obtain better apothic gear traits.

#### Replicator Black-lists
To find the items in the blacklist for both the Replicator Mk1 and the Replicator Mk2, search the following for the two blacklists in EMI respectively:

* `#replicator_1_blacklist` for Replicator Mk1
* `#replicator_blacklist` for Replicator Mk2

### Whitelisting on our Official Servers

1. Read the [#whitelisting](https://discord.com/channels/570630340075454474/726536593136943204) channel on our discord, in it's entirety.

    By whitelisting yourself to one of our servers, you agree to the rules.

2. Head over to one of the server channels.
    * [#craftoria-eu](https://discord.com/channels/570630340075454474/1254490870808318087)
    * [#craftoria-eu2](https://discord.com/channels/570630340075454474/1292199371848552548)
    * [#craftoria-na](https://discord.com/channels/570630340075454474/1282263854922862632)

3. Use the command `/verify` followed by the code you obtain when first attempting to join the server.

!!! question "`/verify`-ed yourself, but still can't get in?"
    1. Use the command `/unverify`, then retry the verification steps.
    2. If Discord is not recognizing your `/verify` command, try **disabling** this setting in Discord:
        - `Settings` -> `Accessability` -> **`Use the legacy chat input.`**

### Installing a Server

See [Your Own Server](../servers/server.md)

### Need further help?

1. Open a post in our discord forum, [#support](https://discord.com/channels/570630340075454474/1028818900768538695).
2. If you have one, include a crash-report, crash file, or latest log.
3. Knowledgable players are very welcome to answer questions there too!

### Found a Bug?

* Please let us know, with a post in our discord forum, [#bug-reports](https://discord.com/channels/570630340075454474/1028644155305496576)
* Github repo issues are also welcomed.

### Addendum: Permissions

* `ftbchunks.max_claimed` (chunk claim quota)
* `command.back` (to enable or disable `/back`)
* `ftbessentials.back.cooldown`
* `ftbessentials.rtp.cooldown`
* `ftbessentials.home.max`

To alter, use:

* `/ftbranks node add [rank] [permission] [value(s)]`
* `/ftbranks node remove [rank] [permission]`

## Behind the Scenes Bonus!

### At Work: Facu

![Facu at Work: *Craftoria's* cover art](img/Craftoria art progression.gif){align=center}

---
