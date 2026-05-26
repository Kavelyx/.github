<div align="center">

# Kavelyx

### Local-first software for private homes, personal servers, and calm automation.

Kavelyx builds practical home infrastructure that stays understandable: local web experiences, secure device control, private media workflows, and installable apps designed for small ARM servers.

[![kavelyxOS](https://img.shields.io/badge/kavelyxOS-local--first-0f172a?style=for-the-badge)](#kavelyxos)
[![Private by design](https://img.shields.io/badge/private-by%20design-14532d?style=for-the-badge)](#principles)
[![Built for ARM](https://img.shields.io/badge/built%20for-ARM%20servers-1d4ed8?style=for-the-badge)](#what-we-are-building)

</div>

---

## What We Are Building

**kavelyxOS** is a local-first web OS for Radxa and Raspberry Pi style mini servers. The goal is to turn a small board into a polished home server experience that can be flashed, booted, configured, and maintained without asking the owner to become a Linux administrator.

The V1 direction includes:

- a flashable SD card image for supported devices
- first-boot setup with no default admin account
- a local web shell for apps, settings, storage, logs, and updates
- secure local automation and camera foundations
- signed `.kavapp` packages for an installable app ecosystem
- storage rules that protect microSD cards from heavy 24/7 workloads
- Cloudflare-backed services only where they make the local system better

## Principles

- **Local first:** the home server should keep working when the cloud is unavailable.
- **Private by default:** secrets, media, device state, and admin surfaces are treated as sensitive from day one.
- **Simple ownership:** setup, updates, backups, and recovery should feel guided instead of fragile.
- **Useful before flashy:** every surface should help the owner understand or control the system.
- **Open architecture, careful releases:** app packaging, signing, validation, and device support evolve with clear rules.

## Project Areas

| Area | Focus |
| --- | --- |
| OS image | Debian/Armbian based image builds, first boot, system services, safe resets |
| Web shell | Next.js interface, dashboard, launcher, settings, installable PWA experience |
| Core API | Fastify, realtime events, SQLite, permissions, device and system services |
| App platform | `.kavapp` manifests, validation, signing, local install/update/rollback flows |
| Store | Cloudflare-backed catalog, private packages, signed metadata, developer/admin portals |
| Devices | MQTT foundations, scenes, camera workflows, future Home Assistant and Zigbee integration |

## Repository Status

Most Kavelyx engineering repositories are private while the foundation is being built. Public repositories, docs, SDKs, and release artifacts will appear here as pieces become useful outside the core team.

## kavelyxOS

The current flagship project is **kavelyxOS**, a private monorepo containing the web UI, API, shared packages, Docker stack, OS image overlays, release scripts, and architecture documentation.
