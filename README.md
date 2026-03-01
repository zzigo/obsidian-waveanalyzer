# Wave Analyzer

Wave Analyzer is an [Obsidian](https://obsidian.md) community plugin for previewing audio files as interactive waveforms and spectrograms inside notes.

![](https://i.imgur.com/SFGbpxS.png)


Repository: [zzigo/obsidian-waveanalyzer](https://github.com/zzigo/obsidian-waveanalyzer)

## Features

- Waveform and spectrogram views
- Play, stop, seek, and draggable playhead
- Loop-region selection in waveform view
- Variable spectrum resolution with 6 FFT sizes
- Optional centroid and harmonicity overlays
- Timeline ruler with second and 10-second markers

## Usage

Embed an audio file in a note with a `wa` code block:

````
```wa
[[my-audio-file.mp3]]
```
````

The plugin renders the analyzer directly in reading view.

## Controls

- `Play / Stop`: start or stop playback
- `W / S`: switch between waveform and spectrum
- `Analysis`: toggle centroid and harmonicity overlays
- `Resolution`: cycle through 6 spectrum resolutions
- `Drag`: move the playhead anywhere on the timeline
- `Shift + drag` in waveform mode: create a loop region

## Development

This plugin currently uses plain JavaScript and esbuild.

Install dependencies:

```bash
npm install
```

Build:

```bash
npm run build
```

Development watch:

```bash
npm run dev
```

## Release Files

The repository root should contain these publishable files for each release:

- `manifest.json`
- `main.js`
- `versions.json`
- `styles.css` if a stylesheet is added later

## Publishing Notes

- Keep the `manifest.json` version in sync with the GitHub release tag.
- Create a GitHub release like `1.1.0` with no `v` prefix.
- Attach or publish the root build artifacts required by Obsidian.
- Submit the plugin repository to the Obsidian community plugin index.

## Manual Installation

1. Download the latest release assets from the GitHub releases page.
2. Copy `manifest.json`, `main.js`, and `versions.json` into `.obsidian/plugins/wave-analyzer/`.
3. Enable the plugin from Obsidian community plugins settings.

## License

MIT
