# Mikasa Bridge

**Bringing Mikasa to life in Minecraft with ChatGPT.**

Mikasa Bridge is my independent, fan-made project for **Minecraft Java Edition 1.21.1 (Fabric)**.

The goal is to make Mikasa Ackerman feel like more than a traditional NPC: someone who can hold conversations, remember interactions, react to her surroundings, and express herself through actions and body language.

The project uses two separate components:

- **Mikasa NPC (Minecraft mod):** Handles the character, in-game behavior, movement, procedural body controller, navigation, combat, environmental interactions, subtitles, and optional voice playback.
- **Mikasa Bridge (Windows companion):** Connects the mod to ChatGPT using Sign in with ChatGPT, processes dialogue and character context, and sends structured intentions back to Minecraft.

You sign in with your **own eligible ChatGPT account**; no conventional OpenAI API key is needed.

## Features

- **AI-powered conversations** with contextual responses and Mikasa's character personality.
- **Persistent memory**, including meaningful interactions and selected body-language moments.
- **Environmental awareness** based on information available to the Minecraft mod, including players, entities, nearby blocks, and situations.
- **In-game behaviors** such as following, staying, guarding, navigation, and combat.
- **Mikasa's cabin and first-encounter system.**
- **Multilingual dialogue** and progressive subtitles.
- **Optional Fish Audio voice synthesis** and local speech recognition using Whisper.
- **Experimental procedural body language**, allowing ChatGPT to express physical intentions while Minecraft's local movement engine calculates and validates their execution.
- **Dynamic gestures and postures**, combining existing animations with procedural movement to create more varied expressions.

### Experimental Body Movement

This is one of the most ambitious parts of Mikasa Bridge, and it's still at a **very early experimental stage**.

The idea is to make ChatGPT, Minecraft, the procedural movement engine, and optional Fish Audio work together so Mikasa can move, react, and express herself more naturally, without requiring a fixed animation for every possible gesture.

The current system explores:

- Gestures influenced by conversation context, meaning, and speech timing.
- Dynamic arm, hand, wrist, palm, and individual finger movement.
- Body-relative goals, such as touching her chest, shoulder, or other reachable body areas.
- Relational gestures, including crossed arms and coordinated limb positioning.
- Persistent postures, including sitting, leaning, and interacting with nearby surfaces.
- Procedural ergonomics, joint coordination, and collision avoidance.
- Alternative movement trajectories and adaptive body positioning.
- Feedback between the movement engine and ChatGPT.
- Selective memory of meaningful gestures and physical interactions.

**Important:** this is not unrestricted physical intelligence. The system still relies on the character's existing skeleton, procedural calculations, and traditional animation clips where appropriate.

ChatGPT does not directly animate individual frames or visually observe the final rendered movements. Instead, it communicates intentions, and Minecraft's movement engine attempts to execute them.

Movements can still look unnatural, repetitive, inaccurate, or fail entirely.

Achieving truly freeform, context-aware body movement is an incredibly difficult challenge. I'm not even sure whether I'll ever achieve the level of freedom and naturalness I have in mind, but I intend to keep experimenting with different approaches and seeing how far I can take it.

**The goal is not simply to add more animations, but to give Mikasa greater freedom to express herself through dynamically generated movements.**

## Downloads and Versions

### Current Releases

| Component | Version |
| --- | --- |
| **Minecraft Mod** | **1.35.1-dev** |
| **Windows Companion** | **0.16.0-dev** |
| Minecraft | Java Edition 1.21.1 |
| Mod Loader | Fabric |
| Body Movement Contract | v12 |

Both components are available through their respective release pages.

- **Minecraft Mod:** [CurseForge — Mikasa Bridge](https://www.curseforge.com/minecraft/mc-mods/mikasa-bridge)
- **Windows Companion:** [GitHub Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases)

**Important:** Make sure the Minecraft mod and Windows companion versions are compatible. Older releases may use different communication protocols and may not work correctly with newer versions.

The `-dev` suffix reflects the ongoing experimental development of the project, even when a build is publicly released.

## Requirements

- Minecraft Java Edition **1.21.1**.
- Fabric Loader.
- Fabric API and GeckoLib compatible with the selected mod.
- **Java 21** for Minecraft.
- **Windows 10 or 11 (64-bit)** for the companion application.
- Internet connection for ChatGPT interactions.
- An eligible ChatGPT account and subscription for Sign in with ChatGPT.

**Optional:**

- Fish Audio account/API key for voice synthesis.
- Microphone for speech input.
- Separately downloaded Whisper model for local speech recognition.

Voice synthesis and speech recognition are optional. Text conversations do not require them.

## Installation

1. Install **Minecraft 1.21.1** with Fabric Loader.
2. Install the required Fabric API and GeckoLib dependencies.
3. Download **Mikasa Bridge 1.35.1-dev** from CurseForge.
4. Place the mod JAR inside your Minecraft `mods` folder.
5. Download **Mikasa Bridge Windows 0.16.0-dev** from GitHub Releases.
6. If Windows blocks the downloaded ZIP, open its **Properties → Unblock** option before extracting it. Keep Windows security features enabled.
7. Extract the complete ZIP into a separate folder.
8. Open `Start Mikasa Bridge.cmd`.
9. Select **Continue with ChatGPT** and complete authorization in your browser.
10. Start Minecraft and interact with Mikasa.

Keep the Windows companion running while using AI-powered features.

The Windows package includes its own Node.js runtime, so a separate Node.js or PNPM installation is not required.

The ZIP also contains documentation and additional instructions for optional voice features.

## Development Status

**EXPECT BUGS — EXPERIMENTAL / WORK IN PROGRESS**

Mikasa Bridge is an ongoing personal project.

Many systems are still being developed, especially procedural body movement, autonomous behavior, environmental interactions, and synchronization between conversations, gestures, and speech.

Some features may behave inconsistently, and the experience can vary depending on the situation, the AI response, and the limitations of Minecraft's movement engine.

### Future Development Goals

- More complex physical interactions with objects and the environment.
- Procedural locomotion and improved movement transitions.
- Multi-step action planning and autonomous behavior.
- More advanced environmental perception.
- Improved ergonomic movement and natural body language.
- Better coordination between speech, emotions, gestures, and physical actions.
- Possible reuse of successful motor solutions to reduce unnecessary computation and improve response times.
- Continued experimentation with more flexible, context-aware body movement.

The project will continue evolving through experimentation, testing, and gradual improvements.

Feel free to use [GitHub Issues](https://github.com/tvalde906-ctrl/Mikasa-Bridge/issues) to report reproducible bugs or suggest improvements.

**Please do not upload account tokens, private conversations, credentials, or other sensitive information.**

## Licensing and Distribution

The original code and assets independently developed for Mikasa Bridge remain proprietary unless explicitly stated otherwise.

Third-party software, libraries, and modifications retain their respective licenses, notices, and distribution requirements.

The Windows companion incorporates components from the **Sign in with ChatGPT DevKit**.

Mikasa Bridge is currently published as a **non-commercial fan project**, while clarification from OpenAI regarding the intended distribution of the modified DevKit and the proprietary Windows companion remains pending.

This publication does not imply special authorization or endorsement from OpenAI. Any future commercial use or redistribution changes remain subject to the applicable licensing conditions.

## Disclaimer

Mikasa Bridge is an **unofficial fan-made project** inspired by *Attack on Titan*.

It is not affiliated with, sponsored by, or endorsed by the rights holders of *Attack on Titan*, Mojang, Microsoft, OpenAI, or Fish Audio.

All third-party characters, trademarks, and other intellectual property remain the property of their respective owners.

**Developed by Tvalde.**
