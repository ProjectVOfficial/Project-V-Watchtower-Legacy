<div align="center">

# Project V // Watchtower

**Local-first Windows situational awareness, mapping, research, case management, and optional local-AI analysis.**

[![Release](https://img.shields.io/github/v/release/ProjectVOfficial/Project-V-Watchtower?include_prereleases&sort=semver&style=flat-square&label=Release)](https://github.com/ProjectVOfficial/Project-V-Watchtower/releases)
[![Downloads](https://img.shields.io/github/downloads/ProjectVOfficial/Project-V-Watchtower/total?style=flat-square&label=Downloads)](https://github.com/ProjectVOfficial/Project-V-Watchtower/releases)
[![License](https://img.shields.io/github/license/ProjectVOfficial/Project-V-Watchtower?style=flat-square&label=License)](LICENSE)
![Platform](https://img.shields.io/badge/platform-Windows%20x64-0078D4?style=flat-square&logo=windows11&logoColor=white)
![Runtime](https://img.shields.io/badge/runtime-Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![Local AI](https://img.shields.io/badge/local%20AI-Ollama-000000?style=flat-square&logo=ollama&logoColor=white)

[**View Releases**](https://github.com/ProjectVOfficial/Project-V-Watchtower/releases) ·
[**Installation**](INSTALLATION.md) ·
[**White Paper**](WHITEPAPER.md) ·
[**Security**](SECURITY.md) ·
[**Upstream & License**](UPSTREAM_AND_LICENSE.md)

</div>

> [!NOTE]
> **Downstream project.** Project V // Watchtower is an independently maintained and substantially modified downstream work based on World Monitor. It is not an official World Monitor release and is not maintained or endorsed by the upstream developers.

> [!WARNING]
> Watchtower has not undergone an independent security audit. Current Windows builds are unsigned and may trigger Windows SmartScreen or unknown-publisher warnings.

## Current Windows build

The current public Windows reference build is **v1.1.0-1**.

Available release assets include:

- Windows NSIS installer: `Project.V.Watchtower_1.1.0-1_x64-setup.exe`
- Windows MSI installer: `Project.V.Watchtower_1.0.0_x64_en-US.msi`
- Standalone Windows executable: `project-v-watchtower.exe`

Use the [Releases page](https://github.com/ProjectVOfficial/Project-V-Watchtower/releases) for downloads.

> The current release line was published as a pre-release / production-candidate build. Project V can publish a later stable-tagged release after its final release review.

## What Watchtower does

Project V // Watchtower is a Windows desktop command center built with Tauri, TypeScript, Vite, MapLibre, and optional local AI through Ollama.

It brings live information, maps, research, cases, operational notes, public-source tools, alerts, and local analysis into one workspace.

### Major capabilities

- Customizable multi-workspace command deck
- Live world map and situational-awareness panels
- Air Operations with ADS-B tracking, watchlists, trails, and aircraft intelligence
- Weather Operations with live radar, forecasts, watched locations, and history
- Severe Weather Intelligence using official alert data
- Tropical Operations using NOAA / NHC data
- Research Library for documents, excerpts, notes, and source material
- Case Desk for investigations and evidence organization
- Data Desk for structured data workflows
- Map Operations for markers, routes, areas, measurements, GeoJSON, and geofenced alerts
- Optional local Command Assistant using Ollama
- Multi-agent Analysis Room
- OSINT Desk for approved public-source research handoffs
- Camera Wall
- Communications Wall
- Launch Deck and restricted Source Browser
- Local plugin foundation with permissions and sandboxing
- Project Lock, backup, recovery, diagnostics, and safe mode
- Optional voice-command and spoken-alert foundations

See [WHITEPAPER.md](WHITEPAPER.md), [UPDATES.md](UPDATES.md), and [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) for more detail.

## Local-first does not mean offline-only

Watchtower stores many workspaces, cases, research records, preferences, and local AI conversations on the computer. Live panels and public-source tools may still connect to external providers.

Some features require internet access, provider credentials, third-party services, or separately installed local services.

See [PRIVACY.md](PRIVACY.md) and [docs/DATA_AND_AI.md](docs/DATA_AND_AI.md).

## Optional local AI

Ollama is optional. Watchtower does not require Ollama merely to open and use the command deck.

AI output is analysis, not evidence. Multiple agent roles using the same underlying model are not independent corroboration.

## Upstream, copyright, and license

Watchtower contains upstream World Monitor-derived material as well as substantial Project V-authored modifications and additions.

Copyright ownership is not collapsed into a single owner:

- upstream authors retain copyright in their upstream contributions;
- Project V contributors retain copyright in their original Project V-authored contributions, subject to any assignments or third-party rights;
- the combined covered work is distributed under **AGPL-3.0-or-later**.

Project V does **not** claim ownership of upstream World Monitor code.

The AGPL licensing of the combined work does not erase the separate copyright ownership of original contributions. It does, however, control how the covered combined work may be redistributed.

See:

- [LICENSE](LICENSE)
- [NOTICE.md](NOTICE.md)
- [UPSTREAM_AND_LICENSE.md](UPSTREAM_AND_LICENSE.md)

## Corresponding source

Because Watchtower is an AGPL-covered downstream work, distributed binaries must be accompanied by, or provide compliant access to, the corresponding source for the exact released build.

The release page may emphasize installers and executables, but the corresponding source requirement still applies.

See [UPSTREAM_AND_LICENSE.md](UPSTREAM_AND_LICENSE.md) for the release rule.

## Security

Watchtower is security-oriented software, but it is not represented as independently security-audited.

Read [SECURITY.md](SECURITY.md) before using it with sensitive information.

## Support

Use GitHub Issues for reproducible bugs and feature requests. Do not post API keys, private research, personal data, sensitive locations, exploit details, or unredacted private logs.

## Project V

Project V // Watchtower is maintained under the **ProjectVOfficial** GitHub account as part of the broader Project V software ecosystem.

---

**Project V // Watchtower**  
Observe widely. Preserve context. Verify before conclusion.
