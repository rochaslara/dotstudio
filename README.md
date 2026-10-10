# Dotwash

A browser tool for making animated halftone loops. Turn a generated pattern, your own text or an uploaded image into a dot screen, pick a motion and a palette, and export a seamless GIF, an MP4 or a PNG still.

**Live app:** https://rochaslara.github.io/dotstudio/

## What it does

- **Sources:** a generated pattern, your own text in any Google Fonts family (742 listed, any other loads by name), or an uploaded image. You can drop or paste images onto the preview.
- **Motion:** Linear, Radial, Pulse, Blobs, Fluid, Waves, Spiral and Drift. Every animation loops seamlessly. Set Speed to *Still* for a static halftone gradient.
- **Halftone:** square, circle, diamond, line or cross dots, plus grid density, screen angle, smallest and largest dot, tone curve, which tones get the dots, and smooth or crisp edges.
- **Color:** background, ink and an optional second ink for larger dots, with quick palettes. For images, dots can take their color from the image.
- **Export:** GIF (loops forever), MP4 (H.264) or PNG, in 1:1, 4:5, 16:9, 9:16 or 3:2.
- **Presets:** ten built in. Save your own, which are kept in your browser.

## Running it

It's a single `index.html` with no build step. Open it in a current Chrome, Edge, Safari or Firefox, or serve the folder with any static server. It needs WebGL2. MP4 export uses WebCodecs where the browser has it and falls back to real-time recording otherwise.

Runtime dependencies load from CDNs: Google Fonts and [mp4-muxer](https://github.com/Vanilagy/mp4-muxer).
