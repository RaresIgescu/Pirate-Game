# 🏴‍☠️ Lost Island of Whispering Skulls

**A 2D Adventure Game built with Godot Engine.**  
Explore mysterious islands, collect treasures, and avoid hidden dangers in a pirate-themed quest filled with secrets.

---

## 🕹️ Gameplay Overview

You play as a **treasure hunter pirate** navigating from island to island. Each level presents unique challenges, enemies, and collectible items. The player can interact with NPCs, collect keys to unlock magical totems, and pause the game to access the inventory or settings.

### ✅ Completed Features

- 🌴 Fully implemented **Start Menu** (Help, Settings, Level Select)
- 🏝️ **3 playable levels** with increasing difficulty and new environments
- 👤 Character Controller (player)
- 🧟 Enemy AI with patrol and chase behavior
- 🗺️ Level Design using TileMaps and background parallax elements
- 🔑 Key and Totem system to unlock progress
- 🎒 Inventory System (toggle with **I**)
- 🎮 Pause Menu (toggle with **ESC**)
- 🧙 Interactive NPCs with dynamic pirate-style dialogue
- 🔊 Scene-based background music

---

## 🧱 Project Architecture

The game is structured modularly using Godot's scene system:

```
StartScene
├── Background (TileMap)
└── Menu (Instanced Scene)

LevelX (x = 1 to 3)
├── Player (CharacterBody2D)
├── Enemies (Instanced scenes)
├── Inventory (Instanced, toggled)
├── Totem (Unlockable via key)
├── Environment (TileMap + decorations)
└── PauseMenu (shared menu)
```

Scripts are written in **GDScript** and attached to specific nodes or scenes. Transitions between levels and menus are managed using `get_tree().change_scene_to_file(...)`.

---

## 🔧 Tech Stack

- 🎮 **Godot Engine** 4.x
- 🎨 Custom Pixel Art & PNG-based assets
- 🧠 GDScript for scripting logic
- 🛠️ Git & GitHub for version control and collaboration

---

## 🤝 Team & Collaboration

This project was developed by a team of 3 students using a clean and efficient Git workflow:

- Feature-based branches (`feature/menu`, `feature/level3`, etc.)
- Pull Requests and code reviews
- Frequent and descriptive commit messages
- Merging only after full testing

---

## 🚀 Getting Started

### Requirements

- [Godot Engine 4.x](https://godotengine.org/download)

### How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/RaresIgescu/Pirate-Game
   cd Pirate-Game
   ```

2. Open the project in Godot Engine.

3. Press `F5` to play the game.

---

## 📜 License

This project is for academic and personal learning purposes.

---

## 🏴‍☠️ Special Thanks

To our professors and classmates for feedback and support during development.
