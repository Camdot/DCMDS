|Command         |Description                    |Help                         |
|----------------|-------------------------------|-----------------------------|
|vvinvoke|Invoke/Call a path with arguments using VV\.|Usage: vvinvoke \<path\> \[arguments\.\.\.\]|
|vvread|Retrieve a path's value using VV \(View Variables\)\.|Usage: vvread \<path\>|
|vvwrite|Modify a path's value using VV \(View Variables\)\.|Usage: vvwrite \<path\>|
|replay_recording_start|Starts a replay recording, optionally with some time limit\.|Usage: replay\_recording\_start \[name\] \[overwrite\] \[time limit\]|
|replay_recording_stop|Stops a replay recording\.|Usage: replay\_recording\_stop|
|replay_recording_stats|Displays information about the current replay recording\.|Usage: replay\_recording\_stats|
|hwid|Returns the current HWID \(HardWare ID\)\.|Usage: hwid|
|setambientlight|Allows you to set the ambient light for the specified map, in SRGB\.|setambientlight \[mapid\] \[r g b a\]|
|saveconfig|Saves the server configuration to the config file\.|saveconfig|
|dump_dependency_injectors|Dump IoCManager's dependency injector cache\.|Usage: dump\_dependency\_injectors|
|dump_event_tables|Prints directed event tables for an entity\.|Usage: dump\_event\_tables \<entityUid\>|
|dump_net_comps|Prints the table of networked components\.|Usage: dump\_net\-comps|
|dump_netserializer_type_map|Dump NetSerializer's type map and serializer hash\.|Usage: dump\_netserializer\_type\_map|
|echo|Echo arguments back to the console|Usage: echo "\<message\>"|
|exec|Executes a script file from the game's writeable user data|Usage: exec \<fileName\><br>Each line in the file is executed as a single command, unless it starts with a \#|
|gc|Run the GC \(Garbage Collector\)|Usage: gc \[generation\]<br>Uses GC\.Collect\(\) to execute the Garbage Collector\.<br>If an argument is provided, it is parsed as a GC generation number and GC\.Collect\(int\) is used\.<br>Use the 'gfc' command to do an LOH\-compacting full GC\.|
|gcf|Run the GC, fully, compacting LOH and everything\.|Usage: gcf<br>Does a full GC\.Collect\(2, GCCollectionMode\.Forced, true, true\) while also compacting LOH\.<br>This will probably lock up for hundreds of milliseconds, be warned\.|
|gc_mode|Change/Read the GC Latency mode|Usage: gc\_mode \[type\]<br>If no argument is provided, returns the current GC latency mode\.<br>If an argument is passed, it is parsed as GCLatencyMode and set as the GC latency mode\.|
|mem|Prints managed memory info|Usage: mem|
|help|Display general help or help text for a specific command|Usage: help \[command name\]<br>When no command name is provided, displays general\-purpose help text\. If a command name is provided, displays help text for that command\.|
|lsasm|Lists loaded assemblies by load context|Usage: lsasm|
|list|Lists available commands, with optional search filter|Usage: list \[filter\]<br>Lists all available commands\. If an argument is provided, it will be used to filter commands by name\.|
|loglevel|Changes the log level for a provided sawmill\.|Usage: loglevel \<sawmill\> \<level\><br>sawmill: A label prefixing log messages\. This is the one you're setting the level for\.<br>level: The log level\. Must match one of the values of the LogLevel enum\.|
|testlog|Writes a test log to a sawmill\.|Usage: testlog \<sawmill\> \<level\> \<message\><br>sawmill: A label prefixing the logged message\.<br>level: The log level\. Must match one of the values of the LogLevel enum\.<br>message: The message to be logged\. Wrap this in double quotes if you want to use spaces\.|
|oldhelp|||
|szr_stats|Report serializer statistics\.|Usage: szr\_stats|
|vfs_ls|List directory contents in the VFS\.|Usage: vfs\_list \<path\><br>Example:<br>vfs\_list /Assemblies|
|cvar|Gets or sets a CVar\.|Usage: cvar \<name \\| ?\> \[value\]<br>If a value is passed, the value is parsed and stored as the new value of the CVar\.<br>If not, the current value of the CVar is displayed\.<br>Use 'cvar ?' to get a list of all registered CVars\.|
|cvar_subs|Lists the OnValueChanged subscriptions for a CVar\.|Usage: cvar\_subs \<name\>|
|audio_length|Shows the length of an audio file|Usage: audio\_length \<file name\>|
|vv|Opens View Variables\.|Usage: vv \<entity ID\\|IoC interface name\\|SIoC interface name\>|
|devwindow|Dev Window|Usage: devwindow|
|testopenfile|||
|scene|Immediately changes the UI scene/state\.|Usage: scene \<className\>|
|textedit_ropeviz|||
|textedit_rebalance|||
|textedit_debugoverlay|||
|textedit_queuelinebreak|||
|loadprototype|Load a prototype file into the server\.|loadprototype|
|uploadfile|Uploads a resource to the server\.|uploadfile \[relative path for the resource\]|
|uploadfolder|Uploads a folder from your UserData folder recursively to the server contentDB\.|uploadfolder \[folder you want to upload in userdata/UploadFolder\]|
|replay_play|Resume replay playback\.|replay\_play|
|replay_pause|Pause replay playback|replay\_pause|
|replay_toggle|Resume or pause replay playback\.|replay\_toggle|
|replay_stop|Stop and unload a replay\.|replay\_stop|
|replay_load|Load and start a replay\.|replay\_load \<replay folder\>|
|replay_set_time|Jump forwards or backwards to some specific time\.|replay\_set \<tick or time\>|
|replay_skip|Skip forwards or backwards in time\.|replay\_skip \<tick or timespan\>|
|replay_toggleui|cmd\-replay\-toggleui\-desc|cmd\-replay\-toggleui\-help|
|profsnap|Make a profiling snapshot\.|Usage: profsnap|
|showislands|Shows the current physics bodies involved in each physics island\.|Usage: showislands|
|showgridnodes|Shows the nodes for grid split purposes\.|Usage: showgridnodes|
|reloadtiletextures|Reloads the tile texture atlas to allow hot reloading tile sprites|Usage: reloadtiletextures|
|bind|Binds an input key combination to an input command\.|Usage: bind \<KeyName\> \<BindMode\> \<InputCommand\><br>Note that this DOES NOT automatically save bindings\.<br>Use the 'svbind' command to save binding configuration\.|
|svbind|||
|vram|Displays video memory usage statics by the game\.|Usage: vram|
|net_entityreport|Toggles the net entity report panel\.|Usage: net\_entityreport|
|net_graph|Toggles the net statistics panel\.|Usage: net\_graph|
|net_watchent|Dumps all network updates for an EntityId to the console\.|Usage: net\_watchent \<0\\|EntityUid\>|
|net_draw_interp|Toggles the debug drawing of the network interpolation\.|Usage: net\_draw\_interp \<0\\|EntityUid\>|
|showspritebb|Toggle whether sprite bounds are shown|Usage: showspritebb|
|togglelookup|Shows / hides entitylookup bounds via an overlay\.|Usage: togglelookup|
|>|Executes server\-side commands|Usage: \> \<command\> \[arg\] \[arg\] \[arg\.\.\.\]<br>Executes a command on the server\. This is necessary if a command with the same name exists on the client, as simply running the command would run the client command first\.|
|addcompc|Adds a component to an entity on the client\.|addcompc \<uid\> \<componentName\>|
|rmcompc|Removes a component from an entity on the client\.|rmcomp \<uid\> \<componentName\>|
|cspawn|Spawns a client\-side entity with specific type at your feet\.|cspawn \<entity type\>|
|cls|Clears the console\.|Clears the debug console of all messages\.|
|fill|Fill up the console for debugging\.|Fills the console with some nonsense for debugging\.|
|dumpentities|Dump entity list\.|Dumps entity list of UIDs and prototype\.|
|getcomponentregistration|Gets component registration information\.|Usage: getcomponentregistration \<componentName\>|
|monitor|Toggles a debug monitor in the F3 menu\.|Usage: monitor \<name\><br>Possible monitors are: Fps, Coords, Net, Time, Frames, Memory, Clyde, Input, Bandwidth, Prof, System<br>You can also use the special values "\-all" and "\+all" to hide or show all monitors, respectively\.|
|fuck|Throws an exception|Throws an exception|
|showpos|Enables debug drawing over all entity positions in the game\.|Usage: showpos|
|showrot|||
|showrays|Toggles debug drawing of physics rays\. An integer for \<raylifetime\> must be provided\.|Usage: showrays \<raylifetime\>|
|disconnect|Immediately disconnect from the server and go back to the main menu\.|Usage: disconnect|
|entfo|Displays verbose diagnostics for an entity\.|Usage: entfo \<entityuid\><br>The entity UID can be prefixed with 'c' to convert it to a client entity UID\.|
|overrideplayername|Changes the name used when attempting to connect to the server\.|Usage: overrideplayername \<name\>|
|ldrsc|Pre\-caches a resource\.|Usage: ldrsc \<path\> \<type\>|
|rldrsc|Reloads a resource\.|Usage: rldrsc \<path\> \<type\>|
|guidump|Dump GUI tree to /guidump\.txt in user data\.|Usage: guidump|
|setclipboard|Sets the system clipboard|Usage: setclipboard \<text\>|
|getclipboard|Gets the system clipboard|Usage: Getclipboard|
|togglelight|Toggles light rendering\.|Usage: togglelight|
|togglefov|Toggles fov for client\.|Usage: togglefov|
|togglehardfov|Toggles hard fov for client\. \(for debugging space\-station\-14\#2353\)|Usage: togglehardfov|
|toggleshadows|Toggles shadow rendering\.|Usage: toggleshadows|
|togglelightbuf|Toggles lighting rendering\. This includes shadows but not FOV\.|Usage: togglelightbuf|
|rldshader|Reloads all shaders\.|Usage: rldshader|
|cldbglyr|Toggle fov and light debug layers\.|Usage: cldbglyr \<layer\>: Toggle \<layer\><br>cldbglyr: Turn all Layers off|
|keyinfo|||
|showanchored|Shows anchored entities on a particular tile|Usage: showanchored|
|dmetamem|Dumps a type's members in a format suitable for the sandbox configuration file\.|Usage: dmetamem \<type\>|
|launchauth|Load authentication tokens from launcher data to aid in testing of live servers\.|Usage: launchauth \<account name\>|
|lightbb|Toggles whether to show light bounding boxes\.|Usage: lightbb|
|lsmonitor|||
|monitorinfo|Monitors info|Usage: monitorinfo \<id\>|
|setmonitor|Set monitor|Usage: setmonitor \<id\>|
|physics|Shows a debug physics overlay\. The arg supplied specifies the overlay\.|Usage: physics \<aabbs / com / contactnormals / contactpoints / distance / joints / shapeinfo / shapes\>|
|profileEntitySpawning|Profiles entity spawning with n entities|Usage: profileEntitySpawning \\| profileEntitySpawning \<amount\> \<prototype\>|
|hardquit|Kills the game client instantly\.|Kills the game client instantly, leaving no traces\. No telling the server goodbye\.|
|quit|Shuts down the game client gracefully\.|Properly shuts down the game client, notifying the connected server and such\.|
|rldloc|Reloads localization \(client & server\)\.|Usage: rldloc|
|csi|Opens a C\# interactive console\.|Usage: csi|
|watch|Opens a variable watch window\.|Usage: watch|
|scsi|Opens a C\# interactive console on the server\.|Usage: scsi|
|sendgarbage|Sends garbage to the server\.|The server will reply with 'no u'|
|setinputcontext|Sets the active input context\.|Usage: setinputcontext \<context\>|
|uitest|Open a dummy UI testing window|Usage: uitest|
|uitest2|Opens a UI control testing OS window|Usage: uitest2 \<tab\>|
|showvelocities|Displays your angular and linear velocities\.|Usage: showvelocities|
|showaudio|||
|midipanic|Turns off every note for every active MIDI renderer\.||
|testcommand|A test command for demonstration purposes\.|Usage: testcommand \<arg1\> \<arg2\> \.\.\.<br>This command does nothing but serves as an example\.|
|showgunspread|Shows gun spread overlay for debugging|showgunspread|
|showmeleespread|Shows the current weapon's range and arc for debugging|showmeleespread|
|votemenu|Opens the voting menu|Usage: votemenu|
|showemergencyshuttle|Shows the expected position of the emergency shuttle|showemergencyshuttle|
|replay_toggle_screenshot_mode|cmd\-replay\-toggle\-screenshot\-mode\-desc|cmd\-replay\-toggle\-screenshot\-mode\-help|
|showbiome|||
|showhtn|Shows the current status for HTN NPCs|showhtn|
|nodevis|Toggles node group visualization||
|nodevisfilter|Toggles showing a specific group on nodevis|Usage: nodevis \[filter\]<br>Omit filter to list currently masked\-off|
|clearnetworklinkoverlays|Clear all network link overlays\.|clearnetworklinkoverlays|
|toggleselfghost|Toggles seeing your own ghost\.|toggleselfghost|
|toggleghostvisibility|Toggles ghost visibility on the client\.|toggleghostvisibility \[bool\]|
|toggledecals|Toggles decaloverlay|toggledecals|
|loadacts|Loads action toolbar assignments from a user\-file\.|Usage: loadacts \<user resource path\>|
|atvrange|Sets the atmos debug range \(as two floats, start \[red\] and end \[blue\]\)|Usage: atvrange \<start\> \<end\>|
|atvmode|Sets the atmos debug mode\. This will automatically reset the scale\.|Usage: atvmode \<TotalMoles/GasMoles/Temperature\> \[\<gas ID \(for GasMoles\)\>\]|
|atvcbm|Changes from red/green/blue to greyscale|Usage: atvcbm \<true/false\>|
|credits|Opens the credits window|Usage: credits|
|showmarkers|Toggles visibility of markers such as spawn points\.|Usage: showmarkers|
|showsubfloor|Makes entities below the floor always visible\.|Usage: showsubfloor|
|showsubfloorforever|Makes entities below the floor always visible until the client is restarted\.|Usage: showsubfloorforever|
|notify|Send a notify client side\.|Usage: notify \<message\>|
|pathfinder|Toggles visibility of pathfinding debuggers\.|Usage: pathfinder \[options\]|
|entitymenug|Sets the entity menu grouping type\.|Usage: entitymenug \<0:2\>|
|hidemechanisms|Reverts the effects of showmechanisms|Usage: hidemechanisms|
|mappingclientsidesetup|Sets up the lighting control and such settings client\-side\. Sent by 'mapping' to client\.|Usage: mappingclientsidesetup|
|openahelp|Opens AHelp channel for a given NetUserID, or your personal channel if none given\.|Usage: openahelp \[\<netuserid\>\]|
|menuvis|Set restrictions about what entities to show on the entity context menu\.|Usage: \{Command\} \[NoFoV\] \[InContainer\] \[Invisible\] \[All\]|
|showhealthbars|Toggles health bars above mobs\.|Usage: showhealthbars \[\<DamageContainerId\>\]|
|showmechanisms|Makes mechanisms visible, even when they shouldn't be\.|Usage: showmechanisms|
|toggleoutline|Toggles outline drawing on entities\.|Usage: toggleoutline|
|zoom|Sets the zoom of the main eye\.|zoom \( \<scale\> \\| \<X\-scale\> \<Y\-scale\> \)|
|changelog|Opens the changelog|Usage: changelog|
|showambient|Shows all AmbientSoundComponents in the viewport|showambient|
|showaccessreaders|Toggles showing access reader permissions on the map|Overlay Info:<br>\-Disabled \\| The access reader is disabled<br>\+Unrestricted \\| The access reader has no restrictions<br>\+Set \[Index\]: \[Tag Name\]\\| A tag in an access set \(accessor needs all tags in the set to be allowed by the set\)<br>\+Key \[StationUid\]: \[StationRecordKeyId\] \\| A StationRecordKey that is allowed<br>\-Tag \[Tag Name\] \\| A tag that is not allowed \(takes priority over other allows\)|
|pausemap|Pauses a map, pausing all simulation processing on it\.|pausemap \<map ID\>|
|querymappaused|Check whether a map is paused or not\.|querymappaused \<map ID\>|
|unpausemap|unpauses a map, resuming all simulation processing on it\.|Usage: unpausemap \<map ID\>|
|resetent|Reset an entity to the most recently received server state\. This will also reset entities that have been detached to null\-space\.|Usage: resetent \<Entity UID\>|
|resetallents|Resets all entities to the most recently received server state\. This only impacts entities that have not been detached to null\-space\.|Usage: resetallents|
|detachent|Detach an entity to null\-space, as if it had left PVS range\.|Usage: detachent \<Entity UID\>|
|localdelete|Deletes an entity\. Unlike the normal delete command, this is CLIENT\-SIDE\. Unless the entity is a client\-side entity, this will likely cause errors\.|Usage: localdelete \<Entity UID\>|
|fullstatereset|Discards any entity state information and requests a full\-state from the server\.|Usage: fullstatereset|
|options|Opens options menu, optionally with a specific tab selected\.|Usage: options \[tab\]|
|fuckrules|||
|incmd|Inserts an input command into the simulation|incmd \<KeyFunction\> \<KeyState\> \[wxPos\] \[wyPos\]|
|loc|Prints the absolute location of the player's entity to console\.|loc|
|sggcell|Lists entities on a snap grid cell\.|Usage: sggcell \<gridID\> \<vector2i\>\\nThat vector2i param is in the form x\<int\>,y\<int\>\.|
|gridtc|Gets the tile count of a grid\.|Usage: gridtc \<gridId\>|
|chunkinfo|Gets info about a chunk under your mouse cursor\.|Usage: chunkinfo|
|showchunkbb|||
|sudo|sudo make me a sandwich|sudo \<command\>|
|rmmap|Removes a map from the world\. You cannot remove nullspace\.|rmmap \<mapId\>|
|spawn|Spawns an entity with specific type\.|spawn \<prototype\> OR spawn \<prototype\> \<relative entity ID\> OR spawn \<prototype\> \<x\> \<y\>|
|hub_advertise_now|Immediately advertise to the master hub server|Usage: hub\_advertise\_now|
|merge_grids|Combines 2 grids into 1 grid|merge\_grids \<gridUid1\> \<gridUid2\> \<offsetX\> \<offsetY\> \[angle\]|
|addcomp|Adds a component to an entity\.|addcomp \<uid\> \<componentName\>|
|savegrid|Serializes a grid to disk\.|savegrid \<gridID\> \<Path\>|
|loadgrid|Loads a grid from a file into an existing map\.|loadgrid \<MapID\> \<Path\> \[x y\] \[rotation\] \[storeUids\]|
|savemap|Serializes a map to disk\. Will not save a post\-init map unless forced\.|savemap \<MapID\> \<Path\> \[force\]|
|loadmap|Loads a map from disk into the game\.|loadmap \<MapID\> \<Path\> \[x\] \[y\] \[rotation\] \[consistentUids\]|
|listplayers|Lists all players currently connected\.|listplayers|
|kick|Kicks a connected player out of the server, disconnecting them\.|kick \<PlayerIndex\> \[\<Reason\>\]|
|rmcomp|Removes a component from an entity\.|rmcomp \<uid\> \<componentName\>|
|scale|Increases or decreases an entity's size naively\.|scale \<entityUid\> \<float\>|
|spin|Causes an entity to spin\. Default entity is the attached player's parent\.|spin velocity \[drag\] \[entityUid\]|
|shutdown|Gracefully shuts down the server\.|shutdown|
|netaudit|Prints into about NetMsg security\.|netaudit|
|showtime|Shows the server time\.|showtime|
|addview|Allows you to subscribe to an entity's view for debugging purposes\.|addview \<entityUid\>|
|removeview|Allows you to unsubscribe to an entity's view for debugging purposes\.|removeview \<entityUid\>|
|listlavaland|Logs a list of all active lavaland maps into the console\.||
|mappinglavaland|Loads lavaland world on a new map\. Be careful, this can cause freezes on runtime\!|mappinglavaland \<prototype id\> \<seed\>|
|timetransferpanel|Opens time transfer menu||
|whitelistadd|Adds the player with the given username to the server whitelist\.|Usage: whitelistadd \<username or User ID\>|
|whitelistremove|Removes the player with the given username from the server whitelist\.|Usage: whitelistremove \<username or User ID\>|
|kicknonwhitelisted|Kicks all non\-whitelisted players from the server\.|Usage: kicknonwhitelisted|
|createvote|Creates a vote|Usage: createvote \<'restart'\\|'preset'\\|'map'\>|
|customvote|Creates a custom vote|Usage: customvote \<title\> \<option1\> \<option2\> \[option3\.\.\.\]|
|vote|Votes on an active vote|vote \<voteId\> \<option\>|
|listvotes|Lists currently active votes|Usage: listvotes|
|cancelvote|Cancels an active vote|Usage: cancelvote \<id\><br>You can get the ID from the listvotes command\.|
|invokeverb|Invokes a verb with the given name on an entity, with the player entity|invokeverb \<playerUid \\| "self"\> \<targetUid\> \<verbName \\| "interaction" \\| "activation" \\| "alternative"\>|
|listverbs|Lists all verbs that a player can use on a given entity\.|listverbs \<playerUid \\| "self"\> \<targetUid\>|
|showvalues|Dumps all stats for a particular category into a table\.|showvalues \<cargosell / lathesell / melee / itemsize\>|
|adduplink|Creates uplink on selected item and link it to users account|Usage: adduplink \[username\] \[item\-id\]|
|sendstationgoal|Sends the selected station target to all faxes that can receive it|Usage: sendstationgoal \<Goal Prototype ID\>|
|startsingularityengine|Automatically turns on the particle accelerator and containment field emitters\.|startsingularityengine|
|delayroundend|Stops the timer that ends the round when the emergency shuttle exits hyperspace\.|delayroundend|
|dock|Attempts to dock 2 airlocks together\. Doesn't check whether it is valid\.|dock \<airlock entityuid1\> \<airlock entityuid2\>|
|dockemergencyshuttle|Calls the emergency shuttle and docks it to the station\.\.\. if it can\.|dockemergencyshuttle|
|launchemergencyshuttle|Early launches the emergency shuttle if possible\.|launchemergencyshuttle|
|colornetwork|color\-network\-command\-description|color\-network\-command\-help\-text|
|salvageruler|Measures grids on this map to get a total world AABB\. Use for salvage bounds specifications\.|Usage: salvageruler|
|addrole|Adds a role to a player's mind\.|addrole \<session ID\> \<role\>|
|listroles|Lists roles|listroles|
|rmrole|Removes a role from a player's mind\.|rmrole \<session ID\> \<Role Type\><br>That role type is the actual C\# type name\.|
|showradiation|Toggle visibility of radiation rays coming from rad sources|Usage: showradiation|
|setbatterypercent|Drains or recharges a battery by entity uid and percentage, i\.e\.: forall with Battery do setbatterypercent $ID 0|setbatterypercent \<id\> \<percent\>|
|powerstat|Shows statistics for pow3r|Usage: powerstat|
|lspsionics|List psionics\.|No arguments\.|
|addpsionicpower|Initialize an entity as Psionic with a given PowerPrototype|Argument 1 must be an EntityUid, and argument 2 must be a string matching the PrototypeId of a PsionicPower\.|
|addrandompsionicpower|Initialize an entity as Psionic with a random PowerPrototype that is available for that entity to roll\.|Argument 1 must be an EntityUid\.|
|removepsionicpower|Remove a Psionic power from an entity\.|Argument 1 must be an EntityUid, and argument 2 must be a string matching the PrototypeId of a PsionicPower\.|
|removeallpsionicpowers|Remove all Psionic powers from an entity\.|Argument 1 must be an EntityUid\.|
|glimmershow|Show the current glimmer level\.|No arguments\.|
|glimmerset|Set glimmer to a number\.|glimmerset \(integer\)|
|nukecodes|Send nuke codes to a station's communication consoles|nukecodes \[station EntityUid\]|
|nukearm|Toggle nuclear bomb timer\. You can set timer directly\. Uid is optional\.|nukearm \<timer\> \<uid\>|
|addnpc|Add a HTN NPC component with a given root task|Usage: addnpc \<entityId\> \<rootTask\><br>    entityID: Uid of entity to add the AiControllerComponent to\. Open its VV menu to find this\.<br>    rootTask: Name of a behaviorset to add to the component on initialize\.|
|npc|Opens the debug window for NPCs|npc|
|npcdomain|Lists the domain of a particular HTN compound task|npcdomain \<htncompoundtask\>|
|lockeyes|Prevents eyes from being rotated any further|lockeyes \<true/false\>|
|rotateeyes|Rotates every player's current eye to the specified rotation|rotateeyes \<degrees \(default 0\)\>|
|get-motd|Prints the Message Of The Day\.|get\-motd|
|motd|Prints or sets the Message Of The Day\.|motd \[ message\.\.\. \]|
|set-motd|Sets or clears the Message Of The Day\.|set\-motd \[ message\.\.\. \]|
|makesentient|Makes an entity sentient \(able to be controlled by a player\)|makesentient \<entity id\>|
|mindinfo|Lists info for the mind of a specific player\.|mindinfo \<session ID\>|
|rename|Renames an entity and its cloner entries, ID cards, and PDAs\.|rename \<Username\\|EntityUid\> \<New character name\>|
|griddrag|Allows someone with permissions to drag grids around\.|griddrag|
|planet|Converts the supplied map into a planet with some specific biome\.|planet \<mapid\> \<biome\>\.|
|resave|||
|mapping|Create or load a map and teleports you to it\.|Usage: mapping \[MapID\] \[Path\]|
|mailto|Queue a parcel to be delivered to an entity\. Example usage: \`mailto 1234 5678 false false\`\. The target container's contents will be transferred to an actual mail parcel\.|Usage: mailto \<recipient entityUid\> \<container entityUid\> \[is\-fragile: true or false\] \[is\-priority: true or false\] \[is\-large: true or false, optional\]|
|mailnow|Force all mail teleporters to deliver another round of mail as soon as possible\. This will not bypass the undelivered mail limit\.|Usage: mailnow|
|languagelist|List languages your current entity can speak at the current moment\.|Usage: languagelist|
|saylang|Send a message in a specific language\. To choose a language, you can use either the name of the language, or its position in the list of languages\.|Usage: saylang \<language id\> \<message\>\. Example: saylang TauCetiBasic "Hello World\!"\. Example: saylang 1 "Hello World\!"|
|languageselect|Select the currently spoken language of your entity\. You can use either the name of the language, or its position in the list of languages\.|Usage: languageselect \<language id\>\. Example: languageselect 1\. Example: languageselect TauCetiBasic|
|tilepry|Pries up all tiles in a radius around the user\.|Usage: tilepry \<radius\>|
|showrules|Opens the rules popup for the specified player\.|showrules \<username\> \[seconds\]|
|ghostkick|Kick a client from the server as if their network just dropped\.|Usage: ghostkick \<Player\> \[Reason\]|
|delaystart|Delays the round start\.|Usage: delaystart \<seconds\><br>Pauses/Resumes the countdown if no argument is provided\.|
|endround|Ends the round and moves the server to PostRound\.||
|forcemap|Forces the game to start with a given map next round\.|forcemap \<map ID\>|
|forcepreset|Forces a specific game preset to start for the current lobby\.|Usage: forcepreset \<preset\>|
|golobby|Enables the lobby and restarts the round\.|Usage: golobby / golobby \<preset\>|
|joingame|||
|observe|||
|respawn|Respawns a player, kicking them back to the lobby\.|respawn \[player\]|
|restartround|Ends the current round and starts the countdown for the next lobby\.||
|restartroundnow|Moves the server from PostRound to a new PreRoundLobby\.||
|setgamepreset|Sets the game preset for the current round\.|setgamepreset \<id\>|
|startround|Ends PreRoundLobby state and starts the round\.||
|toggledisallowlatejoin|Allows or disallows latejoining during mid\-game\.|Usage: toggledisallowlatejoin \<disallow\>|
|toggleready|||
|showfluids|Toggles seeing puddle debug overlay\.|Usage: showfluids|
|spawnentitylist|Spawns a list of entities around you|Usage: spawnentitylist \<entityListPrototypeId\>|
|electrocute|Electrocutes the specified entity, defaults to 10 seconds and 10 damage\. Shocking\!|electrocute \<uid\> \<seconds\> \<damage\>|
|tubeconnections|Shows all the directions that a tube can connect in\.|Usage: tubeconnections \<entityUid\>|
|addobjective|Adds an objective to the player's mind\.|addobjective \<username\> \<objectiveID\>|
|lsobjectives|Lists all objectives in a players mind\.|Usage: lsobjectives \<username\>|
|rmobjective|Removes an objective from the player's mind\.|rmobjective \<username\> \<index\>|
|hungry|Makes you hungry\.|hungry|
|ghost|Give up on life and become a ghost\.|The ghost command turns you into a ghost and makes the character you played permanently catatonic\.<br>Please note that you cannot return to your character's body after ghosting\.|
|ghostroles|Opens the ghost role request window\.|ghostroles|
|makeghostrole|Turns an entity into a ghost role\.|Usage: makeghostrole \<entity uid\> \<name\> \<description\> \[\<rules\>\]|
|makeghostroleraffled|Turns an entity into a raffled ghost role\.|Usage: makeghostroleraffled \<entity uid\> \<name\> \<description\> \(\<settings prototype\> \\| \<initial duration\> \<extend by\> \<max duration\>\) \[\<rules\>\]<br>Durations are in seconds\.|
|editdecal|Edits a decal\.|editdecal \<gridId\> \<uid\> \<mode\>\\n<br>Possible modes are:\\n<br>\- position \<x position\> \<y position\>\\n<br>\- color \<color\>\\n<br>\- id \<id\>\\n<br>\- rotation \<degrees\>\\n<br>\- zindex \<zIndex\>\\n<br>\- clean \<cleanable\><br>|
|adddecal|Creates a decal on the map|adddecal \<id\> \<x position\> \<y position\> \<gridId\> \[angle=\<angle\> zIndex=\<zIndex\> color=\<color\>\]|
|rmdecal|removes a decal|rmdecal \<uid\> \<gridId\>|
|godmode|Makes your entity or another invulnerable to almost anything\. May have irreversible changes\.|Usage: godmode / godmode \<entityUid\>|
|damage|Add or remove damage to an entity\.|Usage: damage \<type/group\> \<amount\> \[ignoreResistances\] \[uid\]|
|crewmanifest|Opens the crew manifest for the given station\.|Usage: crewmanifest \<entity uid\>|
|fixrotations|Sets the rotation of all occluders, low walls and windows to south\.|Usage: fixrotations \<gridId\> \\| fixrotations|
|tilereplace|Replaces one tile with another\.|Usage: tilereplace \[\<gridId\>\] \<src\> \<dst\>|
|tilewalls|Puts an underplating tile below every wall on a grid\.|Usage: tilewalls \<gridId\> \\| tilewalls|
|tilewindows|Puts a reinforced plating tile below every window on a grid\.|Usage: tilewindows \<gridId\> \\| tilewindows|
|grant_connect_bypass|Temporarily allow a user to bypass regular connection checks\.|Usage: grant\_connect\_bypass \<user\> \[duration minutes\]<br>Temporarily grants a user the ability to bypass regular connections restrictions\.<br>The bypass only applies to this game server and will expire after \(by default\) 1 hour\.<br>They will be able to join regardless of whitelist, panic bunker, or player cap\.|
|blacklistadd|Adds the player with the given username to the server blacklist\.|Usage: blacklistadd \<username\>|
|blacklistremove|Removes the player with the given username from the server blacklist\.|Usage: blacklistremove \<username\>|
|upgradeaction|Upgrades an action by one level, or to the specified level, if applicable\.|upgradeaction\-command\-help|
|dumpreagentguidetext|Dumps the guidebook text for a reagent to the console|dumpreagentguidetext \<reagent\>|
|asay|Send chat messages to the private admin chat channel\.|asay \<text\>|
|looc|Send Local Out Of Character chat messages\.|looc \<text\>|
|me|Perform an action\.|me \<text\>|
|ooc|Send Out Of Character chat messages\.|ooc \<text\>|
|say|Send chat messages to the local channel or a specified radio channel\.|say \<text\>|
|setlooc|Allows you to enable or disable LOOC\.|Usage: setlooc OR setlooc \[value\]|
|setooc|Allows you to enable or disable OOC\.|Usage: setooc OR setooc \[value\]|
|subtle|Perform a subtle action\.|subtle \<text\>|
|subtleooc|Perform a subtle OOC action\.|subtleooc \<text\>|
|suicide|Commits suicide|The suicide command gives you a quick way out of a round while remaining in\-character\.<br>The method varies, first it will attempt to use the held item in your active hand\.<br>If that fails, it will attempt to use an object in the environment\.<br>Finally, if neither of the above worked, you will die by biting your tongue\.|
|tsay|Send chat messages to the telepathic\.|tsay \<text\>|
|whisper|Send chat messages to the local channel as a whisper|whisper \<text\>|
|loadcharacter|Applies your currently selected character to an entity|Usage: loadcharacter \\| loadcharacter \<entityUid\> \\| loadcharacter \<entityUid\> \<characterName\>|
|spawncharacter|Spawns your currently selected/specified character|Usage: spawncharacter \\| spawncharacter \<characterName\>|
|changestocksprice|Changes a company's stock price to the specified number\.|changestockprice \<Company index\> \<New price\> \[Station UID\]|
|addstockscompany|Adds a new company to the stocks market\.|addstockscompany \<Display name\> \<Base price\> \[Station UID\]|
|addhand|Adds a hand to your entity\.|Usage: addhand \<entityUid\> \<handPrototypeId\> / addhand \<entityUid\> / addhand \<handPrototypeId\> / addhand|
|attachbodypart|Attaches a body part to you or someone else\.|attachbodypart \<partEntityUid\> / attachbodypart \<entityUid\> \<partEntityUid\>|
|destroymechanism|Destroys a mechanism from your entity|Usage: destroymechanism \<mechanism\>|
|removehand|Removes a hand from your entity\.|Usage: removehand|
|addatmos|Adds atmos support to a grid\.|addatmos \<GridId\>|
|addgas|Adds gas at a certain position\.|addgas \<X\> \<Y\> \<GridEid\> \<Gas\> \<moles\>|
|deletegas|Removes all gases from a grid, or just of one type if specified\.|Usage: deletegas \<GridId\> \<Gas\> / deletegas \<GridId\> / deletegas \<Gas\> / deletegas|
|fillgas|Adds gas to all tiles in a grid\.|fillgas \<GridEid\> \<Gas\> \<moles\>|
|listgases|Prints a list of gases and their indices\.|listgases|
|removegas|Removes an amount of gases\.|removegas \<X\> \<Y\> \<GridId\> \<amount\> \<ratio\><br>If \<ratio\> is true, amount will be treated as the ratio of gas to be removed\.|
|setatmostemp|Sets a grid's temperature \(in kelvin\)\.|Usage: setatmostemp \<GridId\> \<Temperature\>|
|setmapatmos|Sets a map's atmosphere|setmapatmos \<mapid\> \<space\> \[\<temperature\> \[moles\.\.\.\]\]|
|settemp|Sets a tile's temperature \(in kelvin\)\.|Usage: settemp \<X\> \<Y\> \<GridId\> \<Temperature\>|
|showatmos|Toggles seeing atmos debug overlay\.|Usage: showatmos|
|announce|Send an in\-game announcement\.|announce \<sender\> \<message\> \<sound\> \<announcer\>|
|clearalert|Clears an alert for a player, defaulting to current player|clearalert \<alertType\> \<name or userID, omit for current player\>|
|showalert|Shows an alert for a player, defaulting to current player|showalert \<alertType\> \<severity, \-1 if no severity\> \<name or userID, omit for current player\>|
|setalertlevel|Set current station alert level for grid on which the player is standing\.|Usage: setalertlevel \<level\> \[locked\]|
|isafk|Checks if a specified player is AFK|Usage: isafk \<playerName\>|
|addbodypart|Adds a given entity to a containing body\.|Usage: addbodypart \<entity uid\> \<body uid\> \<part slot\> \<part type\>|
|addstorage|Adds a given entity to a containing storage\.|Usage: addstorage \<entity uid\> \<storage uid\>|
|addmechanism|Adds a given entity to a containing body\.|Usage: addmechanism \<entity uid\> \<bodypart uid\>|
|addpolymorphaction|Takes an entity and gives them a voluntary polymorph\.|addpolymorphaction \<id\> \<polymorph prototype\>|
|addreagent|Add \(or remove\) some amount of reagent from some solution\.|Usage: addreagent \<target\> \<solution\> \<reagent\> \<quantity\>|
|adminlogbulk|Adds debug logs to the database\.|Usage: adminlogbulk \<amount\> \<parallel\>|
|adminwho|Returns a list of all admins on the server|Usage: adminwho|
|aghost|Makes you an admin ghost\.|aghost|
|announceui|Opens the announcement UI|announceui|
|babyjail|Toggles the baby jail, which enables stricter restrictions on who's allowed to join the server\.|Usage: babyjail|
|babyjail_show_reason|Toggles whether or not to show connecting clients the reason why the baby jail blocked them from joining\.|Usage: babyjail\_show\_reason|
|babyjail_max_account_age|Gets or sets the maximum account age in minutes that an account can have to be allowed to connect with the baby jail enabled\.|Usage: babyjail\_max\_account\_age \<hours\>|
|babyjail_max_overall_hours|Gets or sets the maximum overall playtime in minutes that an account can have to be allowed to connect with the baby jail enabled\.|Usage: babyjail\_max\_overall\_hours \<hours\>|
|ban|Bans somebody|Usage: ban \<name or user ID\> \<reason\> \[duration in minutes, leave out or 0 for permanent ban\]|
|ban_exemption_update|Set an exemption to a type of ban on a player\.|Usage: ban\_exemption\_update \<player\> \<flag\> \[\<flag\> \[\.\.\.\]\]<br>Specify multiple flags to give a player multiple ban exemption flags\.<br>To remove all exemptions, run this command and give "None" as only flag\.|
|ban_exemption_get|Show ban exemptions for a certain player\.|Usage: ban\_exemption\_get \<player\>|
|banlist|Lists a user's active bans\.|Usage: banlist \<name or user ID\>|
|banpanel|Opens the ban panel|Usage: banpanel \[name or user guid\]|
|clearbluespacelockerlinks|Removes the bluespace links of the given uid\. Does not remove links this uid is the target of\.|Usage: clearbluespacelockerlinks \<storage uid\>|
|controlmob|Transfers user mind to the specified entity\.|Usage: controlmob \<mobUid\>\.|
|deadmin|Temporarily de\-admins you so you can experience the round as a normal player\.|Usage: deadmin<br>Use readmin to re\-admin after using this\.|
|deletecomponent|Deletes all instances of the specified component\.|Usage: deletecomponent \<name\>|
|departmentban|Bans a player from the roles comprising a department|Usage: departmentban \<name or user ID\> \<department\> \<reason\> \[duration in minutes, leave out or 0 for permanent ban\]|
|dirty|Marks all components on an entity as dirty, if not specified, dirties everything|Usage: dirty \[entityUid\]|
|dsay|Sends a message to deadchat as an admin|Usage: dsay \<message\>|
|explosionui|Opens a window for easy access to station destruction|Usage: explosionui|
|explosion|Train go boom|Usage: explosion \[intensity\] \[slope\] \[maxIntensity\] \[x y\] \[mapId\] \[prototypeId\]|
|faxui|Open admin window for sending faxes|Usage: faxui|
|follow|Makes you begin following an entity|Usage: follow \[netEntity\]|
|jobwhitelistadd|Lets a player play a whitelisted job\.|Usage: jobwhitelistadd \<username\> \<job\>|
|jobwhitelistget|Gets all the jobs that a player has been whitelisted for\.|Usage: jobwhitelistadd \<username\>|
|jobwhitelistremove|Removes a player's ability to play a whitelisted job\.|Usage: jobwhitelistadd \<username\> \<job\>|
|jobwhitelists|Opens the job whitelists window|Usage: jobwhitelists \[name or user guid\]|
|linkbluespacelocker|Links an entity, the target, to another as a bluespace locker target\.|Usage: linkbluespacelocker \<two\-way link\> \<origin storage uid\> \<target storage uid\>|
|loadgamemap|Loads the given game map at the given coordinates\.|loadgamemap \<mapid\> \<gamemap\> \[\<x\> \<y\> \[\<name\>\]\] |
|listgamemaps|Lists the game maps that can be used by loadgamemap|listgamemaps|
|adminlogs|Opens the admin logs panel\.|Usage: adminlogs|
|adminnotes|Opens the admin notes panel\.|Usage: adminnotes \<notedPlayerUserId OR notedPlayerUsername\>|
|permissions|Opens the admin permissions panel\.|Usage: permissions|
|adminremarks|Opens the admin remarks page|Usage: adminremarks|
|osay|||
|owoify|For when you need everything to be cat\. Uses OwOAccent's formatting on the name and description of an entity\.|owoify \<id\>|
|panicbunker|Toggles the panic bunker, which enables stricter restrictions on who's allowed to join the server\.|Usage: panicbunker|
|panicbunker_disable_with_admins|Toggles whether or not the panic bunker will disable when an admin connects\.|Usage: panicbunker\_disable\_with\_admins|
|panicbunker_enable_without_admins|Toggles whether or not the panic bunker will enable when the last admin disconnects\.|Usage: panicbunker\_enable\_without\_admins|
|panicbunker_count_deadminned_admins|Toggles whether or not to count deadminned admins when automatically enabling and disabling the panic bunker\.|Usage: panicbunker\_count\_deadminned\_admins|
|panicbunker_show_reason|Toggles whether or not to show connecting clients the reason why the panic bunker blocked them from joining\.|Usage: panicbunker\_show\_reason|
|panicbunker_min_account_age|Gets or sets the minimum account age in hours that an account must have to be allowed to connect with the panic bunker enabled\.|Usage: panicbunker\_min\_account\_age \<hours\>|
|panicbunker_min_overall_hours|Gets or sets the minimum overall playtime in hours that an account must have to be allowed to connect with the panic bunker enabled\.|Usage: panicbunker\_min\_overall\_hours \<hours\>|
|pardon|Pardons somebody's ban|Usage: pardon \<ban id\>|
|persistencesave|Saves server data to a persistence file to be loaded later\.|persistencesave \[mapId\] \[filePath \- default: game\.map \(CCVar\) \]|
|playerpanel|Displays general information and actions for a player|Usage: playerpanel \<name or user ID\>|
|playglobalsound|Plays a global sound for a specific player or for every connected player if no players are specified\.|playglobalsound \<path\> \[volume\] \[user 1\] \.\.\. \[user n\]|
|playtime_addoverall|Adds the specified minutes to a player's overall playtime|Usage: playtime\_addoverall \<user name\> \<minutes\>|
|playtime_addrole|Adds the specified minutes to a player's role playtime|Usage: playtime\_addrole \<user name\> \<role\> \<minutes\>|
|playtime_getoverall|Gets the specified minutes for a player's overall playtime|Usage: playtime\_getoverall \<user name\>|
|playtime_getrole|Gets all or one role timers from a player|Usage: playtime\_getrole \<user name\> \[role\]|
|playtime_save|Saves the player's playtimes to the DB|Usage: playtime\_save \<user name\>|
|playtime_flush|Flush active trackers to stored in playtime tracking\.|Usage: playtime\_flush \[user name\]<br>This causes a flush to the internal storage only, it does not flush to DB immediately\.<br>If a user is provided, only that user is flushed\.|
|playtime_unlock|Unlock the playtime requirement for specific jobs\.|Usage: playtime\_unlock \[user name\] \[trackers\.\.\.\]<br>This command unlocks the playtime requirements for specific jobs for a user\.|
|promotehost|Grants client temporary full host admin privileges\. Use this to bootstrap admins\.|Usage promotehost \<player\>|
|readmin|Re\-admins you if you previously de\-adminned\.|Usage: readmin|
|readyall|Readies up all players in the lobby, except for observers\.|readyall \\| ̣readyall \<ready\>|
|rmbodypart|Removes a given entity from it's containing body, if any\.|Usage: rmbodypart \<uid\>|
|rmstorage|Removes a given entity from it's containing storage, if any\.|Usage: rmstorage \<uid\>|
|removeextracomponents|Removes all components from all entities of the specified id if that component is not in its prototype\.<br>If no id is specified, it matches all entities\.|removeextracomponents \<entityId\> / removeextracomponents|
|rmmechanism|Removes a given entity from it's containing bodypart, if any\.|Usage: rmmechanism \<uid\>|
|roleban|Bans a player from a role|Usage: roleban \<name or user ID\> \<job\> \<reason\> \[duration in minutes, leave out or 0 for permanent ban\]|
|rolebanlist|Lists the user's role bans|Usage: \<name or user ID\> \[include unbanned\]|
|roleunban|Pardons a player's role ban|Usage: roleunban \<role ban id\>|
|setadminooc|Sets the color of your OOC messages\. Color must be in hex format, example: setadminooc \#c43b23|Usage: setadminooc \<color\>|
|setmind|Transfers a mind to the specified entity\. The entity must have a MindContainerComponent\. By default this will force minds that are currently visiting other entities to return \(i\.e\., return a ghost to their main body\)\.|Usage: setmind \<entityUid\> \<username\> \[unvisit\]|
|setoutfit|Sets the outfit of the specified entity\. The entity must have an InventoryComponent|Usage: setoutfit \<entityUid\> \\| setoutfit \<entityUid\> \<outfitId\>|
|setsolutioncapacity|Set the capacity \(maximum volume\) of some solution\.|Usage: setsolutioncapacity \<target\> \<solution\> \<new capacity\>|
|setsolutiontemperature|Set the temperature of some solution\.|Usage: setsolutiontemperature \<target\> \<solution\> \<new temperature\>|
|setsolutionthermalenergy|Set the thermal energy of some solution\.|Usage: setsolutionthermalenergy \<target\> \<solution\> \<new thermal energy\>|
|setstationainame|Sets a specific uid to be given a Station AI name at random\.|Usage: setstationainame \<entityUid\>|
|showghosts|makes all of the currently present ghosts visible\. Cannot be reversed\.|showghosts \<visible\>|
|callshuttle|Calls the emergency shuttle with an optionally provided arrival time\.|Usage: callshuttle \[m:ss\]|
|recallshuttle|Recalls the emergency shuttle\.|Usage: recallshuttle|
|stealthmin|Toggle whether others can see you in adminwho\.|Usage: stealthmin\\nUse stealthmin to toggle whether you appear in the output of the adminwho command\.|
|throwscoreboard|Show round\-end scoreboard for all players, but not finish the round|Usage: throwscoreboard|
|variantize|Randomizes all tile variants on a given grid\.|variantize \<grid id\>|
|warp|Teleports you to predefined areas on the map\.|warp \<location\><br>Locations you can teleport to are predefined by the map\. You can specify '?' as location to get a list of valid locations\.|
|pvs_override_info|Prints information about any PVS overrides associated with an entity\.|pvs\_override\_info|
|forceartifactnode|Forces an artifact to traverse to a given node|forceartifacteffect \<uid\> \<node ID\>|
|getartifactmaxvalue|Reports the maximum research point value for a given artifact|forceartifacteffect \<uid\>|
|applyworldgenconfig|Applies the given worldgen configuration to a map, setting it up for chunk loading/etc\.|applyworldgenconfig \<mapid\> \<prototype\>|
|weather|Sets the weather for the current map\.|weather \<mapId\> \<prototype / null\>|
|tippy|Broadcast a message as Tippy the clown\.|tippy \<user \\| all\> \<message\> \[entity prototype\] \[speak time\] \[slide time\] \[waddle interval\]|
|tip|Spawn a random game tip\.|tip|
|addcurrency|Adds currency to the specified store|addcurrency \<uid\> \<currency prototype\> \<amount\>|
|arrivals|||
|dungen|Generates a procedural dungeon with the specified preset, position, and seed\. Will spawn in space if the MapId doesn't have MapGridComponent\.|dungen \<MapId\> \<DungeonPreset\> \<PosX\> \<PosY\> \[seed\]|
|dungen_preset_vis|Generates a tile\-based preview of a dungeon preset\.|dungen\_preset\_vis \<mapid\> \<preset\>|
|dungen_pack_vis|Generates a tile\-based preview of a dungeon pack\.|dungen\_pack\_vis \<mapid\> \<pack\>|
|biome_clear|Clears a biome entirely|biome\_clear \<biomecomponent\>|
|biome_addlayer|Adds another biome layer|biome\_addlayer \<mapid\> \<biometemplate\> \[seed offset\]|
|biome_addmarkerlayer|Adds another biome marker layer|Adds another biome marker layer|
|toggleautosave|Toggles autosaving for a map\.|autosave \<map\> \<path if enabling\>|
|addtoband|||
|addgamerule||addgamerule \<rules\>|
|endgamerule||endgamerule \<rules\>|
|cleargamerules||cleargamerules|
|listgamerules||listgamerules \- Lists all rules that have been added for the round so far\.|
|appraisegrid|Calculates the total value of the given grids\.|appraisegrid \<grid Ids\>|
|fixgridatmos|Makes every tile on a grid have a roundstart gas mix\.|fixgridatmos \<grid Ids\>|
|pulseanomaly|Pulses a target anomaly|pulseanomaly \<uid\>|
|supercriticalanomaly|Makes a target anomaly go supercritical|supercriticalanomaly \<uid\>|
|addmap|Adds a new empty map to the round\. If the mapID already exists, this command does nothing\.|addmap \<mapID\> \[initialize\]|
|rmgrid|Removes a grid from a map\. You cannot remove the default grid\.|rmgrid \<gridId\>|
|mapinit|Runs map init on a map\.|mapinit \<mapID\>|
|lsmap|Lists maps\.|lsmap|
|lsgrid|Lists grids\.|lsgrid|
|tp|Teleports a player to any location in the round\.|tp \<x\> \<y\> \[\<mapID\>\]|
|tpto|Teleports the current player or the specified players/entities to the location of the first player/entity\.|tpto \<username\\|uid\> \[username\\|NetEntity\]\.\.\.|
|tpgrid|Teleports a grid to a new location\.|tpgrid \<gridId\> \<X\> \<Y\> \[\<MapId\>\]|
|cd|Changes the session's current directory to the given relative or absolute path\.|Usage:<br><br>  cd \<path \(ResPath\)\>|
|ls:here|Lists the contents of the current directory\.|Usage:<br><br>  ls:here \-\> IEnumerable\<ResPath\>|
|ls:in|Lists the contents of the given relative or absolute path\.|Usage:<br><br>  ls:in \<in \(ResPath\)\> \-\> IEnumerable\<ResPath\>|
|i|Integer constant\.|Usage:<br><br>  i \<value \(Int32\)\> \-\> Int32|
|f|Float constant\.|Usage:<br><br>  f \<value \(Single\)\> \-\> Single|
|s|String constant\.|Usage:<br><br>  s \<value \(String\)\> \-\> String|
|b|Bool constant\.|Usage:<br><br>  b \<value \(Boolean\)\> \-\> Boolean|
|ent|Returns the provided entity ID\.|Usage:<br><br>  ent \<uid \(EntityUid\)\> \-\> EntityUid|
|val|Casts the given value, block, or variable to the given type\. This is mostly a workaround for current limitations of variables\.|Usage:<br><br>  val \<value \(T\)\> \-\> T|
|var|Returns the contents of the given variable\. This will attempt to automatically infer a variables type\. Compound commands that modify a variable may need to use the 'val' command instead\.|Usage:<br><br>  var \<var \(VarRef\<T\>\)\> \-\> T|
|methods:get|Returns all methods associated with the input type\.|Usage:<br><br>  \<types \(IEnumerable\<Type\>\)\> \-\> methods:get \-\> IEnumerable\<MethodInfo\>|
|methods:overrides|Returns all methods overridden on the input type\.|Usage:<br><br>  \<types \(IEnumerable\<Type\>\)\> \-\> methods:overrides \-\> IEnumerable\<MethodInfo\>|
|methods:overridesfrom|Returns all methods overridden from the given type on the input type\.|Usage:<br><br>  \<types \(IEnumerable\<Type\>\)\> \-\> methods:overridesfrom \<t \(Type\)\> \-\> IEnumerable\<MethodInfo\>|
|self|Returns the current attached entity\.|Usage:<br><br>  self \-\> EntityUid|
|buildinfo|Provides information about the build of the game\.|Usage:<br><br>  buildinfo|
|cmd:list|Returns a list of all commands, for this side\.|Usage:<br><br>  cmd:list \-\> IEnumerable\<CommandSpec\>|
|cmd:moo|Asks the important questions\.|Usage:<br><br>  cmd:moo \-\> String|
|cmd:descloc|Returns the localization string for a command's description\.|Usage:<br><br>  \<cmd \(CommandSpec\)\> \-\> cmd:descloc \-\> String|
|cmd:info|Returns a CommandSpec for the given command\.<br>On its own, this means it'll print the command's help message\.|Usage:<br><br>  cmd:info \<cmd \(CommandSpec\)\> \-\> CommandSpec|
|cmd:getshim|Returns a command's execution shim\.|Usage:<br><br>  cmd:getshim \<block \(Block\)\> \-\> MethodInfo|
|explain|Explains the given expression, providing command descriptions and signatures\. This only works for valid expressions, it can't explain commands that it fails to parse\.|Usage:<br><br>  explain \<expr \(CommandRun\)\>|
|ioc:registered|Returns all the types registered with IoCManager on the current thread \(usually the game thread\)|Usage:<br><br>  ioc:registered \-\> IEnumerable\<Type\>|
|ioc:get|Gets an instance of an IoC registration\.|Usage:<br><br>  \<t \(Type\)\> \-\> ioc:get \-\> Object|
|loc:tryloc|Tries to get a localization string, returning null if unable\.|Usage:<br><br>  \<str \(String\)\> \-\> loc:tryloc \-\> String|
|loc:loc|Gets a localization string, returning the unlocalized string if unable\.|Usage:<br><br>  \<str \(String\)\> \-\> loc:loc \-\> String|
|more|Prints the contents of $more, i\.e\. any extras that Toolshed didn't print from the last command\.|Usage:<br><br>  more \-\> Object|
|physics:velocity|Returns the velocity of the input entities\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> physics:velocity \-\> IEnumerable\<Single\>|
|physics:parent|Returns the parent\(s\) of the input entities\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> physics:parent \-\> IEnumerable\<EntityUid\>|
|physics:angular_velocity|Returns the angular velocity of the given entities\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> physics:angular\_velocity \-\> IEnumerable\<Single\>|
|search|Searches through the input for the provided value\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> search \<term \(String\)\> \-\> IEnumerable\<FormattedMessage\>|
|stopwatch|Measures the execution time of the given expression\.|Usage:<br><br>  stopwatch \<expr \(CommandRun\)\> \-\> Object|
|types:consumers|Provides all commands that can consume the given type\.|Usage:<br><br>  \<input \(Object\)\> \-\> types:consumers|
|types:tree|Debug tool to return all types the command interpreter can downcast the input to\.|Usage:<br><br>  \<input \(Object\)\> \-\> types:tree \-\> IEnumerable\<Type\>|
|types:gettype|Returns the type of the input\.|Usage:<br><br>  \<input \(Object\)\> \-\> types:gettype \-\> Type|
|types:fullname|Returns the full name of the input type according to CoreCLR\.|Usage:<br><br>  \<input \(Type\)\> \-\> types:fullname \-\> String|
|+|Performs numeric addition\.|Usage:<br><br>  \<x \(T\)\> \-\> \+ \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \+ \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\><br><br>  \<x \(Vector2\)\> \-\> \+ \<y \(Vector2\)\> \-\> Vector2<br><br>  \<x \(IEnumerable\<Vector2\>\)\> \-\> \+ \<y \(IEnumerable\<Vector2\>\)\> \-\> IEnumerable\<Vector2\>|
|+/|Adds a scalar \(single value\) to every element in the input\.|Usage:<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \+/ \<y \(T\)\> \-\> IEnumerable\<T\><br><br>  \<x \(IEnumerable\<Vector2\>\)\> \-\> \+/ \<y \(Vector2\)\> \-\> IEnumerable\<Vector2\>|
|-|Performs numeric subtraction\.|Usage:<br><br>  \<x \(T\)\> \-\> \- \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \- \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\><br><br>  \<x \(Vector2\)\> \-\> \- \<y \(Vector2\)\> \-\> Vector2<br><br>  \<x \(IEnumerable\<Vector2\>\)\> \-\> \- \<y \(IEnumerable\<Vector2\>\)\> \-\> IEnumerable\<Vector2\>|
|-/|Subtracts a scalar \(single value\) from every element in the input\.|Usage:<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \-/ \<y \(T\)\> \-\> IEnumerable\<T\><br><br>  \<x \(IEnumerable\<Vector2\>\)\> \-\> \-/ \<y \(Vector2\)\> \-\> IEnumerable\<Vector2\>|
|*|Performs numeric multiplication\.|Usage:<br><br>  \<x \(T\)\> \-\> \* \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \* \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\><br><br>  \<x \(Vector2\)\> \-\> \* \<y \(Vector2\)\> \-\> Vector2<br><br>  \<x \(IEnumerable\<Vector2\>\)\> \-\> \* \<y \(IEnumerable\<Vector2\>\)\> \-\> IEnumerable\<Vector2\>|
|*/|Multiplies a scalar \(single value\) by every element in the input\.|Usage:<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \*/ \<y \(T\)\> \-\> IEnumerable\<T\><br><br>  \<x \(IEnumerable\<Vector2\>\)\> \-\> \*/ \<y \(Vector2\)\> \-\> IEnumerable\<Vector2\>|
|/|Performs numeric division\.|Usage:<br><br>  \<x \(T\)\> \-\> / \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> / \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|//|Divides every element in the input by a scalar \(single value\)\.|Usage:<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> // \<y \(T\)\> \-\> IEnumerable\<T\>|
|%|Computes the modulus of two values\.<br>This is usually remainder, check C\#'s documentation for the type\.|Usage:<br><br>  \<x \(T\)\> \-\> % \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> % \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|%/|Performs the modulus operation over the input with the given constant right\-hand value\.|Usage:<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> %/ \<y \(T\)\> \-\> IEnumerable\<T\>|
|min|Returns the minimum of two values\.|Usage:<br><br>  \<x \(T\)\> \-\> min \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> min \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|max|Returns the maximum of two values\.|Usage:<br><br>  \<x \(T\)\> \-\> max \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> max \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|&|Performs bitwise AND\.|Usage:<br><br>  \<x \(T\)\> \-\> & \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> & \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|&~|Performs bitwise AND\-NOT over the input\.|Usage:<br><br>  \<x \(T\)\> \-\> &~ \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> &~ \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|||Performs bitwise OR\.|Usage:<br><br>  \<x \(T\)\> \-\> \\| \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \\| \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
||~|Performs bitwise OR\-NOT over the input\.|Usage:<br><br>  \<x \(T\)\> \-\> \\|~ \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> \\|~ \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|^|Performs bitwise XOR\.|Usage:<br><br>  \<x \(T\)\> \-\> ^ \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> ^ \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|^~|Performs bitwise XNOR over the input\.|Usage:<br><br>  \<x \(T\)\> \-\> ^~ \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> ^~ \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|~|Performs bitwise NOT on the input\.|Usage:<br><br>  \<x \(T\)\> \-\> ~ \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> ~ \-\> IEnumerable\<T\>|
|neg|Negates the input\.|Usage:<br><br>  \<x \(T\)\> \-\> neg \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> neg \-\> IEnumerable\<T\>|
|abs|Computes the absolute value of the input \(removing the sign\)|Usage:<br><br>  \<x \(T\)\> \-\> abs \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> abs \-\> IEnumerable\<T\>|
|average|Computes the average \(arithmetic mean\) of the input\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> average \-\> T|
|bibytecount|Returns the size of the input in bytes, given that the input implements IBinaryInteger\.<br>This is NOT sizeof\.|Usage:<br><br>  \<x \(T\)\> \-\> bibytecount \-\> Int32<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> bibytecount \-\> IEnumerable\<Int32\>|
|shortestbitlength|Returns the minimum number of bits needed to represent the input value\.|Usage:<br><br>  \<x \(T\)\> \-\> shortestbitlength \-\> Int32<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> shortestbitlength \-\> IEnumerable\<Int32\>|
|countleadzeros|Counts the number of leading binary zeros in the input value\.|Usage:<br><br>  \<x \(T\)\> \-\> countleadzeros \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> countleadzeros \-\> IEnumerable\<T\>|
|counttrailingzeros|Counts the number of trailing binary zeros in the input value\.|Usage:<br><br>  \<x \(T\)\> \-\> counttrailingzeros \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> counttrailingzeros \-\> IEnumerable\<T\>|
|<|Performs a less\-than comparison, x \< y\.|Usage:<br><br>  \<x \(T\)\> \-\> \< \<y \(T\)\> \-\> Boolean|
|>=|Performs a greater\-than\-or\-equal comparison, x \>= y\.|Usage:<br><br>  \<x \(T\)\> \-\> \>= \<y \(T\)\> \-\> Boolean|
|<=|Performs a less\-than\-or\-equal comparison, x \<= y\.|Usage:<br><br>  \<x \(T\)\> \-\> \<= \<y \(T\)\> \-\> Boolean|
|==|Performs an equality comparison, returning true if the inputs are equal\.|Usage:<br><br>  \<x \(T\)\> \-\> == \<y \(T\)\> \-\> Boolean|
|!=|Performs an equality comparison, returning true if the inputs are not equal\.|Usage:<br><br>  \<x \(T\)\> \-\> \!= \<y \(T\)\> \-\> Boolean|
|fpi|pi \(3\.14159\.\.\.\) as a float\.|Usage:<br><br>  fpi \-\> Single|
|fe|e \(2\.71828\.\.\.\) as a float\.|Usage:<br><br>  fe \-\> Single|
|ftau|tau \(6\.28318\.\.\.\) as a float\.|Usage:<br><br>  ftau \-\> Single|
|fepsilon|The epsilon value for a float, exactly 1\.4e\-45\.|Usage:<br><br>  fepsilon \-\> Single|
|dpi|pi \(3\.14159\.\.\.\) as a double\.|Usage:<br><br>  dpi \-\> Double|
|de|e \(2\.71828\.\.\.\) as a double\.|Usage:<br><br>  de \-\> Double|
|dtau|tau \(6\.28318\.\.\.\) as a double\.|Usage:<br><br>  dtau \-\> Double|
|depsilon|The epsilon value for a double, exactly 4\.9406564584124654E\-324\.|Usage:<br><br>  depsilon \-\> Double|
|hpi|pi \(3\.14\.\.\.\) as a half\.|Usage:<br><br>  hpi \-\> Half|
|he|e \(2\.71\.\.\.\) as a half\.|Usage:<br><br>  he \-\> Half|
|htau|tau \(6\.28\.\.\.\) as a half\.|Usage:<br><br>  htau \-\> Half|
|hepsilon|The epsilon value for a half, exactly 5\.9604645E\-08\.|Usage:<br><br>  hepsilon \-\> Half|
|floor|Returns the floor of the input value \(rounding toward zero\)\.|Usage:<br><br>  \<x \(T\)\> \-\> floor \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> floor \-\> IEnumerable\<T\>|
|ceil|Returns the ceil of the input value \(rounding away from zero\)\.|Usage:<br><br>  \<x \(T\)\> \-\> ceil \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> ceil \-\> IEnumerable\<T\>|
|round|Rounds the input value\.|Usage:<br><br>  \<x \(T\)\> \-\> round \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> round \-\> IEnumerable\<T\>|
|trunc|Truncates the input value\.|Usage:<br><br>  \<x \(T\)\> \-\> trunc \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> trunc \-\> IEnumerable\<T\>|
|round2frac|Rounds the input value to the specified number of fractional digits\.|Usage:<br><br>  \<x \(T\)\> \-\> round2frac \<frac \(Int32\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> round2frac \<frac \(Int32\)\> \-\> IEnumerable\<T\>|
|exponentbytecount|Returns the number of bytes required to store the exponent\.|Usage:<br><br>  \<x \(T\)\> \-\> exponentbytecount \-\> Int32<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> exponentbytecount \-\> IEnumerable\<Int32\>|
|significandbytecount|Returns the number of bytes required to store the significand\.|Usage:<br><br>  \<x \(T\)\> \-\> significandbytecount \-\> Int32<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> significandbytecount \-\> IEnumerable\<Int32\>|
|significandbitcount|Returns the exact bit length of the significand\.|Usage:<br><br>  \<x \(T\)\> \-\> significandbitcount \-\> Int32<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> significandbitcount \-\> IEnumerable\<Int32\>|
|exponentshortestbitcount|Returns the minimum number of bits to store the exponent\.|Usage:<br><br>  \<x \(T\)\> \-\> exponentshortestbitcount \-\> Int32<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> exponentshortestbitcount \-\> IEnumerable\<Int32\>|
|stepnext|Steps to the next float value, adding one to the significand with carry\.|Usage:<br><br>  \<x \(T\)\> \-\> stepnext \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> stepnext \-\> IEnumerable\<T\>|
|stepprev|Steps to the previous float value, subtracting one from the significand with carry\.|Usage:<br><br>  \<x \(T\)\> \-\> stepprev \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> stepprev \-\> IEnumerable\<T\>|
|join|Joins two sequences together into one sequence\.|Usage:<br><br>  \<x \(String\)\> \-\> join \<y \(String\)\> \-\> String<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> join \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|append|Appends a value to the input enumerable\.|Usage:<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> append \<y \(T\)\> \-\> IEnumerable\<T\>|
|?|Replaces the input with the type's default value if it is null, albeit only for value types \(not objects\)\.|Usage:<br><br>  \<value \(Nullable\<TIn\>\)\> \-\> ? \<follower \(Block\<TIn,TOut\>\)\> \-\> TOut|
|or?|If the input is null, uses the provided alternate value\.|Usage:<br><br>  \<value \(T\)\> \-\> or? \<alternate \(ValueRef\<T\>\)\> \-\> T<br><br>  \<value \(Nullable\<T\>\)\> \-\> or? \<alternate \(ValueRef\<T\>\)\> \-\> T|
|??|Prints the given value transparently, for debug prints in a command run\.|Usage:<br><br>  \<value \(T\)\> \-\> ?? \-\> T<br><br>  \<value \(IEnumerable\<T\>\)\> \-\> ?? \-\> IEnumerable\<T\>|
|checkedto|Converts from the input numeric type to the target, erroring if not possible\.|Usage:<br><br>  \<x \(T\)\> \-\> checkedto \-\> TOut<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> checkedto \-\> IEnumerable\<TOut\>|
|saturateto|Converts from the input numeric type to the target, saturating if the value is out of range\.<br>For example, converting 382 to a byte would saturate to 255 \(the maximum value of a byte\)\.|Usage:<br><br>  \<x \(T\)\> \-\> saturateto \-\> TOut<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> saturateto \-\> IEnumerable\<TOut\>|
|truncto|Converts from the input numeric type to the target, with truncation\.<br>In the case of integers, this is a bit cast with sign extension\.|Usage:<br><br>  \<x \(T\)\> \-\> truncto \-\> TOut<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> truncto \-\> IEnumerable\<TOut\>|
|iscanonical|Returns whether the input is in canonical form\.|Usage:<br><br>  \<x \(T\)\> \-\> iscanonical \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> iscanonical \-\> IEnumerable\<Boolean\>|
|iscomplex|Returns whether the input is a complex number \(by value, not by type\)|Usage:<br><br>  \<x \(T\)\> \-\> iscomplex \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> iscomplex \-\> IEnumerable\<Boolean\>|
|iseven|Returns whether the input is even\.<br>Not a javascript package\.|Usage:<br><br>  \<x \(T\)\> \-\> iseven \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> iseven \-\> IEnumerable\<Boolean\>|
|isodd|Returns whether the input is odd\.|Usage:<br><br>  \<x \(T\)\> \-\> isodd \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isodd \-\> IEnumerable\<Boolean\>|
|isfinite|Returns whether the input is finite\.|Usage:<br><br>  \<x \(T\)\> \-\> isfinite \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isfinite \-\> IEnumerable\<Boolean\>|
|isimaginary|Returns whether the input is purely imaginary \(no real part\)\.|Usage:<br><br>  \<x \(T\)\> \-\> isimaginary \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isimaginary \-\> IEnumerable\<Boolean\><br><br>  \<x \(ICommonSession\)\> \-\> isimaginary \-\> Boolean|
|isinfinite|Returns whether the input is infinite\.|Usage:<br><br>  \<x \(T\)\> \-\> isinfinite \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isinfinite \-\> IEnumerable\<Boolean\>|
|isinteger|Returns whether the input is an integer \(by value, not by type\)|Usage:<br><br>  \<x \(T\)\> \-\> isinteger \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isinteger \-\> IEnumerable\<Boolean\>|
|isnan|Returns whether the input is Not a Number \(NaN\)\.<br>This is a special floating point value, so this is by value, not by type\.|Usage:<br><br>  \<x \(T\)\> \-\> isnan \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isnan \-\> IEnumerable\<Boolean\>|
|isnegative|Returns whether the input is negative\.|Usage:<br><br>  \<x \(T\)\> \-\> isnegative \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isnegative \-\> IEnumerable\<Boolean\>|
|ispositive|Returns whether the input is positive\.|Usage:<br><br>  \<x \(T\)\> \-\> ispositive \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> ispositive \-\> IEnumerable\<Boolean\>|
|isreal|Returns whether the input is purely real \(no imaginary part\)\.|Usage:<br><br>  \<x \(T\)\> \-\> isreal \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> isreal \-\> IEnumerable\<Boolean\><br><br>  \<x \(ICommonSession\)\> \-\> isreal \-\> Boolean|
|issubnormal|Returns whether the input is in sub\-normal form\.|Usage:<br><br>  \<x \(T\)\> \-\> issubnormal \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> issubnormal \-\> IEnumerable\<Boolean\>|
|iszero|Returns whether the input is zero\.|Usage:<br><br>  \<x \(T\)\> \-\> iszero \-\> Boolean<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> iszero \-\> IEnumerable\<Boolean\>|
|pow|Computes the power of its lefthand to its righthand\. x^y\.|Usage:<br><br>  \<x \(T\)\> \-\> pow \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> pow \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|rng:to|Returns a number between the input \(inclusive\) and the argument \(exclusive\)\.|Usage:<br><br>  \<from \(Int32\)\> \-\> rng:to \<to \(Int32\)\> \-\> Int32<br><br>  \<from \(Single\)\> \-\> rng:to \<to \(Single\)\> \-\> Single|
|rng:from|Returns a number between the argument \(inclusive\) and the input \(exclusive\)\)|Usage:<br><br>  \<to \(Int32\)\> \-\> rng:from \<from \(Int32\)\> \-\> Int32<br><br>  \<to \(Single\)\> \-\> rng:from \<from \(Single\)\> \-\> Single|
|rng:prob|Returns a boolean based on the input probability/chance \(from 0 to 1\)|Usage:<br><br>  \<prob \(Single\)\> \-\> rng:prob \-\> Boolean|
|sqrt|Computes the square root of its input\.|Usage:<br><br>  \<x \(T\)\> \-\> sqrt \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> sqrt \-\> IEnumerable\<T\>|
|cbrt|Computes the cube root of its input\.|Usage:<br><br>  \<x \(T\)\> \-\> cbrt \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> cbrt \-\> IEnumerable\<T\>|
|root|Computes the Nth root of its input\.|Usage:<br><br>  \<x \(T\)\> \-\> root \<y \(Int32\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> root \<y \(IEnumerable\<Int32\>\)\> \-\> IEnumerable\<T\>|
|hypot|Computes the hypotenuse of a triangle with the given sides A and B\.|Usage:<br><br>  \<x \(T\)\> \-\> hypot \<y \(T\)\> \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> hypot \<y \(IEnumerable\<T\>\)\> \-\> IEnumerable\<T\>|
|sum|Computes the sum of the input\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> sum \-\> T|
|sin|Computes the sine of the input\.|Usage:<br><br>  \<x \(T\)\> \-\> sin \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> sin \-\> IEnumerable\<T\>|
|sinpi|Computes the sine of the input multiplied by pi\.|Usage:<br><br>  \<x \(T\)\> \-\> sinpi \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> sinpi \-\> IEnumerable\<T\>|
|asin|Computes the arcsine of the input\.|Usage:<br><br>  \<x \(T\)\> \-\> asin \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> asin \-\> IEnumerable\<T\>|
|asinpi|Computes the arcsine of the input multiplied by pi\.|Usage:<br><br>  \<x \(T\)\> \-\> asinpi \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> asinpi \-\> IEnumerable\<T\>|
|cos|Computes the cosine of the input\.|Usage:<br><br>  \<x \(T\)\> \-\> cos \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> cos \-\> IEnumerable\<T\>|
|cospi|Computes the cosine of the input multiplied by pi\.|Usage:<br><br>  \<x \(T\)\> \-\> cospi \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> cospi \-\> IEnumerable\<T\>|
|acos|Computes the arcosine of the input\.|Usage:<br><br>  \<x \(T\)\> \-\> acos \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> acos \-\> IEnumerable\<T\>|
|acospi|Computes the arcosine of the input multiplied by pi\.|Usage:<br><br>  \<x \(T\)\> \-\> acospi \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> acospi \-\> IEnumerable\<T\>|
|tan|Computes the tangent of the input\.|Usage:<br><br>  \<x \(T\)\> \-\> tan \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> tan \-\> IEnumerable\<T\>|
|tanpi|Computes the tangent of the input multiplied by pi\.|Usage:<br><br>  \<x \(T\)\> \-\> tanpi \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> tanpi \-\> IEnumerable\<T\>|
|atan|Computes the arctangent of the input\.|Usage:<br><br>  \<x \(T\)\> \-\> atan \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> atan \-\> IEnumerable\<T\>|
|atanpi|Computes the arctangent of the input multiplied by pi\.|Usage:<br><br>  \<x \(T\)\> \-\> atanpi \-\> T<br><br>  \<x \(IEnumerable\<T\>\)\> \-\> atanpi \-\> IEnumerable\<T\>|
|any|Returns true if there's any values in the input, otherwise false\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> any \-\> Boolean|
|as|Casts the input to the given type\.<br>Effectively a type hint if you know the type but the interpreter does not\.|Usage:<br><br>  \<value \(TIn\)\> \-\> as \-\> TOut|
|contains|Returns whether the input enumerable contains the specified value\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> \[not\] contains \<value \(T\)\> \-\> Boolean|
|count|Counts the amount of entries in it's input, returning an integer\.|Usage:<br><br>  \<enumerable \(IEnumerable\<T\>\)\> \-\> count \-\> Int32|
|emplace|Runs the given block over it's inputs, with the input value placed into the variable $value within the block\.<br>Additionally breaks out $wx, $wy, $proto, $desc, $name, and $paused for entities\.<br>Can also have breakout values for other types, consult the documentation for that type for further info\.|Usage:<br><br>  \<value \(TIn\)\> \-\> emplace \<block \(Block\)\> \-\> TOut<br><br>  \<value \(IEnumerable\<TIn\>\)\> \-\> emplace \<block \(Block\)\> \-\> IEnumerable\<TOut\>|
|first|Returns the first entry of the given enumerable\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> first \-\> T|
|isempty|Returns true if the input is empty, otherwise false\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<input \(T\)\> \-\> \[not\] isempty \-\> Boolean|
|isnull|Returns true if the input is null, otherwise false\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<input \(Object\)\> \-\> \[not\] isnull \-\> Boolean|
|iterate|Iterates the given function over the input N times, returning a list of results\.<br>Think of this like successively applying the function to a value, tracking all the intermediate values\.|Usage:<br><br>  \<value \(T\)\> \-\> iterate \<block \(Block\<T,T\>\)\> \<times \(Int32\)\> \-\> IEnumerable\<T\>|
|map|Maps the input over the given block, with the provided expected return type\.<br>This command may be modified to not need an explicit return type in the future\.|Usage:<br><br>  \<value \(IEnumerable\<TIn\>\)\> \-\> map \<block \(Block\<TIn,TOut\>\)\> \-\> IEnumerable\<TOut\>|
|pick|Picks a random value from the input\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> pick \-\> T|
|reduce|Given a block to use as a reducer, turns a sequence into a single value\.<br>The left hand side of the block is implied, and the right hand is stored in $value\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> reduce \<reducer \(Block\)\> \-\> T|
|select|Selects N objects or N% of objects from the input\.<br>One can additionally invert this command with not to make it select everything except N objects instead\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<enumerable \(IEnumerable\<TR\>\)\> \-\> \[not\] select \<quantity \(Quantity\)\> \-\> IEnumerable\<TR\>|
|take|Takes N values from the input sequence|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> take \<amount \(Int32\)\> \-\> IEnumerable\<T\>|
|tee|Tees the input into the given block, ignoring the block's result\.<br>This essentially lets you have a branch in your code to do multiple operations on one value\.|Usage:<br><br>  \<value \(IEnumerable\<TIn\>\)\> \-\> tee \<block \(Block\<TIn,TOut\>\)\> \-\> IEnumerable\<TIn\>|
|unique|Filters the input sequence for uniqueness, removing duplicate values\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> unique \-\> IEnumerable\<T\>|
|where|Given some input sequence IEnumerable\<T\>, takes a block of signature T \-\> bool that decides if each input value should be included in the output sequence\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> where \<check \(Block\<T,Boolean\>\)\> \-\> IEnumerable\<T\>|
|=>|Assigns the input to a variable\.|Usage:<br><br>  \<input \(T\)\> \-\> =\> \<var \(WriteableVarRef\<T\>\)\> \-\> T<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> =\> \<var \(WriteableVarRef\<List\<T\>\>\)\> \-\> List\<T\>|
|vars|Provides a list of all variables set in this session\.|Usage:<br><br>  vars|
|bin|"Bins" the input, counting up how many times each unique element occurs\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> bin \-\> IDictionary\<T,Int32\>|
|extremes|Returns the two extreme ends of a list, interwoven\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> extremes \-\> IEnumerable\<T\>|
|sortby|Sorts the input least to greatest by the computed key\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> sortby \<orderer \(Block\<T,TOrd\>\)\> \-\> IEnumerable\<T\>|
|sort|Sorts the input least to greatest\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> sort \-\> IEnumerable\<T\>|
|sortdownby|Sorts the input greatest to least by the computed key\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> sortdownby \<orderer \(Block\<T,TOrd\>\)\> \-\> IEnumerable\<T\>|
|sortdown|Sorts the input greatest to least\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> sortdown \-\> IEnumerable\<T\>|
|sortmapby|Sorts the input least to greatest by the computed key, replacing the value with it's computed key afterward\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> sortmapby \<orderer \(Block\<T,TOrd\>\)\> \-\> IEnumerable\<TOrd\>|
|sortmapdownby|Sorts the input greatest to least by the computed key, replacing the value with it's computed key afterward\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> sortmapdownby \<orderer \(Block\<T,TOrd\>\)\> \-\> IEnumerable\<TOrd\>|
|iota|Returns a list of numbers 1 to N\.|Usage:<br><br>  \<count \(T\)\> \-\> iota \-\> IEnumerable\<T\>|
|rep|Repeats the input value N times to form a sequence\.|Usage:<br><br>  \<value \(T\)\> \-\> rep \<amount \(Int32\)\> \-\> IEnumerable\<T\>|
|to|Returns a list of numbers N to M\.|Usage:<br><br>  \<start \(T\)\> \-\> to \<end \(T\)\> \-\> IEnumerable\<T\>|
|curtick|The current game tick\.|Usage:<br><br>  curtick \-\> GameTick|
|curtime|The current game time \(a TimeSpan\)|Usage:<br><br>  curtime \-\> TimeSpan|
|realtime|The current realtime since startup \(a TimeSpan\)|Usage:<br><br>  realtime \-\> TimeSpan|
|servertime|The current server game time, or zero if we are the server \(a TimeSpan\)|Usage:<br><br>  servertime \-\> TimeSpan|
|delete|Deletes the input entities\.|Usage:<br><br>  \<entities \(IEnumerable\<EntityUid\>\)\> \-\> delete<br><br>  delete \<entity \(EntityUid\)\>|
|do|Backwards compatibility with BQL, applies the given old commands over the input sequence\.|Usage:<br><br>  \<input \(IEnumerable\<T\>\)\> \-\> do \<command \(String\)\> \-\> IEnumerable\<T\>|
|entities|Returns all entities on the server\.|Usage:<br><br>  entities \-\> IEnumerable\<EntityUid\>|
|named|Filters the input entities by their name, with the regex ^selector$\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> \[not\] named \<regex \(String\)\> \-\> IEnumerable\<EntityUid\>|
|nearby|Creates a new list of all entities nearby the inputs within the given range\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> nearby \<range \(Single\)\> \-\> IEnumerable\<EntityUid\>|
|paused|Filters the input entities by whether or not they are paused\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<entities \(IEnumerable\<EntityUid\>\)\> \-\> \[not\] paused \-\> IEnumerable\<EntityUid\>|
|prototyped|Filters the input entities by their prototype\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> \[not\] prototyped \<prototype \(EntProtoId\)\> \-\> IEnumerable\<EntityUid\>|
|replace|Replaces the input entities with the given prototype, preserving position and rotation \(but nothing else\)|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> replace \<prototype \(EntProtoId\)\> \-\> IEnumerable\<EntityUid\>|
|spawn:at|Spawns an entity at the given coordinates\.|Usage:<br><br>  \<target \(EntityCoordinates\)\> \-\> spawn:at \<proto \(EntProtoId\)\> \-\> EntityUid<br><br>  \<target \(IEnumerable\<EntityCoordinates\>\)\> \-\> spawn:at \<proto \(EntProtoId\)\> \-\> IEnumerable\<EntityUid\>|
|spawn:on|Spawns an entity on the given entity, at it's coordinates\.|Usage:<br><br>  \<target \(EntityUid\)\> \-\> spawn:on \<proto \(EntProtoId\)\> \-\> EntityUid<br><br>  \<target \(IEnumerable\<EntityUid\>\)\> \-\> spawn:on \<proto \(EntProtoId\)\> \-\> IEnumerable\<EntityUid\>|
|spawn:attached|Spawns an entity attached to the given entity, at \(0 0\) relative to it\.|Usage:<br><br>  \<target \(EntityUid\)\> \-\> spawn:attached \<proto \(EntProtoId\)\> \-\> EntityUid<br><br>  \<target \(IEnumerable\<EntityUid\>\)\> \-\> spawn:attached \<proto \(EntProtoId\)\> \-\> IEnumerable\<EntityUid\>|
|with|Filters the input entities by whether or not they have the given component\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> \[not\] with \<component \(Type\)\> \-\> IEnumerable\<EntityUid\><br><br>  \<input \(IEnumerable\<EntityPrototype\>\)\> \-\> \[not\] with \<component \(Type\)\> \-\> IEnumerable\<EntityPrototype\><br><br>  \<input \(IEnumerable\<ProtoId\<T\>\>\)\> \-\> \[not\] with \<protoId \(ProtoId\<T\>\)\> \-\> IEnumerable\<ProtoId\<T\>\>|
|mappos|Returns an entity's coordinates relative to it's current map\.|Usage:<br><br>  \<ent \(EntityUid\)\> \-\> mappos \-\> EntityCoordinates<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> mappos \-\> IEnumerable\<EntityCoordinates\>|
|pos|Returns an entity's coordinates\.|Usage:<br><br>  \<ent \(EntityUid\)\> \-\> pos \-\> EntityCoordinates<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> pos \-\> IEnumerable\<EntityCoordinates\><br><br>  pos \-\> EntityCoordinates|
|tp:coords|Teleports the target to the given coordinates\.|Usage:<br><br>  \<teleporter \(EntityUid\)\> \-\> tp:coords \<target \(EntityCoordinates\)\> \-\> EntityUid<br><br>  \<teleporters \(IEnumerable\<EntityUid\>\)\> \-\> tp:coords \<target \(EntityCoordinates\)\> \-\> IEnumerable\<EntityUid\>|
|tp:to|Teleports the target to the given other entity\.|Usage:<br><br>  \<teleporter \(EntityUid\)\> \-\> tp:to \<target \(EntityUid\)\> \-\> EntityUid<br><br>  \<teleporters \(IEnumerable\<EntityUid\>\)\> \-\> tp:to \<target \(EntityUid\)\> \-\> IEnumerable\<EntityUid\>|
|tp:into|Teleports the target "into" the given other entity, attaching it at \(0 0\) relative to it\.|Usage:<br><br>  \<teleporter \(EntityUid\)\> \-\> tp:into \<target \(EntityUid\)\> \-\> EntityUid<br><br>  \<teleporters \(IEnumerable\<EntityUid\>\)\> \-\> tp:into \<target \(EntityUid\)\> \-\> IEnumerable\<EntityUid\>|
|allcomps|Returns all components on the given entity\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> allcomps \-\> IEnumerable\<IComponent\>|
|comp:get|Gets the given component from the given entity\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> comp:get \-\> IEnumerable\<T\><br><br>  \<input \(EntityUid\)\> \-\> comp:get \-\> T|
|comp:add|Adds the given component to the given entity\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> comp:add \-\> EntityUid<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> comp:add \-\> IEnumerable\<EntityUid\>|
|comp:rm|Removes the given component from the entity\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> comp:rm \-\> EntityUid<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> comp:rm \-\> IEnumerable\<EntityUid\>|
|comp:ensure|Ensures the given entity has the given component\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> comp:ensure \-\> EntityUid<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> comp:ensure \-\> IEnumerable\<EntityUid\>|
|comp:has|Check if the given entity has the given component\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> comp:has \-\> Boolean<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> comp:has \-\> IEnumerable\<Boolean\>|
|entitysystemupdateorder:tick|Lists the tick update order of entity systems\.|Usage:<br><br>  entitysystemupdateorder:tick \-\> IEnumerable\<Type\>|
|entitysystemupdateorder:frame|Lists the frame update order of entity systems\.|Usage:<br><br>  entitysystemupdateorder:frame \-\> IEnumerable\<Type\>|
|actor:controlled|Filters entities by whether or not they're actively controlled\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> actor:controlled \-\> IEnumerable\<EntityUid\>|
|actor:session|Returns the sessions associated with the input entities\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> actor:session \-\> IEnumerable\<ICommonSession\>|
|player:list|Returns a list of all player sessions\.|Usage:<br><br>  player:list \-\> IEnumerable\<ICommonSession\>|
|player:self|Returns the current player session\.|Usage:<br><br>  player:self \-\> ICommonSession|
|player:imm|Returns the session associated with the player given as argument\.|Usage:<br><br>  player:imm \<username \(String\)\> \-\> ICommonSession|
|player:entity|Returns the entities of the input sessions\.|Usage:<br><br>  \<sessions \(IEnumerable\<ICommonSession\>\)\> \-\> player:entity \-\> IEnumerable\<EntityUid\><br><br>  \<sessions \(ICommonSession\)\> \-\> player:entity \-\> EntityUid<br><br>  player:entity \<username \(String\)\> \-\> EntityUid|
|visualize|Takes the input list of entities and puts them into a UI window for easy browsing\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> visualize|
|runverbas|Runs a verb over the input entities with the given user\.|Usage:<br><br>  \<input \(IEnumerable\<NetEntity\>\)\> \-\> runverbas \<runner \(EntityUid\)\> \<verb \(String\)\> \-\> IEnumerable\<NetEntity\>|
|acmd:perms|Returns the admin permissions of the given command, if any\.|Usage:<br><br>  \<command \(CommandSpec\)\> \-\> acmd:perms \-\> AdminFlags\[\]|
|acmd:caninvoke|Check if the given player can invoke the given command\.|Usage:<br><br>  \<command \(CommandSpec\)\> \-\> acmd:caninvoke \<player \(ICommonSession\)\> \-\> Boolean|
|laws:list|Returns a list of all law bound entities\.|Usage:<br><br>  laws:list \-\> IEnumerable\<EntityUid\>|
|laws:get|Returns all of the laws for a given entity\.|Usage:<br><br>  \<lawbound \(EntityUid\)\> \-\> laws:get \-\> IEnumerable\<String\>|
|polymorph|Polymorphs the input entity with the given prototype\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> polymorph \<protoId \(ProtoId\<PolymorphPrototype\>\)\> \-\> Nullable\<EntityUid\><br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> polymorph \<protoId \(ProtoId\<PolymorphPrototype\>\)\> \-\> IEnumerable\<EntityUid\>|
|unpolymorph|Reverts a polymorph\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> unpolymorph \-\> Nullable\<EntityUid\><br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> unpolymorph \-\> IEnumerable\<EntityUid\>|
|stationevent:simulate|Simulates N number of rounds in which events will occur and prints the occurrences of every event after\.|Usage:<br><br>  stationevent:simulate \<eventScheduler \(EntityPrototype\)\> \<rounds \(Int32\)\> \<playerCount \(Int32\)\> \<roundEndMean \(Single\)\> \<roundEndStdDev \(Single\)\> \-\> IEnumerable\<ValueTuple\<String,Single\>\>|
|stationevent:lsprob|Lists the probability of different station events occuring out of the entire pool\.|Usage:<br><br>  stationevent:lsprob \<eventScheduler \(EntityPrototype\)\> \-\> IEnumerable\<ValueTuple\<String,Single\>\>|
|stationevent:lsprobtime|Lists the probability of different station events occuring based on the specified length of a round\.|Usage:<br><br>  stationevent:lsprobtime \<eventScheduler \(EntityPrototype\)\> \<time \(Single\)\> \-\> IEnumerable\<ValueTuple\<String,Single\>\>|
|stationevent:prob|Returns the probability of a single station event occuring out of the entire pool\.|Usage:<br><br>  stationevent:prob \<eventScheduler \(EntityPrototype\)\> \<eventId \(String\)\> \-\> Single|
|mind:get|Grabs the mind from the entity, if any\.|Usage:<br><br>  \<session \(ICommonSession\)\> \-\> mind:get \-\> MindComponent<br><br>  \<ent \(EntityUid\)\> \-\> mind:get \-\> MindComponent|
|mind:control|Assumes control of an entity with the given player\.|Usage:<br><br>  \<target \(EntityUid\)\> \-\> mind:control \<player \(ICommonSession\)\> \-\> EntityUid|
|language:add|Adds a new language to the piped entity\. The two last arguments indicate whether it should be spoken/understood\. Example: 'self language:add "Canilunzt" true true'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> language:add \<language \(ProtoId\<LanguagePrototype\>\)\> \<canSpeak \(Boolean\)\> \<canUnderstand \(Boolean\)\> \-\> EntityUid|
|language:rm|Removes a language from the piped entity\. Works similarly to language:add\. Example: 'self language:rm "TauCetiBasic" true true'\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> language:rm \<language \(ProtoId\<LanguagePrototype\>\)\> \<removeSpeak \(Boolean\)\> \<removeUnderstand \(Boolean\)\> \-\> EntityUid|
|language:lsspoken|Lists all languages the entity can speak\. Example: 'self language:lsspoken'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> language:lsspoken \-\> IEnumerable\<ProtoId\<LanguagePrototype\>\>|
|language:lsunderstood|Lists all languages the entity can understand\. Example: 'self language:lssunderstood'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> language:lsunderstood \-\> IEnumerable\<ProtoId\<LanguagePrototype\>\>|
|translator:addlang|Adds a new target language to the piped translator entity\. See language:add for details\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> translator:addlang \<language \(ProtoId\<LanguagePrototype\>\)\> \<addSpeak \(Boolean\)\> \<addUnderstand \(Boolean\)\> \-\> EntityUid|
|translator:rmlang|Removes a target language from the piped translator entity\. See language:rm for details\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> translator:rmlang \<language \(ProtoId\<LanguagePrototype\>\)\> \<removeSpeak \(Boolean\)\> \<removeUnderstand \(Boolean\)\> \-\> EntityUid|
|translator:addrequired|Adds a new required language to the piped translator entity\. Example: 'ent 1234 translator:addrequired "TauCetiBasic"'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> translator:addrequired \<language \(ProtoId\<LanguagePrototype\>\)\> \-\> EntityUid|
|translator:rmrequired|Removes a required language from the piped translator entity\. Example: 'ent 1234 translator:rmrequired "TauCetiBasic"'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> translator:rmrequired \<language \(ProtoId\<LanguagePrototype\>\)\> \-\> EntityUid|
|translator:lsspoken|Lists all spoken languages for the piped translator entity\. Example: 'ent 1234 translator:lsspoken'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> translator:lsspoken \-\> IEnumerable\<ProtoId\<LanguagePrototype\>\>|
|translator:lsunderstood|Lists all understood languages for the piped translator entity\. Example: 'ent 1234 translator:lssunderstood'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> translator:lsunderstood \-\> IEnumerable\<ProtoId\<LanguagePrototype\>\>|
|translator:lsrequired|Lists all required languages for the piped translator entity\. Example: 'ent 1234 translator:lsrequired'|Usage:<br><br>  \<input \(EntityUid\)\> \-\> translator:lsrequired \-\> IEnumerable\<ProtoId\<LanguagePrototype\>\>|
|jobs:jobs|Returns all jobs on a station\.|Usage:<br><br>  \<station \(EntityUid\)\> \-\> jobs:jobs \-\> IEnumerable\<JobSlotRef\><br><br>  \<stations \(IEnumerable\<EntityUid\>\)\> \-\> jobs:jobs \-\> IEnumerable\<JobSlotRef\>|
|jobs:job|Returns a given job on a station\.|Usage:<br><br>  \<station \(EntityUid\)\> \-\> jobs:job \<job \(ProtoId\<JobPrototype\>\)\> \-\> JobSlotRef<br><br>  \<stations \(IEnumerable\<EntityUid\>\)\> \-\> jobs:job \<job \(ProtoId\<JobPrototype\>\)\> \-\> IEnumerable\<JobSlotRef\>|
|jobs:isinfinite|Returns true if the input job is infinite, otherwise false\.|The behaviour of this command can be inverted using the "not" prefix\.<br><br>Usage:<br><br>  \<job \(JobSlotRef\)\> \-\> \[not\] jobs:isinfinite \-\> Boolean<br><br>  \<jobs \(IEnumerable\<JobSlotRef\>\)\> \-\> \[not\] jobs:isinfinite \-\> IEnumerable\<Boolean\>|
|jobs:adjust|Adjusts the number of slots for the given job\.|Usage:<br><br>  \<ref \(JobSlotRef\)\> \-\> jobs:adjust \<by \(Int32\)\> \-\> JobSlotRef<br><br>  \<ref \(IEnumerable\<JobSlotRef\>\)\> \-\> jobs:adjust \<by \(Int32\)\> \-\> IEnumerable\<JobSlotRef\>|
|jobs:set|Sets the number of slots for the given job\.|Usage:<br><br>  \<ref \(JobSlotRef\)\> \-\> jobs:set \<by \(Int32\)\> \-\> JobSlotRef<br><br>  \<ref \(IEnumerable\<JobSlotRef\>\)\> \-\> jobs:set \<by \(Int32\)\> \-\> IEnumerable\<JobSlotRef\>|
|jobs:amount|Returns the number of slots for the given job\.|Usage:<br><br>  \<ref \(JobSlotRef\)\> \-\> jobs:amount \-\> UInt32<br><br>  \<ref \(IEnumerable\<JobSlotRef\>\)\> \-\> jobs:amount \-\> IEnumerable\<UInt32\>|
|stations:list|Returns a list of all stations\.|Usage:<br><br>  stations:list \-\> IEnumerable\<EntityUid\>|
|stations:get|Gets the active station, if and only if there is only one\.|Usage:<br><br>  stations:get \-\> EntityUid|
|stations:getowningstation|Gets the station that a given entity is "owned by" \(within\)|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> stations:getowningstation \-\> IEnumerable\<Nullable\<EntityUid\>\><br><br>  \<input \(EntityUid\)\> \-\> stations:getowningstation \-\> Nullable\<EntityUid\>|
|stations:largestgrid|Returns the largest grid the given station has, if any\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> stations:largestgrid \-\> Nullable\<EntityUid\><br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> stations:largestgrid \-\> IEnumerable\<Nullable\<EntityUid\>\>|
|stations:grids|Returns all grids associated with the input station\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> stations:grids \-\> IEnumerable\<EntityUid\><br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> stations:grids \-\> IEnumerable\<EntityUid\>|
|stations:config|Returns the config associated with the input station, if any\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> stations:config \-\> StationConfig<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> stations:config \-\> IEnumerable\<StationConfig\>|
|stations:addgrid|Adds a grid to the given station\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> stations:addgrid \<grid \(EntityUid\)\>|
|stations:rmgrid|Removes a grid from the given station\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> stations:rmgrid \<grid \(EntityUid\)\>|
|stations:rename|Renames the given station\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> stations:rename \<name \(String\)\>|
|stations:rerollBounties|Clears all the current bounties for the station and gets a new selection\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> stations:rerollBounties|
|deletechatmessage:id|Delete a specific chat message by message ID|Usage:<br><br>  deletechatmessage:id \<messageId \(UInt32\)\>|
|nukechatmessages:usernames|Delete all of the supplied usernames' chat messages posted during this round|Usage:<br><br>  nukechatmessages:usernames \<usernamesCsv \(String\)\>|
|admins:active|Returns a list of active admins\.|Usage:<br><br>  admins:active \-\> IEnumerable\<ICommonSession\>|
|admins:all|Returns a list of ALL admins, including deadmined ones\.|Usage:<br><br>  admins:all \-\> IEnumerable\<ICommonSession\>|
|marked|Returns the value of $marked as a List\<EntityUid\>\.|Usage:<br><br>  marked \-\> IEnumerable\<EntityUid\>|
|rejuvenate|Rejuvenates the given entities, restoring them to full health, clearing status effects, etc\.|Usage:<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> rejuvenate \-\> IEnumerable\<EntityUid\><br><br>  rejuvenate|
|solution:get|Grabs the given solution off the given entity\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> solution:get \<name \(String\)\> \-\> Nullable\<SolutionRef\><br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> solution:get \<name \(String\)\> \-\> IEnumerable\<SolutionRef\>|
|solution:adjreagent|Adjusts the given reagent on the given solution\.|Usage:<br><br>  \<input \(SolutionRef\)\> \-\> solution:adjreagent \<proto \(ProtoId\<ReagentPrototype\>\)\> \<amount \(FixedPoint2\)\> \-\> SolutionRef<br><br>  \<input \(IEnumerable\<SolutionRef\>\)\> \-\> solution:adjreagent \<name \(ProtoId\<ReagentPrototype\>\)\> \<amount \(FixedPoint2\)\> \-\> IEnumerable\<SolutionRef\>|
|tag:list|Lists tags on the given entities\.|Usage:<br><br>  \<ent \(IEnumerable\<EntityUid\>\)\> \-\> tag:list \-\> IEnumerable\<ProtoId\<TagPrototype\>\>|
|tag:add|Adds a tag to the given entities\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> tag:add \<tag \(ProtoId\<TagPrototype\>\)\> \-\> EntityUid<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> tag:add \<tag \(ProtoId\<TagPrototype\>\)\> \-\> IEnumerable\<EntityUid\>|
|tag:rm|Removes a tag from the given entities\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> tag:rm \<tag \(ProtoId\<TagPrototype\>\)\> \-\> EntityUid<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> tag:rm \<tag \(ProtoId\<TagPrototype\>\)\> \-\> IEnumerable\<EntityUid\>|
|tag:addmany|Adds a list of tags to the given entities\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> tag:addmany \<tags \(IEnumerable\<ProtoId\<TagPrototype\>\>\)\> \-\> EntityUid<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> tag:addmany \<tags \(IEnumerable\<ProtoId\<TagPrototype\>\>\)\> \-\> IEnumerable\<EntityUid\>|
|tag:rmmany|Removes a list of tags from the given entities\.|Usage:<br><br>  \<input \(EntityUid\)\> \-\> tag:rmmany \<tags \(IEnumerable\<ProtoId\<TagPrototype\>\>\)\> \-\> EntityUid<br><br>  \<input \(IEnumerable\<EntityUid\>\)\> \-\> tag:rmmany \<tags \(IEnumerable\<ProtoId\<TagPrototype\>\>\)\> \-\> IEnumerable\<EntityUid\>|
|addaccesslog|Adds an access log to this entity\. Do note that this bypasses the log's default limit and pause check\.|Usage:<br><br>  addaccesslog \<input \(EntityUid\)\> \<seconds \(Single\)\> \<accessor \(String\)\><br><br>  \<input \(EntityUid\)\> \-\> addaccesslog \<seconds \(Single\)\> \<accessor \(String\)\>|
