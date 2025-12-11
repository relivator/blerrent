# Blerrent

✨ Website (soon) • [💬 Discord](https://discord.gg/Pb8uKbwpsJ) • [📦 GitHub](https://github.com/reliverse/blerrent) • [💖 Sponsor Development](https://github.com/sponsors/blefnk)

> @reliverse/blerrent (CLI + 🔜 library + 🔜 desktop) is a high-performance BitTorrent client built for today's tools — and tomorrow's ideas. The CLI and desktop app are designed for users who want power without the bloat. The TypeScript-first library is crafted for developers who care about precision, speed, and clean, frictionless DX.

## What is Blerrent?

**@reliverse/blerrent** is your all-in-one BitTorrent experience:

- 🧑‍💻 **CLI tool** — for terminal lovers & automation
- 🛠️ **TypeScript-first library** — for clean, hackable integrations
- 🖥️ **Desktop app** — for everyday users (coming soon)

> **⚡ Note:**  
> Blerrent is a vision in motion. The CLI is already live; the library and desktop app are coming next.
> Got ideas, needs, or wild feature requests? Tell us on [Discord](https://discord.gg/Pb8uKbwpsJ) or open an [Issue](https://github.com/reliverse/blerrent/issues). Your voice shapes the future.

## Core Features

@reliverse/blerrent is your zero-bloat, high-speed gateway to the BitTorrent universe — built for modern CLIs, precision dev tools, and future-ready apps.

### CLI-first BitTorrent Client

- 📥 Download torrents via magnet links or `.torrent` files
- 🔥 Stream files as you download (video, audio, anything)
- 📦 Seed and share torrents easily
- 🧩 CLI extensions: download playlists, archives, data bundles
- 🏃 Smart resume support for interrupted downloads

### TypeScript-first Library

> Power to the devs. Build your own tools with fine-grained control.

- 📚 Full TS typings, JSDoc, and lightweight DX
- 🛠️ Import core modules (torrent engine, magnet parser, piece manager)
- 🔥 Extendable via plugins/hooks
- 🧩 Easy embedding into CLI, web, and desktop apps

### Desktop App (coming soon)

- 🖥️ Local torrent manager
- 🎛️ Stream and control torrents from GUI
- 🧹 Focus on speed, UX, and zero-bloat
- 🛠️ Plugin-ready (themes, streaming tools, file converters)

## Use Cases

- 📡 Download Linux ISOs, datasets, movies, and anything else at full speed
- 🎥 Stream videos from magnet links directly in your terminal
- 🎮 Share mods, maps, and game assets via decentralized sharing
- 🛠️ Integrate a torrent engine into your Node.js, Bun, or Deno projects
- 🚀 Build your own automation flows (e.g., "download + seed + auto-archive")

## Platform Support

| Platform    | CLI | Library | Desktop App | Status        |
|-------------|-----|---------|-------------|---------------|
| macOS       | ✅  | 🔜       | 🔜           | CLI ready     |
| Windows     | ✅  | 🔜       | 🔜           | CLI ready     |
| Linux       | ✅  | 🔜       | 🔜           | CLI ready     |
| Web (Browser) | 🔜 | 🔜       | 🔜           | Planned       |

> **Built with** Node.js, Bun, WebTorrent, Tauri, TypeScript.

## CLI Examples

```bash
# Download a torrent from a magnet link
blerrent download "magnet:?xt=urn:btih:..."

# Download from a .torrent file
blerrent download ./ubuntu-iso.torrent

# Stream a video while downloading
blerrent stream "magnet:?xt=urn:btih:..."

# Seed a folder as a new torrent
blerrent seed ./my-shared-folder

# Check active downloads
blerrent status
```

## Library Examples

```ts
import { createClient } from '@reliverse/blerrent'

const client = createClient()

await client.add('magnet:?xt=urn:btih:...')
client.on('download', (torrent) => {
  console.log(`Progress: ${torrent.progress}%`)
})
```

> **More API docs soon!** Expect a clean modular structure for full control.

## Planned Features

- 🔥 Streaming server (stream torrents to devices on local network)
- 🚀 Support for WebSeeds
- 🧠 Smart bandwidth management
- 🛡️ IP filtering and privacy options
- 🔗 Trackerless DHT-only mode
- 📦 Bundled CLI plugins (e.g., "auto-extract archives after download")
- 🎛️ Desktop app with theming & extensions

## Why Blerrent?

- 🏎️ Speed-first. No bloat.
- 🧩 Hackable & modular.
- ⚙️ CLI-native and scriptable.
- 🔒 Privacy-respecting.
- 🚀 Built with developers, creators, and heavy users in mind.

## Contributing

- 🧠 Share feature ideas
- 🐛 Report bugs
- 🔥 Build CLI plugins
- 🎨 Contribute to the desktop app
- 📦 Help improve the TypeScript SDK

> **Welcome to the next-gen torrenting experience. Let’s build it together.**

## Recommended Setup

- [Node.js 22+](https://nodejs.org/)
- [Bun 1.2+](https://bun.sh/)
- [VS Code](https://code.visualstudio.com/)

## License

MIT © [@blefnk (Nazar Kornienko)](https://github.com/blefnk)  
Part of the [Reliverse](https://github.com/reliverse) ecosystem.

*🧹 Built with speed, soul, and relentless simplicity.*  
*⚡ Blerrent is torrenting for those who care about their tools.*
