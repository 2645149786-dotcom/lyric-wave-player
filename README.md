<p align="center">
  <img src="https://img.shields.io/github/stars/2645149786-dotcom/lyric-wave-player?style=for-the-badge&color=a78bfa" alt="stars">
  <img src="https://img.shields.io/github/license/2645149786-dotcom/lyric-wave-player?style=for-the-badge&color=6366f1" alt="license">
  <img src="https://img.shields.io/badge/vanilla-js-yellow?style=for-the-badge" alt="vanilla js">
  <img src="https://img.shields.io/badge/Web_Audio_API-purple?style=for-the-badge" alt="web audio">
  <img src="https://img.shields.io/badge/zero-deps-brightgreen?style=for-the-badge" alt="zero deps">
</p>

<h1 align="center">Lyric Wave Player</h1>
<h3 align="center"><i>Immersive Audio Visualizer with Synced Lyrics</i></h3>

<p align="center">
  Upload audio + LRC lyrics for a beautiful fullscreen experience.<br>
  Real-time waveform meets perfectly timed lyrics. 100% client-side.
</p>

<p align="center">
  <a href="https://2645149786-dotcom.github.io/lyric-wave-player/"><strong>Live Demo</strong></a>
  &middot;
  <a href="https://toolknit.com/tools/lyric-visualizer.html"><strong>Full Version on ToolKnit</strong></a>
  &middot;
  <a href="#quick-start"><strong>Quick Start</strong></a>
</p>

<br>

---

## What This Is

A **pure JavaScript audio visualizer** that combines real-time waveform rendering with perfectly synced lyrics from LRC files.

Drop in an MP3 and its matching `.lrc` lyric file, and you get an immersive fullscreen music experience with a symmetrical frequency waveform and perfectly timed lyrics.

---

## Features

<table><tr><td width="50%">

### Audio Engine
- **Web Audio API** with AnalyserNode (FFT 512)
- **Symmetrical dual-wing waveform** with frequency boost
- **Solid fill** gradient below waveform curve
- **Clickable progress bar** for seek anywhere

</td><td width="50%">

### Lyric Engine
- **LRC parser** with regex `[mm:ss.ms]` extraction
- **Millisecond precision** sub-second sync
- **Fade transitions** for lyric entrance/exit
- **ID3 auto-extraction** of title, artist, cover art

</td></tr></table>

---

## Quick Start

```bash
git clone https://github.com/2645149786-dotcom/lyric-wave-player.git
open lyric-wave-player/index.html
```

That is it. No `npm install`. No build step. **One HTML file.**

---

## Architecture

```
index.html
   鈹溾攢鈹€ Inline CSS (dark-themed UI + fullscreen overlay)
   鈹溾攢鈹€ Inline JS
   鈹?    鈹溾攢鈹€ LRC Parser          Regex timestamp extraction
   鈹?    鈹溾攢鈹€ Web Audio Engine    AudioContext + AnalyserNode
   鈹?    鈹溾攢鈹€ Canvas Renderer     Symmetrical waveform draw loop
   鈹?    鈹斺攢鈹€ Lyric Syncer        currentTime lyric index match
   鈹斺攢鈹€ 1 CDN: jsmediatags        ID3 tag extraction (optional)
```

---

## Related

- **[ToolKnit](https://toolknit.com)** 89 free browser tools, full bilingual (EN/CH) version
- **[ToolKnit GitHub](https://github.com/2645149786-dotcom/toolknit)** More open-source standalone demos

---

## License

MIT. See [LICENSE](./LICENSE).

<br>

<p align="center"><sub>Built with love by <a href="https://toolknit.com">ToolKnit</a></sub></p>