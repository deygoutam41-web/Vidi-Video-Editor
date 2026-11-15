# Vidi Video Editor

A browser-based video editing MVP built for desktop Chrome and other modern browsers.

## Run
Open `index.html` through a local web server or enable GitHub Pages for this repository. The FFmpeg WebAssembly export engine is loaded from a CDN on demand, so internet access is required for MP4 export.

## MVP features
- Import a local video and preview it in the browser
- Playback, seek, and jump controls
- Set a trim-in and trim-out range
- Add a separate audio file to the export
- Add simple text overlays to the preview
- Export an MP4 at 720p, 1080p, or original resolution using FFmpeg.wasm

## Current limitations
This is an initial MVP, not a full nonlinear editor. Split adds a visual playhead marker only; text overlays are preview-only and are not burned into the exported MP4. Transitions, multi-clip compositing, project saving, and frame-accurate editing are not included yet. Large videos may exceed browser memory limits.

## Privacy
Video and audio files are processed locally in the browser; they are not uploaded to an application server. FFmpeg and its core are downloaded from the configured CDN when exporting.
