# Wave Analyzer

Wave Analyzer is an [Obsidian](https://obsidian.md) community plugin for previewing audio files as interactive waveforms and spectrograms inside notes.

![](https://i.imgur.com/ODNE3Gr.png)


Repository: [zzigo/obsidian-waveanalyzer](https://github.com/zzigo/obsidian-waveanalyzer)

## Features

- Waveform and spectrogram views
- Play, stop, seek, and draggable playhead
- Loop-region selection in waveform view
- Variable spectrum resolution with 6 FFT sizes
- Optional audio-descriptors centroid and harmonicity overlays
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


## Audio-Descriptor's roadmap

[x] Spectral Centroid  
    Indicates brightness by computing the spectrum’s center of mass.

[x] Harmonicity  
    Measures degree of periodic structure versus noise in the signal.

[ ] Spectral Flux  
    Quantifies frame-to-frame spectral change, capturing timbral and onset activity.

[ ] Spectral Rolloff  
    Frequency below which a fixed percentage of spectral energy accumulates.

[ ] Zero-Crossing Rate  
    Counts sign changes per frame; correlates with noisiness and high-frequency content.

[ ] RMS Energy  
    Computes signal power per frame, reflecting perceived loudness dynamics.

[ ] Spectral Flatness  
    Ratio of geometric to arithmetic mean; indicates tonality versus noise-like spectra.
    
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

## Road Map 


## License

MIT
