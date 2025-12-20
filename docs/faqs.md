# Frequently Asked Questions
_Just the FAQs, ma'am. Just the FAQs._

<div class="grid cards" markdown>
!!! info "Pack Specific?"
    See the **Modpack** pages for FAQ, Guides, and Tips

!!! info "Mod Specific?"
    See the **Select Mods** pages for FAQ, Guides, and Tips
</div>

??? danger "`craftoria.net` is BOGUS"
    That site is **not** owned or run by us and we do not affiliate with it. It was created by an unknown entity without permission and contains a _lot_ of false information about [_**Craftoria**_](modpacks/Craftoria.md).

## General FAQ

??? success "Credit and thanks to Inno..."
    ...for writing and maintaining a long, informative, quality FAQ before this wiki came along and absorbed it.

### Connection lost when joining a server? Something about "channels" and "missing mods"?
Normally, when you get this message, you should see two boxes of orange text. One talks about the "Channel Name" and the other a "Reason." For 99.9% of cases, this purely means that the version of the modpack you are on does _not_ align with the version of the modpack the server is running.

- For the public servers, the version says on the server's MOTD (the message on the server, in the multiplayer list). It also states it in the channel topic for the specific server.
- For other servers ensure that you are on the right version and that the server host has not modified the pack in any meaningful way.
- For your own self-hosted server, ensure that you are on a matching version. If that is checked, a possibility could be a failed server install. Sometimes Windows Firewall/Defender can deny downloads with seemingly no reason. Ensure your firewall/defender is not blocking some of these downloads.

### Modded Server lagging?
Your ping may be fine. Your computer may be fine as well. But that doesn't necessary mean the server _isn't_ fine. You must remember that Minecraft isn't exactly optimized with heavy modification in mind, especially when it comes to hosting a modified version of Minecraft to many people.
A lower TPS (Ticks Per Second) is very common. 20 TPS is the most fluid a server can be, but you will rarely see that, especially if a server has a lot going on in the world.
From someone who has played on modded servers with TPS dipping into, and below, 5 TPS: It takes some getting used to, but it's definitely playable.

Although, sometimes, it stays _very_ low for little apparent reason, such as low (or one) player count(s), newer server, etc. This could be a bug, but most of the time, it isn't.

### Want to force load chunks?
There's really only two ways to do it. Either use a vanilla chunk loader (yes it exists, look it up) or use FTBChunks!

- For FTBChunks, open your inventory and locate the map looking button with a beige border in the top left corner of your screen labeled "FTB Chunks: Claim Manager" and click on it.
- To claim a chunk, **Right-Click** or **Right-Click + Hold-Down** on the chunk(s) you wish to claim. You must claim before you can force load. Do the same with the **Left-Click** to un-claim.
- To force load a chunk, **Shift + Right-Click** or **Shift + Right-Click + Hold-Down** on the _claimed_ chunk(s) you wish to force load. Do the same with **Left-Click** to un-force load.
- Keep in mind the number of claimed chunks and force load chunks are limited and display at the bottom of your chunk manager screen.

### Have _power_ on a server and want to adjust values such as max claim/force-load chunks, homes, and more?
You'll need to use the power of commands for this one.
#### For Chunk related things, use the following command and node permissions:
`/ftbranks node add member <node> <value>`

- `ftbchunks.max_claimed` This uses an integer for `<value>`
- `ftbchunks.max_force_loaded` This uses an integer for `<value>`
- `ftbchunks.chunk_load_offline` This uses a boolean (`true` or `false`) for `<value>` **This permission is highly recommended you remain false to prevent excessive lag.**

#### For Home and Teleportation related things, use the following command and node permissions:
`/ftbranks node add member <node> <value>`

- `ftbessentials.home.max` This uses an integer for `<value>`
- `ftbessentials.back.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.spawn.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.home.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.tpa.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.rtp.cooldown` This uses an integer (seconds) for `<value>`

### Quest have a _gray_ question mark and cannot be completed, even though all dependencies have been finished?
This is a common bug with the mod FTBQuests. In the latest versions, we've disabled the ability to "finish" a quest before it's unlocked to prevent this issue, but if you've already pre-competed a quest, you might need to forcefully complete (or reset) the quest using level 2 Operator commands.

If you have the ability to do so, enter your FTBQuests screen, locate the quest you'd like to reset, enter "Edit Mode" by pressing on the pencil button in the bottom right corner of the screen, then **Right-Click** on the desired quest, and press **Reset Progress**.
If you need to reset the progress of someone else's quest, enter your FTBQuests screen, locate the quest you'd like to reset, enter "Edit Mode" by pressing on the pencil button in the bottom right corner of the screen, then **Right-Click** on the desired quest, and press **Copy ID**. Then run the command: `/ftbquests change_progress <IGN> reset <Quest ID>`

### Blank, Missing, or Invisible GUI/UI (Example Shaders, Building Gadget, etc.)

You may have come into a bug with the menu background blur. Enter your `Accessability Settings` and locate `Menu Background Blur` and disable it. The GUI should show up now.

### How much memory does your server need?
It depends on a few factors. Most notably:

- Number of players
- Play styles
- Number of bases (any teams?)
- The lowest TPS _you_ can tolerate.

For about 10 players, actively playing, matching player for gig (10gb) would most likely keep you good on TPS for a bit until the big bases come along. _Although_ unoptimized, laggy bases can tank a server's TPS alone, so do ensure that you aren't allowing that.

Playstyles means: How do the players plan to build their bases and setups? Unoptimized ones using entity based farms, or a lot of tick accelerating can cause a considerable amount of lag, but more optimized ones may fly right under the TPS radar.

The number of bases really just tells you how many different instances of crap there will be running at the same time. If all 10 people run one base, 10 gigs will get you far. If they split into 5 teams of 2, then maybe not _as_ much.

High TPS (no lag) is fantastic, but getting dips in TPS is common when you're playing Modded Minecraft. Most can get used to 15 TPS, and others (with time) can get used to 10 TPS or lower, though it can be a little annoying at times.

Extrapolate the 1 gig per 1 player and factor in the rest of the variables. More bases? More ram. Less Optimized? More ram.

For example, the public servers have about 16GB of ram, but once it gets up to 30 people, it can lag really badly (especially now that everyone's bases are big and complex). But sometimes, even 5 people with HUGE bases can start tanking the TPS, even if there isn't one singular thing that is laggy.

If you can, start at 10 for most servers (unless you only have 2 or 3 players on at a time, then lower it to 6-8). If you need, add more.

## How do I...?

### ...profile my game to analyze problems?
Run a Spark client profile for 30 seconds while doing the action that causes the lowered client performance. Use the following command:

`/sparkc profiler start --timeout 30`

Send the resulting URL it gives you once it finishes.

### ...calculate ==energy conversion== from one kind to another?

| EU   | FE   | AE   | J    | E    | LF   | :material-lightning-bolt: |
| :--- | :--- | :--- | :--- | :--- | :--- | :------------------------ |
| 0.1  | 1    | 2    | 2.5  | 1    | 1    | 1                         |

/// caption
Conversion ratios of various Energies
///

In [_**Craftoria**_](modpacks/Craftoria.md) the Flux Transformer will convert 1 EU to 50 FE, only.
Connecting EU directly to anything that runs on FE will yield a 1 EU : 10 FE result.

!!! info "Powering Modern Industrialization"
	No energy kind can be converted into EU. However [_Modern Industrialization_](mods/mi.md) has a config option for MI to allow this, if you wish it for you own worlds.

---
