# NpcInteract
FFXI Windower addon for multiboxers to reduce tedious switching. Make your alts copy your main's NPC interactions!

Note that this addon has not been tested to work exhaustively in all cases. If you experience an issue,

# PLEASE DISABLE NPCINTERACT BEFORE FILING A TICKET!

Retry the interaction after restarting the character and disabling NpcInteract.

This addon should work in the following cases:

* Conquest NPCs (signet, etc.)
* Field Manuals (changing page, getting tab buffs)
* Custom Era Warp NPCs (NPC to XP location).
* Outpost warp
* Getting key items (telepoint, etc.)

For any other case, especially missions, I advise disabling NpcInteract, or at minimum double checking your progress manually on all characters.
Either way, you will probably experience a character getting frozen or stuck. The `npc retry` command only works occasionally, so you'll probably
have to restart that character. You can force close a character with the `terminate` command.

Again, if you experience an issue,

# PLEASE DISABLE NPCINTERACT BEFORE FILING A TICKET! 

Retry the interaction after restarting the character and disabling NpcInteract.

## Installation
After downloading, extract to your Windower addons folder. Make sure the folder is called NpcInteract, rather than NpcInteract-master or NpcInteract-v1.whatever. Your file structure should look like this:

    addons/NpcInteract/NpcInteract.lua

Once the addon is in your Windower addons folder, it won't show up in the Windower launcher. You need to add a line to your scripts/init.txt:

    lua load NpcInteract

## Commands

    //npc [help] -- Show this usage guide.
    //npc mirror [on/off] -- Toggle/enable/disable mirroring, causing all other alts to mirror this one.  
    //npc report [on/off] -- Toggle/enable/disable reporting, showing when alts successfully mirror the main.  
    //npc fade <duration> -- Set how long it takes the report box to fade.
    //npc retry -- Retry the last NPC interaction.  
    //npc reset -- Try this if alts get frozen when attempting to interact with an NPC.  
