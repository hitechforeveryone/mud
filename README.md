## Current Version 7025

* Java code-base, flat-file data storage. 

This JAVA-based MUD project is a classic-style, systems-heavy multiplayer text RPG built around persistent worlds, dynamic combat, immersive roleplay mechanics, and deeply modular content creation tools. The design philosophy leans toward old-school sandbox MUDs, but with modernized internal systems and cleaner extensibility.

At its core, the game world is composed of interconnected worlds, zones, and rooms featuring dynamic weather, seasonal changes, lighting systems, scripted events, wandering NPCs, and cross-zone travel. Rooms can contain environmental effects, directional exits, doors, and layered atmospheric mechanics that affect gameplay and exploration.

The combat system is tick-based and supports melee combat, spellcasting, abilities, status effects, AoE effects, directional attacks, threat management, and reactive combat hooks. Effects are highly modular, allowing buffs, debuffs, room effects, movement restrictions, spell interception, damage reflection, and stat modification through a unified effect framework.

Professions define gameplay identity, with systems already supporting spellcasters (both damage and healing types), martial abilities, and a Bard archetypes.  Bards are built around persistent songs rather than traditional spellcasting. Bard songs function as maintained effects powered by a voice resource system, enabling party buffs, debuffs, battlefield control, illumination, silence effects, and morale-based support mechanics.

The project also includes extensive builder and administration tooling:

* World, Zone, Room editors
* Mob/Player editors
* Object editors
* Help file systems
* Scripted triggers/events
* Cross-zone exit creation
* Searchable help indexes
* Dynamic mob behaviors such as sentries, wandering, and combat AI

NPC AI is behavior-flag driven, allowing mobs to cast spells, sing songs, patrol, defend areas, retaliate intelligently, and respond to environmental or scripted conditions.

Narratively, the world emphasizes atmosphere, mystery, and immersive exploration rather than purely mechanical progression. The setting of Tithrius includes regions such as the Misty Forest, Dagger Hills, and Withering Woods, each designed with environmental identity and interconnected lore.

Technically, the architecture is highly object-oriented and extensible:

* Spells, Songs, Effects, and Behaviors are modularized
* Tick systems drive persistence and world simulation
* Effects self-register and self-cleanup
* Systems are designed for future professions, mechanics, and content expansion

Overall, the project feels like a modern reinterpretation of classic Diku/Circle-style MUD design philosophy, but with stronger systemic cohesion, cleaner abstractions, and a focus on immersive persistent-world simulation rather than purely combat grinding.


## Please Compile to Run/play
* /src/server/Server.java - This is the server that runs the MUD and that clients may connect to. Requires Read/Write privs on your server for File I/O (player saves, new/edit worlds, zones, rooms, mobs, objs, scripts)
* /src/client/Client.java - optional, to play from your commandline or IDE console.
