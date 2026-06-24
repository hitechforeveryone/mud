# AxiomMUD Engine

## Current Version 07028

* Java code-base, flat-file data storage.

AxiomMUD is a classic-style, systems-heavy multiplayer text RPG engine built around persistent worlds, dynamic simulation, immersive roleplay mechanics, and modular content creation tools. The engine follows the philosophy of old-school sandbox MUDs while introducing modernized internal systems, cleaner abstractions, and extensible architecture.

The engine is designed to support multiple persistent worlds. Individual worlds, such as the current Tithrius world implementation, are built using the engine's systems for zones, rooms, NPCs, objects, scripts, combat, and environmental simulation.

At its core, AxiomMUD models worlds as interconnected zones and rooms featuring dynamic weather, seasonal changes, lighting systems, scripted events, wandering NPCs, and cross-zone travel. Rooms support environmental effects, directional exits, doors, and layered atmospheric mechanics that influence exploration and gameplay.

The combat system is tick-based and supports melee combat, spellcasting, abilities, status effects, AoE effects, directional attacks, threat management, and reactive combat hooks. Effects are highly modular, allowing buffs, debuffs, room effects, movement restrictions, spell interception, damage reflection, and stat modification through a unified effect framework.

Professions define gameplay identity, with systems supporting spellcasters, martial combatants, and specialized archetypes. The Bard profession uses a unique maintained-song system rather than traditional spellcasting. 

AxiomMUD includes extensive builder and administration tooling:

* World editors
* Zone editors
* Room editors
* Mob and player editors
* Object editors
* Help file systems
* Scripted triggers/events
* Cross-zone exit creation
* Searchable help indexes
* Dynamic mob behavior configuration

NPC AI is behavior-flag driven, allowing mobs to cast spells, sing songs, patrol areas, defend territory, retaliate intelligently, and respond to environmental or scripted conditions.

The Tithrius world built on top of AxiomMUD emphasizes atmosphere, mystery, and immersive exploration rather than purely mechanical progression. Regions such as the Misty Forest, Dagger Hills, and Withering Woods are designed with distinct environmental identities and interconnected lore.

Technically, AxiomMUD is designed as an object-oriented and extensible engine:

* Spells, Songs, Effects, and Behaviors are modularized
* Tick systems drive persistence and world simulation
* Effects self-register and self-cleanup
* Content is separated from core engine systems
* Architecture supports future worlds, professions, mechanics, and expansions

Overall, AxiomMUD is a modern reinterpretation of classic Diku/Circle-style MUD design philosophy, focusing on systemic cohesion, maintainable architecture, and immersive persistent-world simulation rather than purely combat grinding.

## Please Compile to Run/Play

* `/src/server/Server.java` - Runs the AxiomMUD server that clients connect to. Requires Read/Write permissions for file operations including player saves, world creation/editing, zones, rooms, mobs, objects, and scripts.

* `/src/client/Client.java` - Optional command-line client for connecting and playing through a terminal or IDE console.
