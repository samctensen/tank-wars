# Tank Wars

A networked multiplayer tank game built in C# with a client-server architecture and a Windows Forms client.

Originally developed as the final project of fall semester 2021, before Christmas break. Uploaded to GitHub in January 2022. The [original development notes and controls](Resources/README.txt) document work through November and December 2021.

## Run

Open `TankWars.sln` in Visual Studio on Windows and restore NuGet packages. The original solution uses .NET Framework 4.7.2 and .NET Standard 2.0; the earlier networking tests target .NET Core 3.1.

Start the `Server` project, then the `View` client and connect to the server. World settings live in `Resources/settings.xml`. Keep the expected resource paths when launching from Visual Studio. The original `GameController` project also contains a machine-specific Windows Forms assembly path that may need adjusting for your Windows installation.

Use W/A/S/D to move, the mouse to aim, the left mouse button to fire, and the right mouse button to use a collected beam powerup.

## Project

- `Server/`, `World/`, `GameController/`, `Vector2D/` — game and server logic.
- `View/`, `DrawingPanel/` — desktop client and rendering.
- `Resources/` — artwork, settings, original notes, and supplied libraries.
- `exercises/networking/` — the earlier PS7 networking solution and tests.

The game solution now sits at the repository root; original code and resources are preserved.
