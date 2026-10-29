<div align="center">

  <img src="icon.png" alt="Projectile Trajectory Preview logo" width="130" />

  # Projectile Trajectory Preview

  **Full client-side projectile trajectory previews for Minecraft Java 1.21.11 (Fabric).**

  [![CI build](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/actions/workflows/build.yml/badge.svg?branch=compat/minecraft-1.21.11)](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/actions/workflows/build.yml)
  ![Minecraft](https://img.shields.io/badge/Minecraft-1.21.11-62b47a)
  ![Loader](https://img.shields.io/badge/Loader-Fabric-f2bd74)
  ![Side](https://img.shields.io/badge/Side-Client%20Only-3b82f6)
  ![License](https://img.shields.io/badge/License-MIT-gray)

  **[Download v1.0.35 .jar](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/releases/download/v1.0.35-mc1.21.11-client/ptp%2B1.21.11-1.0.35.jar)** · **[Release notes](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/releases/tag/v1.0.35-mc1.21.11-client)** · **[Issues](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/issues)**

</div>

> [!IMPORTANT]
> **Install on your client only.** No mod, plugin, handshake, or configuration is required on the Minecraft server.
> This is a **pre-release**: GitHub Actions build and JAR structural checks pass, but in-game testing is not yet complete.

## Features

- **Projectile trajectories** – see a predicted flight path before throwing or firing.
- **Impact previews** – highlight or outline the expected block or entity impact area.
- **Supported vanilla items** – bow, crossbow, trident, ender pearl, snowball, egg, wind charge, potions, experience bottles, and fishing rod.
- **Configurable display** – change trajectory color, transparency, style, impact highlighting, and per-item toggles.
- **Offhand support** – use supported projectiles from your offhand.
- **Fully client-side** – trajectory prediction and rendering run on the local client without a custom server packet exchange.

## Requirements

| Component | Requirement |
| --- | --- |
| Minecraft Java Edition | **1.21.11** |
| Mod loader | **Fabric Loader** |
| Dependency | **Fabric API** compatible with Minecraft 1.21.11 |
| Java | **21 or later** |
| Mod Menu | Optional |

Other Minecraft or loader versions have not been verified for this release.

## Installation

1. Install Fabric Loader for **Minecraft 1.21.11** and a compatible Fabric API.
2. Download **[ptp+1.21.11-1.0.35.jar](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/releases/download/v1.0.35-mc1.21.11-client/ptp%2B1.21.11-1.0.35.jar)**.
3. Place the JAR in your Minecraft instance's `mods/` folder (typically `.minecraft/mods/`).
4. Start the Minecraft **Fabric 1.21.11** instance. **Do not install this mod on the server.**

**สำหรับผู้เล่นไทย:** ลง Fabric 1.21.11 และ Fabric API จากนั้นนำไฟล์ `.jar` ไปใส่ในโฟลเดอร์ `mods` ของ Minecraft ฝั่งผู้เล่นเท่านั้น ไม่ต้องลง Mod ที่เซิร์ฟเวอร์

## Configuration and controls

- Open the configuration screen with the **`/ptpConfig`** client command.
- If Mod Menu is installed, open the mod's configuration through Mod Menu.
- Settings are saved to `.minecraft/config/ptp.json` (inside your active Minecraft instance).
- Hold **B** (default) to preview a dropped item's trajectory.
- A separate **trajectory toggle** keybind is provided but is unbound by default; assign it under Minecraft Controls / Key Binds.

## Multiplayer and limitations

- **Server installation is not required.** The mod has no server initializer or custom handshake packets.
- Trajectory predictions use client-visible information. Random projectile spread, latency, server-side physics, and other discrepancies may make actual impact locations differ.
- Items from other mods are not officially supported by this build.
- Some servers restrict trajectory-assistance mods, particularly in PvP. Follow the server's rules before using this mod.

## Source, builds, and project status

- **Working 1.21.11 source:** [`compat/minecraft-1.21.11`](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/tree/compat/minecraft-1.21.11).
- **Release v1.0.35:** built from commit [`5f28bc0`](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/commit/5f28bc0b5afea6fddacdf6ac392fff0d5992b70d).
- **Verified CI:** [GitHub Actions run #40929984005](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/actions/runs/40929984005) passed Java compilation, remapping, JAR metadata checks, and artifact upload.
- **`master` branch:** contains separate newer-version development code; do not assume the master branch builds for Minecraft 1.21.11.
- **Earlier v1.0.34 release:** remains available in [Releases](https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/releases), but **v1.0.35** is the first full client-only release.

To build this version from source:

```bash
git clone --branch compat/minecraft-1.21.11 https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21.git
cd ProjectilesTrajectoryPreview1.21
./gradlew build
```

Find the remapped mod JAR in `build/libs/`, excluding the `-sources.jar` file.

## Credits and license

Based on the original MIT-licensed **[Projectile Trajectory Preview by maDU59](https://github.com/maDU59/ProjectilesTrajectoryPreview)**. Original artwork and attribution are retained. See [LICENSE](LICENSE).

> [!NOTE]
> The Modrinth and CurseForge listings for Projectile Trajectory Preview refer to the **original upstream project**, not this fork's GitHub Releases.

---

<!-- CYTECH_STAR_HISTORY:START -->

## Star History

<a href="https://github.com/Namnarak/ProjectilesTrajectoryPreview1.21/stargazers">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Namnarak/ProjectilesTrajectoryPreview1.21/refs/heads/master/assets/star-history-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Namnarak/ProjectilesTrajectoryPreview1.21/refs/heads/master/assets/star-history-light.svg" />
    <img alt="Star history for Namnarak/ProjectilesTrajectoryPreview1.21" src="https://raw.githubusercontent.com/Namnarak/ProjectilesTrajectoryPreview1.21/refs/heads/master/assets/star-history-light.svg" width="1100" />
  </picture>
</a>

<sub>Updated automatically from GitHub's dated stargazers. Only currently starred accounts are included.</sub>

<!-- CYTECH_STAR_HISTORY:END -->
