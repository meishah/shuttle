# Shuttle

A lightweight Android VPN client for OpenVPN, WireGuard and AmneziaWG.

## Features

- **OpenVPN** — import `.ovpn` files (single file or ZIP), saved username/password
- **WireGuard & AmneziaWG** — full Amnezia settings (Mimic QUIC/DNS/SIP, junk packets)
- **Kill switch**, auto-connect and auto-reconnect
- **Config groups** — custom names, reorderable, shown on the home screen
- **Ping & sort** — ping servers from the list, sort by lowest ping
- **Per-app VPN** — choose which apps use the tunnel
- **Quick Settings tile** and home-screen widget for connect/disconnect
- **Backup & export** — configs as a ZIP file, manual in-app editing
- **Connection log** for troubleshooting
- **Themes** — light, dark, auto; **languages** — English and Persian
- Very low battery use, no extra permissions, arm64 only

## Download

Get the latest APK from [Releases](https://github.com/meishah/shuttle/releases) — three variants:

| Variant | For |
|---|---|
| `universal` | Any device |
| `arm64-v8a` | Most modern phones (64-bit ARM) |
| `armeabi-v7a` | Older phones (32-bit ARM) |

## Screenshots

![Home — connected](screenshots/home-connected.jpg)
![Home — disconnected](screenshots/home-disconnected.jpg)
![Settings](screenshots/settings.jpg)

## Usage

1. Install the APK and import your configs (`+` → import file or ZIP).
2. Tap **Ping servers** to measure latency, then **Connect** on any config.
3. Long-press a config for rename, delete, move to a group, or edit.
4. Long-press a group chip to reorder groups.

## Build from source

```bash
./build.sh assembleStandaloneRelease
```

Requires JDK 21 and the Android SDK (API 37).

## Credits & license

Built on [WG Tunnel](https://github.com/wgtunnel/android) (Apache 2.0) and [ics-openvpn](https://github.com/schwabe/ics-openvpn) (GPLv3). Shuttle is released under the **GNU General Public License v3.0** — see [LICENSE](LICENSE).
