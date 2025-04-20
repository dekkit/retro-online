WORK IN PROGRESS - This will be expanded over time (Last Update - 20/04/25)

# retro-online
A collection of notes and experiences for playing retro games online via emulators.
This will evolve based on continued experiences and discovery of better options (take note of the date/time stamp when referring any specific items).

**Why this Document**

When a few friends and I decided to explore playing retro games online more regularly, we were keen to explore what options were available and what gaming systems worked best, particularly for games that supported 2 players or more.

While retro computer / retro video console emulation quality has improved drastically in the past 10-20 years, most emulators with netplay are not easy to setup and users need an undertstanding basic computer networking concepts (e.g. IP Addresses, Ports, Port Forwarding, and protocols like TCP/UDP) in order to get things running smoothly.

Below aims to provides some of basics and an idea of what to expect.

**Types of Multiplayer**

Multiplayer games can refer many different styles.  To briefly summarise:

_**Local Multiplayer**_ 

Traditionally this would involve all player being in the same room (i.e. same physical location) and all sitting / huddled around the same console or computer (**ie. Same Device**)

- **Split Screen** - All players share the same screen and device and the screen is split in half or quarters -  either 2 or 4 players can play at the same time (Examples: Super Mario Kart / Mario Kart 64 / Crash Team Racing, Burnout Revenge etc)
- **Single Screen (Same time)** - All players share the same screen and device, typically 2+ players can play at the same time each taking on playable character(Examples: Simpsons Arcade, TMNT, Double Dragon, Bubble Bobble, Smash Bros etc)
- **Single Screen (Alternating)** - All players share the same screen and device, each player take a turn to play (usually until they met a goal or lose a live), then the next player will take a turn to play (Examples: Galaga, Frogger, Super Mario Brothers 1, Summer Games etc).

_**Linked Multiplayer**_ 

As technology evolved,  additional methods of communicating between systems emerged.   This meant that players no longer needed be on the same device (in some cases not even in the same room or physical location), instead they could have their own device (**ie. Different Devices that are Linked**).

- **Comm / Serial / Parallel / Modem** - Each player has their own device and screen which was typically connected via a communication cable or modem - typically a max of 2 players although greater numbers were possible (Examples: Tetris via GameBoy Link / Need for Speed 1 via Null Modem Cable)
- **Local LAN** - Each player has their own device and screen which was typically connected via a local area network (LAN) device and cable in the same physical location - this could have any number of players cabled or wirelessly connected in the same location (Examples: Doom, Duke3d, WarCraft 2 etc) 

_**Online Multiplayer**_ 

As the internet took off, multiplayer gaming was taken in new amazing directions  -  you can now game anywhere with any number of players using a variety of different connectivity options both wired and wirelessly (**ie. Different Devices Connected via the Internet**).

- **Internet** - Each player has their own device, screen and connection to the internet, and typically a installation of the game on the players device (Examples: World of Warcraft, Counter Strike, Fortnite, Minecraft  etc etc etc)
- **Cloud / Streaming** - Each player has their own device and screen and connection to the internet, howeever the game is stored and operated remotely on another computer with the video output streamed to each player  (Examples: AntStream, Xbox Cloud)


_Emulation Challenges_
- Many early games were simply never designed to support remote players - emulation developers have to design methods to keep copies of a single console in sync across multiple locations.
- Linked games are very sensitive to data delays, as the fast as modern internet can be, any delays can cause link games to get out of sync.
- LAN based games were never designed to take player data from outside / public networks.



**Retro-Online Options**


With thanks to many talented developers, there are now some incredible ways to play your favourate retro games online with like minded friends.    I'll expand on these over the next few months / years, but highly recommend googling the following for more informatin to get started...

Things to note:
- You should aim to play with friends that are located within the same country or region of the planet (network latency of no more than about 50-150 max).  Some emulation options are more tolerant but significantly diminish the gaming experience.
- Use wired connections whenever possible (wireless is possible but usually problematic)
- in some cases you will need to create a PORT or enable Upnp  on your internet router (this will be explained in more detail later).
- In most cases the following are free / accessible community projects.
- There are many remakes / remasters of retro games available from Steam / Epic etc that also support revised online modes.


**Getting Started**

The following are my picks for playing 'Local Multiplayer' of your favourite console, computer and arcade fighting games using optimised NETPLAY features.

- **Fightcade** - One of the best, once installed plays a huge range of retro game and fighting games with a strong community and heavily optimised for online gaming with roll back and other tweaks (example: Mortal Kombat, Street Fighter 2).  Note: Limited to Max 2 Players, offers lobby and chat.  While all the best 8-bit/16-bit consoles and arcades are supported, also includes dreamcast (flycast).
- **RetroArch** - Offers play 4 players for your favourite emulatators, and relay servers to minimise needing to mess with your internet router.   While performance was generally really good, retroarch can be challenging to setup and nagivating the endless options - particularly with players thats have never used retroarch before.
- **AmigaLive** - Offers a great way to play side by side Amiga 500 and Amiga 1200 games over the internet, setup is very easy and a large number of amiga classics are supported.   Supports more than 2 players for games that support it.
- **DuckStation** - Offers a great way to play side by side PSX games over the internet, using rollback features to ensure smooth play online.

An alternative approach to consider for local multiplayer, is to use a video streaming service such as:
- **Parsec**  - While the above options use  netplay features (each player runs an local instance of the console / computer that is kept in sync at regular intervals), parsec runs everything on one computer and streams the video output to each participating player (players provide gamepad inputs to the host).  It is much more bandwidth heavy but avoids desync issues associated with netplay.  It is generally better for emulators that have no online / limited netplay features - i.e. N64 etc.   It effectively turns the hosts pc into a private retro cloud gaming service.

The following are my picks for playing 'Linked Multiplayer' of your favourite LAN / Serial link games:

- **DOSBOX** - Offers a great way to play network LAN games over the internet.   The best option is to look for the eXoDOS collection, which already configures each network / serial game for easy network play (the host will have to forward a network port on their router, which may not be possible for some users).
- **Doom / Duke3d / various source ports** - Many linked / LAN multiplayer games have been adapted into modern online friendly versions by various community focused projects.  This takes a lot of the pain of running online LAN Parties of your favourite FPS games, and adds in some nice quality of life improvements (support more than 8 players, mouse look) to make the classics much enjoyable.
- **Xlink Kai** - Provide a network tunnelling service for  emulators (and real gaming hardware) to communicate online.  It works great, has great documentation and support, but of time to setup can be considerable depending on the emulator  or real console your setting up.   The biggest benefit is that you can game with a mix of real gaming hardware (e.g. PS2) and emulators (PCSX2) on the same network.


**Network Ports**

Sooner or later when playing retro games online, you'll reach a point where you cannot play a certain game or service without first forwarding a network port on your router. This is highlighted  when you attempt to host a game and no players can connect to your game because no players are able to make direct connection to your gaming server.  There are a few options on how navigate this:

Configure your home internet router
- Login to your router and manually forward a TCP/UDP port to your local PC (as instructed by the game or emulator)
- Login to your router and enable uPnP (this enables some emulators to automatically setup port forwarding / or easy setup port forwarding from your desktop PC using a upnp app)

Use a Relay Service / VPN
- If you cannot forward ports due to limitations / restrictions of you network - you can use a free network relay services like https://portmap.io/  (haven't used this one yet, but there many alternatives available).  This will enable you to host a game without amending any of your network settings as other players will connect to the publically accessible relay service which is then redirected to via a tunnelling app to the gaming server on your pc.

While using a relay service will add some minor lag to your player connections, it may be the only option for some users.


dek 
