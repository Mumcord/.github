<a href="https://mumcord.app/en">
  <img src="banner.png" alt="Mumcord: Your Mumble server. Finally cosy." width="100%">
</a>

<p align="center">
  <a href="https://github.com/Mumcord/mumcord/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/Mumcord/mumcord?include_prereleases&style=for-the-badge&label=release&labelColor=0e0a26&color=ff6fa8"></a>
  <a href="https://github.com/Mumcord/mumcord/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/github/license/Mumcord/mumcord?style=for-the-badge&labelColor=0e0a26&color=9b7bff"></a>
  <a href="https://github.com/Mumcord/mumcord/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/Mumcord/mumcord?style=for-the-badge&labelColor=0e0a26&color=ffb08a"></a>
  <a href="https://mumcord.app/en"><img alt="Website" src="https://img.shields.io/badge/mumcord.app-visit-3ee39e?style=for-the-badge&labelColor=0e0a26"></a>
</p>

### Hey there 👋

**Mumcord** is a modern desktop client for [Mumble](https://www.mumble.info): server bar, text channels you can read without joining, member list, push-to-talk on any key or mouse button, themes, a game overlay, watch parties and screen sharing. It speaks the plain Mumble protocol, so it works on **any standard Mumble server** with nothing to install there.

Open source, no telemetry, made in the EU.

### Projects

| | Project | What it is | Status |
|:-:|:--|:--|:--|
| 🎧 | **[mumcord](https://github.com/Mumcord/mumcord)** | The desktop client for Linux, Windows and macOS | <a href="https://github.com/Mumcord/mumcord/releases"><img alt="Mumcord release" src="https://img.shields.io/github/v/release/Mumcord/mumcord?include_prereleases&label=alpha&labelColor=0e0a26&color=ff6fa8"></a> |
| 🤖 | **[mumbot](https://github.com/Mumcord/mumbot)** | Bots for any Mumble server: a webhook bot that posts alerts and CI results into channels, and a scripted test bot for Mumble clients | <a href="https://github.com/Mumcord/mumbot/releases"><img alt="Mumbot release" src="https://img.shields.io/github/v/release/Mumcord/mumbot?label=release&labelColor=0e0a26&color=9b7bff"></a> |
| 🔁 | **[mumpeer](https://github.com/Mumcord/mumpeer)** | An optional relay for Mumcord's peer-to-peer features, for users behind strict NAT or who want to hide their IP address | Planned for Epic 3 |
| 🌐 | **[mumcord-www](https://github.com/Mumcord/mumcord-www)** | The website at [mumcord.app](https://mumcord.app/en) | Live |

### Get Mumcord

- **Windows and macOS:** grab the installer from the [latest release](https://github.com/Mumcord/mumcord/releases/latest).
- **Linux:** `.deb`, `.rpm` and AppImage in the [latest release](https://github.com/Mumcord/mumcord/releases/latest), or the installer in one line:

  ```sh
  curl -fsSL https://github.com/Mumcord/mumcord/releases/latest/download/install.sh | sh
  ```

No server of your own yet? The [server guide](https://mumcord.app/en/server) sets one up with Docker in a few minutes.

### Get Mumbot

Post a message into a Mumble channel with one HTTP request, from monitoring, CI or any script. Mumbot logs in like a normal client, so nothing changes on the server.

```sh
docker run -d --name mumbot \
  -v "$PWD/bot.toml:/config/bot.toml:ro" \
  -v mumbot-data:/data -p 127.0.0.1:8080:8080 \
  ghcr.io/mumcord/mumbot:latest
```

Binaries for Linux, Windows and macOS, the config and [Docker Compose examples](https://github.com/Mumcord/mumbot/tree/main/examples) are on the [Mumbot page](https://mumcord.app/en/mumbot).

### Get involved

- 💡 Have an idea? [Request a feature](https://github.com/Mumcord/mumcord/issues/new?template=feature_request.yml)
- 🐞 Something broke? [Report a bug](https://github.com/Mumcord/mumcord/issues/new?template=bug_report.yml)
- 📖 Guides and answers live in the [wiki](https://github.com/Mumcord/mumcord/wiki)
- 🗺️ What's next: the [Mumcord roadmap](https://mumcord.app/en/roadmap) and the [Mumbot roadmap](https://mumcord.app/en/mumbot#roadmap)
- 🤖 Ideas for a bot? [Mumbot issues](https://github.com/Mumcord/mumbot/issues)

<sub>Mumcord is compatible with Mumble but is neither affiliated with nor endorsed by the Mumble project.</sub>
