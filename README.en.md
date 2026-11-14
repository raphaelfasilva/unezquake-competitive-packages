# unezQuake / ezQuake – Competitive configs

[🇧🇷 Português](README.md) | 🇺🇸 English

Ready-to-play packages of **unezQuake** (the ezQuake fork used in competitive play) and the original **ezQuake**, with a config optimized for competitive QuakeWorld.

## Packages

| Folder | Description |
|---|---|
| `unezquake_with_grey_texture` | unezQuake/ezQuake with **grey map textures** and **solid-color fullbright skins**, both widely used in competitive play. |
| `unezquake_without_grey_texture` | unezQuake/ezQuake **without the grey textures** (uses the original nQuake texture pack) and with **solid-color fullbright skins**. |

Fullbright skins paint each player in a solid, bright color that doesn't get darker in shadowed areas, so it's easy to tell who is who:

- **Enemies:** yellow. In FFA, every other player counts as an enemy.
- **Teammates:** dark blue, in team modes (2v2, 4v4, etc.).

## Binaries

| File | Description |
|---|---|
| `ezquake.exe` | unezQuake (competitive ezQuake fork) for **Windows** |
| `ezquake_original.exe` | Original ezQuake for **Windows** |
| `ezquake_linux_x86_64.AppImage` | unezQuake (competitive ezQuake fork) for **Linux** |
| `ezquake_original_linux_x86_64.AppImage` | Original ezQuake for **Linux** |

## Installation

> ⚠️ `pak1.pak` is **not included**, since it is part of the commercial version of Quake. Copy `pak1.pak` from your own copy of Quake (Steam, GOG, etc.) into the package's `id1` folder.

### Windows

1. Download and extract the package you prefer.
2. Copy `pak1.pak` into the `id1` folder.
3. Run `ezquake.exe` (unezQuake) or `ezquake_original.exe` (original ezQuake).

### Linux (Ubuntu 22.04 or newer)

1. Install the dependency required to run AppImages:
   ```bash
   sudo apt install libfuse2
   ```
   On Ubuntu 24.04 or newer, the package is called `libfuse2t64`:
   ```bash
   sudo apt install libfuse2t64
   ```
2. Download and extract the package you prefer.
3. Copy `pak1.pak` into the `id1` folder.
4. Make the binary executable:
   ```bash
   chmod +x ezquake_linux_x86_64.AppImage
   ```
5. Run it:
   ```bash
   ./ezquake_linux_x86_64.AppImage
   ```

## Main binds

| Key | Action |
|---|---|
| `MOUSE1` | Fire the currently selected weapon |
| `MOUSE2` | Fire the Shaft (LG / Thunderbolt) while held, then switch back to the previous weapon on release |
| `MOUSE3` | Select the SNG (Super Nailgun) |
| `MOUSE4` | Select the GL (Grenade Launcher) |
| `MOUSE5` | Rocket jump (selects the RL, jumps and fires) |
| `E` | Select the RL (Rocket Launcher) |
| `R` | Select the GL (Grenade Launcher) |
| `Q` | Select the LG (Lightning Gun) |
| `CAPSLOCK` | Select the SNG (Super Nailgun) |
| `TAB` | Show the scoreboard |
| `F12` | Take a screenshot |

## Commands

Type in the console (`` ` `` key):

| Command | Description |
|---|---|
| `ktx` | Enable the KTX mod (to play against bots) |
| `qwbrktx` | Connect to QW Brazil KTX server #1 |
| `qwbrktx2` | Connect to QW Brazil KTX server #2 (dedicated to practice) |
| `qwbrtd2` | Connect to the QW Brazil Total Destruction server |

> KTX lives in a separate folder and is **not loaded automatically**, since most people play on servers. To play against bots, type `ktx` in the console **before loading a map or joining a server**. Once a map is loaded, the command can't switch to the mod.

## Author

Package put together by **CrazyKillerBR**.

Questions, suggestions or issues: reach out on Discord at **`crazykillerbr`**.

## Credits

- **[Tiba](https://github.com/tibazera)**: original package with the grey textures and the competitive optimization settings.
- **[nQuake](https://nquake.com)** ([GitHub](https://github.com/nQuake)): texture pack used in competitive play and the base for the skins in this package.
- **[ezQuake](https://github.com/QW-Group/ezquake-source)**: QuakeWorld client.
- **[KTX](https://github.com/QW-Group/ktx)**: server mod (Kombat Teams eXtreme).
