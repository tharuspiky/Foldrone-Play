# Foldrone Play

**Unbound Playback | One Fluid Space**

> The next evolution in media playback. Intelligent audio tuning and crisp visuals, crafted for absolute clarity.

Foldrone Play is a privacy-first, responsive media player built as part of the Foldrone ecosystem. It is designed around a universal playback experience that adapts to phones, tablets, desktops, large displays and future native clients without making playback dependent on cloud services.

## ✨ Phase 1 Public Preview

**v0.4.9**

The Phase 1 baseline establishes the first public Foldrone Play Media Core experience.

### Included

- Local media playback
- Direct media URL playback
- Video, audio and image presentation
- Audio-only visualizer
- Playback speed cycling: 1× → 1.5× → 2× → 0.5× → 0.75× → 1×
- Intelligent audio modes and video-quality modes
- Foldrone CC Engine
- Embedded and external subtitles
- SRT/VTT subtitle loading
- Subtitle provider discovery
- Subtitle timing/synchronization foundation
- Picture-in-Picture and fullscreen where supported
- Responsive portrait and landscape layouts
- PWA support
- Touch playback zones
- Queue and transport controls
- Cinematic landing experience
- Foldrone Play welcome tone
- Cloudflare Worker security headers and health endpoint

## 🧠 Design Principles

### Playback first
Local playback should remain useful when network services are unavailable. Optional intelligence should enhance playback, not become a prerequisite for it.

### Universal by design
The interface uses responsive and capability-aware behavior rather than being designed around one device family.

### Privacy first
Media processing should happen locally whenever practical. Provider credentials and other secrets must never be shipped to browser code.

### Modular Media Core
Playback, captions, audio enhancement, visual enhancement, provider adapters and future Foldra capabilities are intended to remain modular.

## 💬 Foldrone CC Engine

The compact **CC+** control cycles through available caption tracks. A dedicated subtitle workflow supports local subtitle loading and provider discovery.

Current subtitle inputs include:

- Embedded subtitle tracks
- SRT
- WebVTT
- Matching subtitle sidecars
- Additional formats where the runtime can parse them

Online subtitle discovery currently opens external services. Automatic provider API integration must remain server-side and must respect each provider's terms.

## 🔐 Security

The public repository contains no provider API secrets.

The Cloudflare Worker provides security headers including:

- Content Security Policy
- Strict Transport Security
- Referrer Policy
- X-Content-Type-Options
- X-Frame-Options
- Permissions Policy
- Cross-Origin policies

See [SECURITY.md](SECURITY.md).

**Important:** browser source code cannot be made secret in a public web application. Security-sensitive operations must therefore be enforced server-side.

## ☁️ Deployment

Foldrone Play is designed to run as a Cloudflare Worker with static assets.

```bash
npx wrangler deploy
```

Never place Cloudflare tokens, provider credentials or other secrets in source files.

## 🗺️ Roadmap

Future Media Core work may include:

- Device/output-aware adaptive audio
- Advanced video enhancement
- Improved subtitle synchronization and selection
- Additional media containers and streaming paths
- Native receiver/casting architecture
- Media session continuity
- Semantic media search
- Chapters and scene intelligence
- Offline media intelligence
- Foldra-assisted media workflows
- Native Foldrone clients

## 🤝 Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## 📜 License & Brand

Source code is released under the **Apache License 2.0**. See [LICENSE](LICENSE).

Foldrone, Foldrone Play, Foldra and associated logos/marks are Foldrone branding. The source-code license does not grant trademark rights.

Built under **Foldrone Labs**.

**Unbound Playback | One Fluid Space**
