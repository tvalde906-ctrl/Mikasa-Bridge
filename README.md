# Mikasa Bridge

**Bringing Mikasa to life in Minecraft with ChatGPT.**

Mikasa Bridge is my personal project for Minecraft Java Edition 1.21.1, built using Fabric.

My goal is to bring Mikasa Ackerman from *Attack on Titan* into Minecraft as more than just a traditional NPC. I want her to be able to hold conversations, remember previous interactions, understand what's happening around her, and interact with the Minecraft world.

The project combines a Minecraft mod with a separate Windows application that connects Mikasa to ChatGPT.

## How It Works

Mikasa Bridge has two main components:

- **Mikasa NPC:** The Minecraft mod, which handles Mikasa's character, animations, movement, combat, interactions, and other in-game mechanics.
- **Mikasa Bridge Windows:** A companion application that runs locally on Windows and connects the mod to ChatGPT through Sign in with ChatGPT.

You sign in using your own eligible ChatGPT account. You don't need a conventional OpenAI API key.

## Features

Here's what I've implemented so far:

- AI-powered conversations with contextual responses
- Mikasa's personality and persistent memories
- Awareness of nearby players, entities, and the environment
- Following, navigation, guarding, and combat behaviors
- Custom animations, dual blades, and ODM-inspired movement
- Mikasa's cabin and a first encounter system
- Multilingual conversations and progressive subtitles
- Optional voice synthesis through Fish Audio

I'm still working on improving these systems, so some features may not always behave as expected.

## Requirements

- Minecraft Java Edition 1.21.1
- Fabric Loader
- Fabric API
- GeckoLib
- Java 21
- Windows for the companion application
- An eligible ChatGPT account and subscription

Additional configuration or services may be needed for optional voice features.

## Downloads

### Minecraft Mod

You can find the Minecraft mod on CurseForge:

**[Mikasa Bridge — CurseForge](https://www.curseforge.com/minecraft/mc-mods/mikasa-bridge)**

### Windows Companion

The companion application is distributed separately through GitHub Releases:

**[Mikasa Bridge — Releases](https://github.com/tvalde906-ctrl/Mikasa-Bridge/releases)**

Make sure you're using compatible versions of the Minecraft mod and Windows companion.

## Installation

1. Install Minecraft Java Edition 1.21.1 with Fabric Loader.
2. Install Fabric API and GeckoLib.
3. Place the Mikasa NPC JAR in your Minecraft `mods` folder.
4. Download the Windows companion ZIP from GitHub Releases.
5. Extract the ZIP into a separate folder.
6. Start the companion using the included Windows launcher.
7. Follow the Sign in with ChatGPT authorization process.
8. Launch Minecraft with Mikasa NPC installed.

The Windows companion needs to be running for the ChatGPT-powered features to work.

## Development Status

**Beta — Work in Progress**

Mikasa Bridge is still an experimental project.

I've spent a lot of time working on its different systems, but there's still plenty I want to improve, especially Mikasa's behavior, interactions, and ability to act naturally within Minecraft.

You may encounter bugs, unexpected behavior, or features that aren't completely finished.

If you run into a problem, feel free to report it through GitHub Issues.

## Licensing

I'm sharing Mikasa Bridge as a free fan-made project.

The original code and assets I've developed remain proprietary unless stated otherwise. Third-party components have their own licenses, notices, and applicable terms.

I'm also reviewing the redistribution conditions associated with the Sign in with ChatGPT DevKit. This project is not officially affiliated with or endorsed by OpenAI.

## Disclaimer

Mikasa Bridge is an unofficial fan-made project.

It is not affiliated with or endorsed by the creators or rights holders of *Attack on Titan*, Mojang, Microsoft, OpenAI, or Fish Audio.

All third-party characters, trademarks, and intellectual property belong to their respective owners.
