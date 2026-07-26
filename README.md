# C-Sonic-the-hedgehog
Sonic Forces — OOP
Object-Oriented Programming semester project: a 2D Sonic platformer in C++ with SFML, featuring the classic trio — Sonic, Tails, and Knuckles — with enemies, rings, obstacles, boosters, multiple levels, and a persistent leaderboard.

All game code lives in Code/Source.cpp; sprites, audio, and the font are under Data/.

Features
Three playable characters with distinct abilities:
Sonic — speed and jumps
Tails — flight (dedicated fly animation frames)
Knuckles — wall-breaking with reach and cooldown mechanics
Followers trail the leader with smooth lerp-based following
Enemy roster — BatBrain (with projectiles), BeeBot, Crabmeat, MotoBug, plus a boss fight (Boss.ogg)
Collectibles & hazards — rings, spikes, obstacles, item boxes, and boosters
Level system — multiple themed levels (including an ice stage) with per-level score targets and a level timer
Leaderboard — high scores persisted to Code/leaderboard.txt
Audio — background themes per stage and sound effects for jumps, rings, spikes, and switches
Design
The project is fully class-driven (per OOP course requirements): Game, GameMechanics, Level, Player/Tails/Knuckles, an Enemy hierarchy with an EnemyManager, plus managers for rings, obstacles, items, boosters, audio, and scoring.

Building
Requires SFML (graphics, window, audio):

g++ Code/Source.cpp -o sonic-forces -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
./sonic-forces
Run from the repo root so the assets in Data/ load correctly.
