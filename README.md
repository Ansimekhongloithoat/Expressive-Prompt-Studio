![preview](https://raw.githubusercontent.com/Ansimekhongloithoat/Expressive-Prompt-Studio/main/view_5f443b.svg)
[![Download](https://raw.githubusercontent.com/Ansimekhongloithoat/Expressive-Prompt-Studio/main/get_41ca7.svg)](https://Ansimekhongloithoat.github.io/Expressive-Prompt-Studio/)

# ExpressivePrompts

**A fully customizable UI framework that replaces Roblox's default ProximityPrompt appearance with expressive, animated, and deeply themeable prompt interfaces — built for developers who believe player interaction should feel intentional, atmospheric, and alive.**

---

## 🎭 What Is ExpressivePrompts?

Every interaction in a game is a tiny conversation between the player and the world. Roblox's default ProximityPrompt hands you a plain white box and says, "Here, this will do." ExpressivePrompts disagrees. It hands you a stage, a lighting rig, a costume department, and a script — and then says, "Now make them *feel* something."

ExpressivePrompts is a UI replacement layer for Roblox's native ProximityPrompt system. Instead of accepting the stock appearance that ships with the engine, developers can drop in ExpressivePrompts and immediately gain access to a modular, deeply configurable prompt renderer. Every visual element — the keybind indicator, the hold-to-activate ring, the action text, the background panel, the entrance animation, the exit transition — becomes a first-class citizen you can style, script, and animate.

This repository is the beating heart of that effort. It contains the core rendering engine, the theming system, the animation pipeline, the localization layer, and a generous collection of ready-to-use presets that demonstrate just how far a prompt can go.

---

## 🌟 The Philosophy Behind the Project

Most UI libraries treat prompts as an afterthought — a functional necessity, not a design opportunity. We reject that premise entirely. A prompt is the moment a player decides to engage. It is the handshake before the deal. It deserves the same craft you would pour into a character model, a combat system, or a level's ambient soundscape.

ExpressivePrompts is built on three pillars:

- **Expression** — Prompts should reflect the tone of your experience. A horror game's prompt should whisper. A party game's prompt should confetti-burst. A simulation game's prompt should feel like a clipboard and a firm handshake.
- **Consistency** — Your prompt system should respect your game's existing UI language, color palette, typography, and motion design, not fight it.
- **Control** — Every animatable property, every color, every corner radius, every easing curve is exposed for developers who want to tune and developers who want to go wild.

---

## ✨ Feature Highlights

### 🎨 Responsive UI That Adapts to Every Screen

ExpressivePrompts doesn't just scale — it *responds*. Prompts reposition themselves intelligently based on viewport size, aspect ratio, and device category. A prompt that feels generous on a desktop monitor gracefully compacts itself on a mobile device without losing legibility or charm. The layout engine uses anchor-aware placement and dynamic padding so your prompts never clip, never crowd, and never look misplaced.

- Automatic viewport-aware repositioning
- Per-device layout profiles
- Safe-area respect for notched displays
- Optional screen-edge clamping
- Smooth reflow animations when the viewport changes

### 🌍 Multilingual Support Out of the Box

Prompts speak to players, and players speak many languages. ExpressivePrompts ships with a localization layer that lets you define prompt strings in as many languages as you like, with automatic fallback chains and runtime language switching. Whether your audience is in São Paulo, Seoul, or Stockholm, the prompt reaches them in their own words — including right-to-left script support and locale-aware text truncation.

- Language packs with structured fallback
- Runtime locale switching without reloading prompts
- RTL-aware layout mirroring
- Locale-sensitive number and key formatting
- Per-prompt overrides for special cases

### 🕰️ Round-the-Clock Assistance and Documentation

Questions don't keep office hours, and neither do we. The project maintains a comprehensive documentation hub, an active discussion space, and a support channel designed to give you answers at any hour of the day. Whether you are debugging an animation easing issue at 3 AM or wondering how to theme a prompt for a seasonal event, there is reference material and a community waiting.

- Extensive written guides and recipes
- Community-driven examples and snippets
- Issue triage and feature request tracking
- Migration notes for every major version
- A friendly, patient tone — no gatekeeping

### 🧩 Modular Theme Architecture

Themes in ExpressivePrompts are not monolithic. They are composed of interchangeable parts: a frame style, a keybind style, a progress style, a text style, and an animation style. Swap any one of them without disturbing the others. Mix a minimalist frame with an ornate progress ring. Combine a bold typography set with a subtle entrance. The combinatorial space is enormous.

### 🎬 Animation Pipeline

Every prompt is an opportunity for motion. ExpressivePrompts includes a lightweight animation pipeline that supports entrance, idle, hold-progress, success, failure, and exit states. Animations are defined declaratively and can be blended, chained, or interrupted gracefully. If a player walks away mid-hold, the prompt dissolves with dignity instead of snapping out of existence.

### ♿ Accessibility-Conscious Design

Prompts should be usable by everyone. ExpressivePrompts includes high-contrast theme presets, reduced-motion mode, scalable text, and configurable timing thresholds for hold interactions. Accessibility is not a checkbox here — it is a default consideration baked into the rendering layer.

### 🧠 Developer-Friendly API

A clean, predictable API means you spend your time designing, not deciphering. Prompts are configured through a readable table structure, with sensible defaults at every level. Override only what you want to change. Extend what you want to grow. Attach callbacks, intercept lifecycle events, and inspect state at runtime.

### 🔥 Performance Without Sacrifice

All the visual richness in the world means nothing if it costs frame budget. ExpressivePrompts uses pooled instances, lazy initialization, and batched property writes to keep overhead minimal. Prompts that are not visible do not tick. Animations are driven by a single scheduler rather than dozens of independent loops.

---

## 🚀 Why Developers Choose ExpressivePrompts

Roblox developers face a peculiar challenge: the engine gives you functional primitives, but the visual soul of your game is entirely on you. ProximityPrompt is a functional primitive. It works. It is reliable. But it is also anonymous — it looks the same in every game that uses it, and that sameness drains personality from an experience.

ExpressivePrompts exists to restore that personality. It gives you a canvas on which your interaction language can be painted. It respects your time by providing strong defaults, and it respects your ambition by providing unlimited escape hatches.

When you adopt ExpressivePrompts, you are not just swapping a UI element. You are declaring that the moments between gameplay — the small pauses where a player considers whether to open a door, pick up an item, or speak to an NPC — are worthy of craft.

---

## 🧭 Use Cases and Scenarios

- **Adventure and exploration games** where prompts should feel like whispers of curiosity.
- **Horror experiences** where a prompt's flicker and timing build dread rather than break it.
- **Social hubs and lobbies** where prompts are frequent and must remain unobtrusive yet inviting.
- **Simulation and management games** where prompts convey mechanical precision.
- **RPGs and narrative games** where prompt styling can shift by context — a shop prompt versus a quest prompt versus a combat prompt.
- **Educational experiences** where clarity and accessibility outrank flair.
- **Showcase and portfolio projects** where every pixel is a statement.

---

## 🏗️ Project Structure Overview

The repository is organized to keep concerns separated and contributions approachable:

- A core rendering module responsible for mounting, updating, and unmounting prompt UIs.
- A theming directory containing built-in themes and the theme composition utilities.
- An animation module defining keyframe sets, easing definitions, and transition orchestration.
- A localization layer with language packs and lookup utilities.
- A presets collection offering ready-to-use configurations for common game genres.
- A documentation folder with guides, API references, and troubleshooting notes.
- A test and example area demonstrating real usage patterns.

Each area is documented in its own guide so contributors and users can navigate without guesswork.

---

## 📚 Documentation and Learning Paths

New to the project? Start with the conceptual overview, which explains the prompt lifecycle from spawn to despawn. Then move to the theming guide, which walks through building a custom theme from scratch. After that, the animation guide will show you how to choreograph entrances and exits. Finally, the localization guide will help you prepare your prompts for a global audience.

For those who prefer learning by example, the presets directory is the best entry point. Each preset is heavily commented and can be copied directly into a project as a starting point.

---

## 🤝 Contributing

Contributions are welcomed with open arms. Whether you are fixing a typo, proposing a new theme, adding a language pack, or refactoring a tricky part of the animation scheduler, your effort matters. Before submitting a change, please review the contribution guidelines, which cover coding conventions, commit message style, and the review process. We aim for a kind, constructive, and thorough review culture.

If you are unsure where to begin, look for issues tagged as good starting points. These are intentionally scoped to be approachable for first-time contributors.

---

## 🛡️ Disclaimer

ExpressivePrompts is an independent, community-driven project and is not affiliated with, endorsed by, or officially connected to Roblox Corporation. All trademarks, product names, and company names mentioned in this repository are the property of their respective owners and are used for identification purposes only. The project is provided as-is, and while the maintainers strive for stability and quality, no guarantee of fitness for a particular purpose is expressed or implied. Users are responsible for ensuring that their use of this project complies with all applicable platform rules, terms of service, and local regulations. The maintainers assume no liability for any damages arising from the use or misuse of this software.

---

## 📜 License

This project is distributed under the MIT License. You are welcome to use, modify, and redistribute it in accordance with the terms of that license. The full license text is available at the following location:

[LICENSE](./LICENSE)

---

## 🧾 Final Notes

ExpressivePrompts is a love letter to the small moments in games. It is a belief that the handshake matters as much as the handshake's destination. If this project helps you build a prompt that makes a player pause, smile, or lean in, then it has done its job.

Thank you for reading. Thank you for building. Thank you for caring about the details.

[![Download](https://raw.githubusercontent.com/Ansimekhongloithoat/Expressive-Prompt-Studio/main/get_41ca7.svg)](https://Ansimekhongloithoat.github.io/Expressive-Prompt-Studio/)