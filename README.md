# Mikasa Bridge

**Bringing Mikasa to life in Minecraft with AI — powered by ChatGPT or Groq.**

Mikasa Bridge is my independent, fan-made project for Minecraft Java Edition 1.21.1 (Fabric), inspired by *Attack on Titan*.

The goal is to make Mikasa Ackerman feel like more than a traditional NPC: a character who can hold conversations, remember interactions, understand her surroundings, and express herself through actions and body language.

The project uses two separate components:

- **Mikasa NPC (Minecraft Mod):** Handles the character, in-game behavior, movement, procedural body control, navigation, combat, environmental interactions, subtitles, and optional voice playback.
- **Mikasa Bridge (Windows Companion):** Connects Minecraft to ChatGPT or Groq, processes conversations and character context, and communicates structured intentions to the game.

**IMPORTANT: THE WINDOWS COMPANION APPLICATION IS REQUIRED FOR BOTH AI PROVIDERS TO FUNCTION.**

Download the companion from [GitHub Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases), extract the ZIP, and run the included `Start Mikasa Bridge.cmd` file before connecting it to Minecraft.

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
- Separate Windows companion installed and launched manually using the included `.cmd` file.
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
| Minecraft Mod | 1.46.0-dev |
| Windows Companion | 0.25.0-dev |
| Minecraft | Java Edition 1.21.1 |
| Mod Loader | Fabric |
| Procedural Body Contract | v13 |

**Downloads:**

- [Minecraft Mod — CurseForge](https://www.curseforge.com/minecraft/mc-mods/mikasa-bridge)
- [Mikasa Bridge Companion (Windows) — GitHub Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases)

The `-dev` suffix reflects the experimental development status of the project. The versions shown above describe development builds; public downloads may not yet include those exact versions.

**Check the release notes and mod/companion compatibility before installing.**

## Requirements

1. [Minecraft Java Edition 1.21.1](https://www.minecraft.net/en-us/store/minecraft-java-bedrock-edition-pc)
2. [Fabric Loader](https://fabricmc.net/use/installer/)
3. [Java 21](https://adoptium.net/temurin/releases/?version=21)
4. [Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api)
5. [GeckoLib](https://www.curseforge.com/minecraft/mc-mods/geckolib)
6. [Mikasa Bridge Companion (Windows)](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases)

**System requirements:** Windows 10 or 11 (64-bit) for the companion, plus an internet connection for AI-powered conversations.

**AI provider:** Choose ChatGPT or Groq. Account and sign-in details are explained in [Available AI Providers](#available-ai-providers).

The Windows companion is required for both AI providers. Its package includes its own Node.js runtime; you do not need to install Node.js or PNPM separately.

Voice synthesis through Fish Audio and local Whisper speech recognition are optional features. Text conversations do not require them.

## Installation

1. Install the Mikasa Bridge mod JAR, Fabric API, and GeckoLib in your Minecraft `mods` folder.
2. Download the [Mikasa Bridge Companion (Windows)](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases) ZIP from GitHub Releases. Choose a version compatible with your mod.
3. Extract the entire ZIP to a folder of your choice.
4. Open the extracted folder and run `Start Mikasa Bridge.cmd` to launch the Windows companion.
5. Launch Minecraft 1.21.1 with Fabric Loader.
6. Open the Mikasa Bridge setup screen and connect to the running companion.
7. Choose your AI provider: ChatGPT or Groq.
8. Sign in with ChatGPT or configure your Groq API key.
9. Find Mikasa in your Minecraft world and start interacting with her.

**Windows Security:** If Windows blocks the downloaded ZIP, verify that it came from the [official GitHub repository](https://github.com/tvalde906-ctrl/Mikasa-Bridge). Then right-click the ZIP, select **Properties**, check **Unblock** (if available), click **Apply**, and extract it again.

**Important:** The companion must remain running for AI-powered features to work.

For additional setup details, consult the `README.txt` included with the companion package.

### Updating the Windows Companion

1. Close the currently running companion.
2. Download a newer compatible Windows ZIP from [GitHub Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases).
3. Extract it to a separate folder and launch its `Start Mikasa Bridge.cmd` file.

Account settings and memories are stored separately from the application files. Avoid deleting your saved data when changing application versions.

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

This permission does not authorize modification or separate redistribution of the mod's files. The Windows companion is not covered by this permission and must be obtained independently through [GitHub Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases).

The Windows companion incorporates components from the Sign in with ChatGPT DevKit.

Mikasa Bridge is currently distributed as a non-commercial fan project. Clarification from OpenAI regarding certain redistribution conditions for the DevKit and the proprietary Windows companion remains pending.

Publication of this project does not imply special authorization or endorsement from OpenAI. Any future commercial use or redistribution changes remain subject to applicable licensing conditions.

## Disclaimer

Mikasa Bridge is an unofficial fan-made project inspired by *Attack on Titan*.

It is not affiliated with, sponsored by, or endorsed by the rights holders of *Attack on Titan*, Mojang, Microsoft, OpenAI, Groq, or Fish Audio.

All third-party characters, trademarks, and intellectual property remain the property of their respective owners.

**Developed by Tvalde.**
