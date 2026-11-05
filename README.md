# Mikasa Bridge

**Bringing Mikasa to life in Minecraft with ChatGPT.**

Mikasa Bridge is my independent, fan-made project for **Minecraft Java Edition 1.21.1 (Fabric)**. The goal is to make Mikasa Ackerman feel like more than a traditional NPC: someone who can hold conversations, remember interactions, react to her surroundings, and express herself through actions and body language.

The project uses two separate components:

- **Mikasa NPC (Minecraft mod):** character, in-game behavior, movement, body controller, navigation, combat, environmental interactions, subtitles, and optional voice playback.
- **Mikasa Bridge (Windows companion):** connects the mod to ChatGPT using Sign in with ChatGPT, processes dialogue and character context, and passes structured intentions back to Minecraft.

You sign in with your **own eligible ChatGPT account**; no conventional OpenAI API key is needed.

## Features

- **AI-powered conversations** with contextual responses and Mikasa's character personality.
- **Persistent memory**, including meaningful interactions and selected body-language moments.
- **Environmental awareness** based on information available to the Minecraft mod: players, entities, nearby blocks, and situations.
- **In-game behaviors** such as following, staying, guarding, navigation, and combat.
- **Mikasa's cabin and first-encounter system**.
- **Multilingual dialogue** and progressive subtitles.
- **Optional Fish Audio voice synthesis** and optional local speech recognition using Whisper.
- **Experimental procedural body language**: ChatGPT can specify what it wants Mikasa to express, while Minecraft's local movement engine chooses and validates ways to execute it.

### Experimental body movement

This is one of the most ambitious parts of the project, and it's still at a **very early stage**.

The aim is for ChatGPT, Minecraft, the procedural movement engine, and optional Fish Audio to work together so Mikasa can express herself more naturally **without needing a unique, fixed animation for every gesture**.

The current experimental system explores:

- Gestures related to the meaning and timing of speech.
- Continuous arm and hand placement, wrist/palm orientation, and individual finger movement.
- Body-relative goals, such as resting a hand on her chest or shoulder, and relational poses such as crossed arms.
- Persistent postures, including sitting and leaning against nearby surfaces.
- Collision checks, joint limits, ergonomic choices, and alternative movement paths.
- Feedback indicating what Minecraft's movement engine was able to execute, including some moments worth remembering.

**Important:** this isn't unrestricted physical intelligence. The system still uses existing animation clips where appropriate, the available character rig, and procedural rules. Gestures may look awkward or fail, and ChatGPT does **not** directly control individual animation frames or see the rendered result.

Truly freeform, context-aware body movement is very difficult. I don't know whether I'll ever reach the level of freedom and naturalness I have in mind, but I plan to keep trying different approaches and improving it.

## Versions and download status

| Component | Latest publicly listed release at the time of this README update | New development build |
| --- | --- | --- |
| Minecraft mod | **1.29.0** on CurseForge | **1.35.1-dev** (experimental) |
| Windows companion | **0.9.3 Beta** on GitHub | **0.16.0-dev** (experimental) |

**The development builds listed above are not automatically available for public download.** The Windows 0.16.0-dev package is currently prepared for review only and has unresolved distribution conditions. Do not mix a new mod with an older companion unless their compatibility has been verified. The new development pair still requires final Minecraft end-to-end checks.

- **Minecraft mod:** [CurseForge — Mikasa Bridge](https://www.curseforge.com/minecraft/mc-mods/mikasa-bridge)
- **Windows companion:** [GitHub Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases)

Check the requirements shown on the **specific files you download**, rather than assuming all releases work together.

## Requirements

- Minecraft Java Edition **1.21.1**.
- Fabric Loader, Fabric API, and GeckoLib compatible with the selected mod release.
- **Java 21** for Minecraft.
- **Windows 10 or 11, 64-bit** for the companion application.
- Internet connection for ChatGPT interactions.
- An eligible ChatGPT account and subscription for Sign in with ChatGPT inference.

**Optional:** Fish Audio account/API key for voice synthesis; microphone and a separately downloaded Whisper model for local speech recognition. Neither is required for text conversations.

## Installation

1. Install Minecraft 1.21.1 with Fabric Loader, Fabric API, and GeckoLib.
2. Download a supported Mikasa Bridge mod JAR from CurseForge and put it in your Minecraft `mods` folder.
3. Download the **compatible** Windows companion ZIP from GitHub Releases.
4. On Windows, if the ZIP is blocked, use **Properties → Unblock** on the ZIP *before* extracting it. Keep Windows security features enabled.
5. Extract the full ZIP into its own folder; don't run it from inside the archive.
6. Open `Start Mikasa Bridge.cmd` and choose **Continue with ChatGPT**.
7. Complete authorization in the browser and return to the companion application.
8. Start Minecraft and interact with Mikasa. Keep the Windows companion running for AI-powered interactions.

The package contains a detailed `README.txt`, including troubleshooting and optional microphone setup. Some features may differ between versions.

## Development status

**EXPECT BUGS — EXPERIMENTAL / WORK IN PROGRESS**

Mikasa Bridge is an ongoing personal project. AI-driven movements, autonomous postures, environment interactions, and speech synchronization can behave inconsistently. Automated tests are useful, but they do not replace observing the character inside Minecraft.

Future goals include richer object interactions, procedural locomotion, more complex action planning, better environmental perception, and improved movement ergonomics. I am also considering reuse of successful motor solutions to reduce computation time, where profiling shows that it would help.

Feel free to use [GitHub Issues](https://github.com/tvalde906-ctrl/Mikasa-Bridge/issues) to report reproducible bugs or suggest improvements. Please **do not upload account tokens, private conversations, or other sensitive files**.

## Licensing and distribution

The original code and assets independently developed for Mikasa Bridge remain proprietary unless stated otherwise. Third-party software and modifications retain their own licenses, notices, and restrictions.

The Windows companion includes components from the **Sign in with ChatGPT DevKit**. Clarification regarding the intended distribution of the modified DevKit and the proprietary Windows companion is still pending. Preparing a build or passing automated tests does not itself authorize public redistribution or commercial use.

## Disclaimer

Mikasa Bridge is an **unofficial fan-made project** inspired by *Attack on Titan*. It is not affiliated with, sponsored by, or endorsed by the rights holders of *Attack on Titan*, Mojang, Microsoft, OpenAI, or Fish Audio. All third-party characters, trademarks, and other intellectual property remain the property of their respective owners.

**Developed by Tvalde.**
