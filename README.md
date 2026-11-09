# Mikasa Bridge

**Bringing Mikasa to life in Minecraft with AI — powered by ChatGPT or Groq.**

Mikasa Bridge is my independent, fan-made project for Minecraft Java Edition 1.21.1 (Fabric), inspired by *Attack on Titan*.

The goal is to make Mikasa Ackerman feel like more than a traditional NPC: a character who can hold conversations, remember interactions, understand her surroundings, and express herself through actions and body language.

The project uses two separate components:

- **Mikasa NPC (Minecraft Mod):** Handles the character, in-game behavior, movement, procedural body control, navigation, combat, environmental interactions, subtitles, and optional voice playback.
- **Mikasa Bridge (Windows Companion):** Connects Minecraft to ChatGPT or Groq, processes conversations and character context, and communicates structured intentions to the game.

**IMPORTANT: THE WINDOWS COMPANION APPLICATION IS REQUIRED FOR BOTH AI PROVIDERS TO FUNCTION.**

The companion can now be downloaded and installed directly through Minecraft with the player's permission. Manual installation remains available.

## Available AI Providers

Mikasa Bridge supports two AI providers. Both use the same character systems, persistent memory, and in-game capabilities.

### ChatGPT — Paid (Recommended)

**Requires an eligible ChatGPT Plus or Pro subscription.**

ChatGPT is currently recommended for a more reliable experience with Mikasa Bridge.

**Advantages:**
- More consistent results with the project's current AI integration.
- Better suited to its complex conversations and structured actions.
- Generally more comfortable usage availability for this project, subject to the applicable subscription limits.

**Disadvantages:**
- Requires a paid subscription.
- Response times and usage availability may vary.

ChatGPT uses **Sign in with ChatGPT**, allowing players to authorize the companion with their own eligible account. A conventional OpenAI API key is not required.

### Groq — Free Alternative

**No paid ChatGPT subscription required.**

Groq allows players to connect Mikasa to AI using their own Groq account and API key, with free-tier access available.

**Advantages:**
- Free-tier access.


**Disadvantages:**
- Stricter token and usage limits.
- Occasional rate-limit and structured-response errors.
- Integration improvements are still in progress.

**Recommendation:** ChatGPT Plus or Pro is currently recommended, while Groq provides an accessible alternative for players who want to try Mikasa Bridge without a paid ChatGPT subscription.

The selected provider can be changed without separating or deleting Mikasa's existing memories.

## Features

- AI-powered conversations with contextual responses and Mikasa's character personality.
- Persistent memory, including meaningful interactions and selected body-language moments.
- Environmental awareness based on information available to the Minecraft mod.
- In-game behaviors such as following, staying, guarding, navigation, and combat.
- Mikasa's cabin and first-encounter system.
- Context-aware autonomy and initiative.
- Interactions with items, including picking them up, holding them, and handing them over.
- Multilingual dialogue and progressive subtitles.
- Optional Fish Audio voice synthesis and local Whisper speech recognition.
- Experimental procedural body language and dynamic gestures.
- Automatic Windows companion installation, startup, and assisted updates.
- AI communication and token-usage optimizations.

Some features remain experimental and may behave inconsistently.

## Experimental Body Movement

Procedural body movement is one of the most ambitious parts of Mikasa Bridge and remains under active development.

The goal is to let the selected AI provider, Minecraft's movement engine, and optional voice systems work together so Mikasa can move, react, and express herself naturally without requiring a fixed animation for every possible gesture.

The current system explores:

- Gestures influenced by conversation context, meaning, and speech timing.
- Dynamic arm, hand, wrist, palm, and individual finger movement.
- Body-relative goals, such as touching reachable body areas.
- Relational gestures, including crossed arms and coordinated limb positioning.
- Persistent postures, including sitting, leaning, and interactions with nearby surfaces.
- Procedural ergonomics, joint coordination, and collision avoidance.
- Alternative movement trajectories and adaptive body positioning.
- Feedback between Minecraft's movement engine and the selected AI provider.
- Selective memory of meaningful gestures and physical interactions.

**Important:** This is not unrestricted physical intelligence.

The AI does not directly animate individual frames or visually observe the final rendered movements. It communicates intentions, while Minecraft's local movement engine calculates, validates, and attempts to execute them.

Movements may still look unnatural, repetitive, inaccurate, or fail entirely.

Achieving truly flexible, context-aware body movement is an ongoing experiment. The goal is not simply to add more animations, but to give Mikasa greater freedom to express herself through dynamically generated movements.

## Downloads and Versions

### Current Development Builds

| Component | Version |
|---|---|
| Minecraft Mod | 1.44.2-dev |
| Windows Companion | 0.24.0-dev |
| Minecraft | Java Edition 1.21.1 |
| Mod Loader | Fabric |
| Procedural Body Contract | v13 |

**Official Downloads:**

- [Minecraft Mod — CurseForge](https://www.curseforge.com/minecraft/mc-mods/mikasa-bridge)
- [Windows Companion — Latest Release](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases/latest)
- [All GitHub Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases)

The `-dev` suffix reflects the experimental development status of the project, even when a build is publicly released.

Always check the available release and compatibility information before installing.

### Update Manifest

The [Mikasa Bridge Update Manifest](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases/tag/bridge-manifest) contains signed information used by the Minecraft mod to locate and verify companion downloads.

These manifest files are intended for the automatic installation and update system. Players do not need to download them manually.

## Requirements

### Minecraft and Dependencies

- Minecraft Java Edition 1.21.1.
- Fabric Loader.
- Fabric API 0.116.17 or a newer compatible version.
- GeckoLib 4.9.3 or a newer compatible version.
- Java 21.
- Windows 10 or 11 (64-bit) for the companion application.
- Internet connection for AI-powered conversations.

### AI Provider

Choose one:

- **ChatGPT:** An eligible Plus or Pro subscription.
- **Groq:** A Groq account and API key, with free-tier access available.

### Windows Companion

**Mikasa Bridge Windows is indispensable for both ChatGPT and Groq to function with the Minecraft mod.**

The companion application is separate from the Minecraft JAR. It can be installed through the in-game setup system or downloaded manually.

The Windows package includes its own Node.js runtime. Players do not need to install Node.js or PNPM separately.

### Optional Features

- **Fish Audio:** Account and API key for Mikasa's synthesized voice.
- **Whisper:** Local speech recognition for microphone input. A one-time model download is required.
- **Microphone:** Needed only for voice input.

Voice synthesis and speech recognition are optional. Text conversations work without either service.

## Installation

### Option 1 — Automatic Installation (Recommended)

Starting with the latest versions, Minecraft can guide players through installing the separate Windows companion application.

1. Install Minecraft 1.21.1 with Fabric Loader.
2. Install Fabric API and GeckoLib.
3. Download the Mikasa Bridge mod from CurseForge.
4. Place the mod JAR in your Minecraft `mods` folder.
5. Launch Minecraft.
6. Open the Mikasa Bridge setup screen.
7. Select the companion installation option and review the download information.
8. Authorize the download and installation.
9. Choose ChatGPT or Groq and configure your account.
10. Find Mikasa in your Minecraft world and start interacting with her.

The installer downloads the official Windows companion from GitHub and verifies the package before installation.

With the player's permission, Minecraft can also launch the managed companion application and assist with compatible updates.

Existing accounts, memories, and settings are stored separately from the managed application files and are preserved during updates.

**The companion is not embedded inside the Minecraft JAR. Minecraft downloads it separately from the official repository.**

### Option 2 — Manual Installation

Players who prefer manual installation can still manage the Windows companion themselves.

1. Install the Minecraft mod and its required dependencies.
2. Visit [Mikasa Bridge — Latest Release](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases/latest).
3. Download the Windows companion ZIP.
4. Extract the complete ZIP into a separate folder.
5. Launch `Start Mikasa Bridge.cmd`.
6. Choose ChatGPT or Groq and complete the corresponding setup.
7. Launch Minecraft and interact with Mikasa.

If Windows flags the downloaded file, verify that it came from the official repository before taking any action. Keep Windows security protections enabled.

The Windows companion must remain running for AI-powered features to work.

### Automatic Update Checks

When enabled, the Minecraft mod checks GitHub once per game launch for compatible companion information.

The system can offer an installation or update when required. Compatible existing installations are not automatically replaced simply because a newer version is available.

Downloads and installations require player consent.

Automatic update checks can be disabled.

## How to Talk to Mikasa

**Stand in front of Mikasa and press `R` to open the interaction interface.**

From there, you can communicate through text or use optional microphone and voice features.

Minecraft provides the selected AI with information about Mikasa's surroundings, memories, and available actions. The game validates and executes supported actions locally.

## Development Status

**EXPECT BUGS — EXPERIMENTAL / WORK IN PROGRESS**

Mikasa Bridge is an ongoing personal project.

Many systems are still being developed, particularly procedural movement, autonomous behavior, physical interactions, environmental awareness, and coordination between conversation, gestures, and speech.

The new Groq integration may occasionally encounter token-limit, rate-limit, or structured-response errors.

During conversations, Mikasa may reflect on her own capabilities, identify potential limitations, or suggest improvements. These observations are not always accurate or verified.

### Future Development Goals

- More reliable Groq integration and better handling of provider limits.
- Lower perceived response latency and improved voice playback.
- Streaming audio playback synchronized with progressive subtitles.
- More complex physical interactions with objects and the environment.
- Procedural locomotion and improved movement transitions.
- Multi-step action planning and autonomous behavior.
- More advanced environmental perception.
- Improved ergonomic movement and natural body language.
- Better coordination between speech, emotions, gestures, and physical actions.
- Continued experimentation with flexible, context-aware body movement.

The project will continue evolving through experimentation, testing, and gradual improvements.

Feel free to use [GitHub Issues](https://github.com/tvalde906-ctrl/Mikasa-Bridge/issues) to report reproducible bugs or suggest improvements.

**Please do not upload account tokens, API keys, private conversations, credentials, or other sensitive information.**

## Licensing and Distribution

The original code and assets independently developed for Mikasa Bridge remain proprietary unless explicitly stated otherwise.

Third-party software, libraries, and modifications retain their respective licenses, notices, and distribution requirements.

**Modpack Inclusion:** Mikasa Bridge may be included in CurseForge modpacks through the official CurseForge manifest system, provided the original mod files remain unmodified.

This permission does not authorize modification or separate redistribution of the mod's files. The Windows companion is not covered by this permission and must be obtained independently through the official installation system or releases.

The Windows companion incorporates components from the Sign in with ChatGPT DevKit.

Mikasa Bridge is currently distributed as a non-commercial fan project. Clarification from OpenAI regarding certain redistribution conditions for the DevKit and the proprietary Windows companion remains pending.

Publication of this project does not imply special authorization or endorsement from OpenAI. Any future commercial use or redistribution changes remain subject to applicable licensing conditions.

## Disclaimer

Mikasa Bridge is an unofficial fan-made project inspired by *Attack on Titan*.

It is not affiliated with, sponsored by, or endorsed by the rights holders of *Attack on Titan*, Mojang, Microsoft, OpenAI, Groq, or Fish Audio.

All third-party characters, trademarks, and intellectual property remain the property of their respective owners.

**Developed by Tvalde.**
