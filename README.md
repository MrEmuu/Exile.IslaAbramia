# Exile.IslaAbramia
Mission and Server files w/ Easy Traders and Loot Spawn Building Positions. Default Loot Tables

This is a shared effort and credit will be given. 

Required Mods
==============
- ExileMod - http://www.exilemod.com/downloads/
- Cup Core - https://steamcommunity.com/sharedfiles/filedetails/?id=583496184 or http://cup-arma3.org/
- Isla Abramia: http://www.armaholic.com/page.php?id=30616 or https://steamcommunity.com/sharedfiles/filedetails/?id=648775794
              
Information
==============
The Exile_Server_Config.pbo has already been edited for this map. You will only need to edit the config.cpp if you want rcon, turn off halo, adj weather etc.
 
Building Loot Positions are already added but not tested for floating loot, if you notice any loot floating let me know in exilemod.com forum with the coordinates so i may correct.

LootTables are default and you will need to use http://www.exilemod.com/download-all-the-files/LootTableCompiler-1.0.2.zip
to compile loot if your using other mods.

The Map Markers and Single Trader with objects and trader data was provided by cantkillphantom - http://www.exilemod.com/profile/89301-cantkillphantom/

Easy trader was provided by Red Ned - http://www.exilemod.com/profile/41243-red_ned/ and https://github.com/redned70/Trader-Mod and incorported into this release by myself.

I have made the mission files so they are easy to edit. simply edit the hpp files included:
- config.cpp
- CfgRemoteExec.hpp
- CfgExileCustomCode.hpp
- CfgMusicPlaylist.hpp
- CfgMusic.hpp
- CfgSounds.hpp
- CfgFunctions.hpp
- CfgRscTitles.hpp
- CfgHints.cpp
- CfgNetworkMessages.hpp

CfgMusicPlaylist.hpp you can add classnames of custom music tracks, or remove default exile tracks if not wanted.
CfgMusic.hpp you can add your own tracks, I have left examples of 3, so you can see how the format would be.

For example, if you wanted a new intro song. you would make your ogg music file. call it introSong1.ogg and copy it into the Music folder.

then edit CfgMusicPlaylist.hpp

	Ambient[] = {"ExileTrack03","ExileTrack04"};
	Combat[] = {"ExileTrack06","ExileTrack07"};
	Intro[] = {"ExileTrack02","ExileTrack03","intro1"};
  
duplicate for combat and ambient if wanted, just note, that if you add music to your mission file, it will become very large.
 
I have tested this and it does load, it does snow when you are over snow texture.
