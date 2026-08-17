# Kashmir Shaivism: Interactive Study Website

> A single-file, self-contained educational platform exploring the philosophy of Kashmir Shaivism through a warm, reading-focused interface. No build tools. No dependencies. Just open the HTML file.


---

![Live website](https://jps-saahil.github.io/kashmirshaivism.github.io/)


## Table of Contents

- [Overview](#overview)
- [Topics Covered](#topics-covered)
- [Features](#features)
- [Customization Panel](#customization-panel)
- [Music](#music)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Getting Started](#getting-started)
- [Technical Notes](#technical-notes)
- [Music Credits](#music-credits)

---

## Overview

This website is a single `.html` file that functions as a full single-page application for studying Kashmir Shaivism, one of the most sophisticated non-dual philosophical systems to emerge from the Indian subcontinent. It is designed to be both technically rigorous and aesthetically warm, pairing dense philosophical content with a paper-and-ink reading experience.

The site runs entirely in the browser with no server, no build step, and no external dependencies beyond Google Fonts and GitHub-hosted audio files.

---

## Topics Covered

The content is organized into **13 main topics**, each with multi-level subtopics:

| # | Topic | Description |
|---|-------|-------------|
| 1 | **Paramaśiva** | The supreme reality: Cit, Parasaṃvit, Prakāśa, Vimarśa, Svātantrya, and their unity |
| 2 | **Svātantrya** | Absolute freedom as the nature of consciousness |
| 3 | **Tattvas** | The 36 levels of manifestation from pure consciousness to earth |
| 4 | **Maya** | The veiling power and how the infinite appears finite |
| 5 | **Kañcukas** | The five sheaths of limitation that cover the soul |
| 6 | **Puruṣa** | The bound individual, the conditioned self |
| 7 | **Prakṛti** | Nature as the creative matrix below the Kañcukas |
| 8 | **Antaḥkaraṇa** | The inner instrument: Manas, Buddhi, Ahaṃkāra |
| 9 | **Pramātā** | The knower and varieties of experiencers across the Tattvas |
| 10 | **Upāyas** | The four means of liberation |
| 11 | **Spanda** | The divine vibration, dynamic pulsation of consciousness |
| 12 | **Pratyabhijñā** | Recognition, the heart of Kashmir Shaivism |
| 13 | **Mokṣa** | Liberation and the nature of recognition |

Each topic contains 2-3 levels of nested subtopics, offering progressively deeper engagement with each concept.

---

## Features

### Reading Experience

- **Warm paper-and-ink aesthetic**: sepia tones, editorial typography, generous spacing
- **11 curated typefaces**: EB Garamond, Cormorant Garamond, Crimson Text, Lora, Merriweather, Source Serif 4, Libre Baskerville, Gentium Plus, Spectral, Inter, Nunito
- **Custom font support**: load any Google Font by name, or upload a local font file (TTF, OTF, WOFF, WOFF2)
- **4 reading sizes**: S, M, L, XL with live in-panel preview
- **12 reading filters**: Off, Sepia, Paper, Parchment, Warm, Cool, Dim, Twilight, Night, Contrast, Moonlight, Forest
- **Light and Dark themes**: warm paper light mode and deep dark mode

### Navigation

- **Collapsible sidebar** with full three-level topic tree
- **Live topic search**: type `/` to focus, results filter instantly
- **Mobile bottom sheet**: drag-to-dismiss sidebar on small screens
- **SPA navigation** with no page reloads and instant transitions
- **Reading progress**: full-width bar at the top and a radial ring indicator
- **Continue Reading pill** that returns to your last position after navigating away

### Annotations

- **Sanskrit hover tooltips**: hover any highlighted Sanskrit term to see its meaning
- **Multi-bookmark drawer**: save and label any position, persists across sessions
- **English dictionary**: Free Dictionary API integration, accessible from the header
- **Google Translate**: full-page translation support built into the settings panel

### Interface

- **Fancy mode**: WebGL animated canvas background with glassmorphism panels
- **Basic mode**: clean, distraction-free layout
- **Blob magnifier lens**: a floating zoom lens for fine reading
- **Tracking eye**: animated logo with realistic iris, pupil, lashes, and blink
- **On-screen tutorial**: guided walkthrough for first-time visitors
- **localStorage persistence**: all preferences and bookmarks are saved locally

---

## Customization Panel

The customization panel (accessible via the sliders icon in the header) gives readers full control over the reading environment.

![Customization Panel](https://github.com/JPS-Saahil/Formique/blob/Assets/Kashmir%20shaivism%20website%20assets/custom.png)

The panel is organized into sections:

- **Typeface**: 11 built-in fonts + custom Google Font input + local file upload
- **Size**: four steps with a live preview sentence below the controls
- **Reading Filter**: colour overlay swatches applied to the page background
- **Mode**: toggle between Fancy (WebGL) and Basic
- **Language**: Google Translate selector
- **Dictionary**: inline English dictionary with the Free Dictionary API

---

## Music

The music player (header icon) supports two categories of tracks:

### Devotional

| Track | Creator |
|-------|---------|
| Chandrachooda | [Raghotham R](https://m.youtube.com/@raaghuu) |
| Karpura Gauram | [Traditional](https://youtu.be/ttmecaJuh1o?si=QFUOGKmNySAuPp_K) |
| Lingashtakam | [@hspiritual](https://m.youtube.com/@hspiritual) |
| Maha Mrityunjaya Mantra | [@SanatanSpiritualMusic](https://m.youtube.com/@SanatanSpiritualMusic) |
| Shiva Tandava Stotram | [@timesmusicspiritual](https://m.youtube.com/@timesmusicspiritual) |
| Vedasara Strotam | [Abhilipsa Panda](https://m.youtube.com/channel/UCv7UH9AVv2NF_1EIC1YYXlQ) |
| Vedic Chanting | [@ManishVyas](https://m.youtube.com/@ManishVyas) |

### Ambient

Forest · Flowing River · Winter Wind · Gentle Rain

Open the track list via the playlist icon in the music bar. Selecting a track starts playback immediately. On mobile the panel appears as a bottom sheet; on desktop it floats above the bar.

The creator card on the home page also includes a separate **voice message** audio player with a seek bar and time display.

---

## Keyboard Shortcuts



![Keyboard Shortcuts](https://github.com/JPS-Saahil/Formique/blob/Assets/Kashmir%20shaivism%20website%20assets/keyshortcut.png)

---

## Getting Started

No installation required.

1.Just press the link

---

## Technical Notes

| Property | Detail |
|----------|--------|
| **Architecture** | Single-file SPA: all HTML, CSS, and JS in one file |
| **Dependencies** | None (Google Fonts loaded via `<link>`, audio from GitHub Raw) |
| **State management** | Plain JS object (`S`) persisted to `localStorage` |
| **Rendering** | DOM manipulation with no virtual DOM and no framework |
| **Animations** | CSS transitions + WebGL shaders (Fancy mode) |
| **Audio** | Native `<audio>` element, streamed from GitHub Raw URLs |
| **Font loading** | Google Fonts API + `@font-face` injection for local uploads |
| **Mobile** | Responsive from 320px: draggable bottom sheet, touch events |
| **Browser support** | All modern browsers; WebGL required only for Fancy mode |

---

## Music Credits

All music used with attribution. Devotional tracks are the creative work of their respective artists; click the creator links in the music panel or in the table above to support them directly.

Ambient soundscapes are included as atmospheric aids to reading and contemplation.

---

*"This website is one of your tools on your spiritual journey, not a single source of solution to your understanding of yourself. May it serve as a gentle companion, not a destination."*
