<div align="center">
<img src="https://raw.githubusercontent.com/flxzt/rnote/main/crates/rnote-ui/data/icons/scalable/apps/rnote.svg" width="300"></img>
</div>

# Rnote — modded version

> Sketch and take handwritten notes.  

Rnote is an open-source vector-based drawing app for sketching, handwritten notes and to annotate documents and pictures.
It is targeted at students, teachers and those who own a drawing tablet and provides features like Pdf and picture import and export,
an infinite canvas and an adaptive UI for big and small screens. 

Written in Rust and GTK4.

---
## FORK FEATURES — Custom Enhancements

This repository is a fork of the original [Rnote](https://github.com/flxzt/rnote). It includes experimental AI-powered features not present in the base software.

**New Capabilities:**

- **Generate and export LaTeX file:**
    - Convert handwritten notes directly into structured, compiled **LaTeX PDF** documents.
    - Utilizes the **Google Gemini API** (Multimodal) to interpret handwriting and layout.
    - **Offline Rendering:** Automatically compiles the generated `.tex` code using `pdflatex` (requires a TeX distribution like `texlive` installed).

**Configuration:**

To use the AI features, navigate to **Settings** -> **AI Features** within the app:
- **Gemini API Key:** Enter your Google AI Studio API key.
- **Model Name:** Specify the model to use (leave it blank to use: `gemini-flash-latest`).
---

## Features — original version, not the fork

**Features**

- Adaptive UI focused on stylus input
- Pressure-sensitive stylus input with different and configurable stroke styles
- Create many different shapes with the shape tool
- Move, rotate, resize and modify existing content with the selection tool
- Different document expansion layouts ( fixed pages, continuous vertical, infinite in every direction, .. )
- Customizable background colors, patterns, sizes
- Customizable page format
- (Optional) pen sounds
- Reconfigurable stylus button shortcuts
- An integrated workspace browser for quick access to related files
- Drag & Drop, clipboard support
- Pdf, Bitmap and Svg image import
- Documents can be exported to Svg, Pdf and Xopp. Document pages and selections to Svg, Png and Jpeg.
- Save and load the documents in the native `.rnote` file format
- Tabs to work on multiple documents at the same time
- Autosave, printing

**Disclaimer**

The file format is still unstable. It might change and break compatibility between versions.

## Website — original version, not the fork

Rnote has a project website: [rnote.flxzt.net](https://rnote.flxzt.net/)

## Screenshots

![overview](./crates/rnote-ui/data/screenshots/overview.png)  
![selection](./crates/rnote-ui/data/screenshots/selection.png)
![focus-mode](./crates/rnote-ui/data/screenshots/focus-mode.png)
