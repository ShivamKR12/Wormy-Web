# Wormy

A classic snake-like arcade game built with Python and Pygame. Guide your worm across the grid, eat apples to grow, and avoid hitting the walls or yourself!

![Wormy Gameplay](https://img.shields.io/badge/Status-Stable-brightgreen)
![Python Version](https://img.shields.io/badge/Python-3.7+-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [How to Play](#how-to-play)
- [Controls](#controls)
- [Building from Source](#building-from-source)
- [Requirements](#requirements)
- [Project Structure](#project-structure)
- [License](#license)

## Features

- **Classic Gameplay** - Addictive snake-style mechanics with smooth controls
- **Score Tracking** - Real-time score display as you consume apples
- **Smooth Animation** - 15 FPS gameplay with responsive input handling
- **Grid-Based Movement** - 32x24 cell grid system for precise movement
- **Start & Game Over Screens** - Polished UI with animated title screen
- **Keyboard Controls** - Support for both WASD and arrow keys
- **Windows Executable** - Pre-built .exe for easy distribution and launch

## Installation

### Option 1: Run Pre-Built Executable (Recommended for Windows)

Download the latest `wormy.exe` from the `dist/` folder and run it directly. No Python installation required!

```bash
# Simply double-click wormy.exe
```

### Option 2: Run from Python Source

1. **Install Python 3.7 or higher** from [python.org](https://www.python.org/downloads/)

2. **Install dependencies:**
   ```bash
   pip install pygame
   ```

3. **Run the game:**
   ```bash
   python wormy.py
   ```

## How to Play

1. **Start Screen** - Press any key to begin the game
2. **Objective** - Navigate your worm to eat red apples and grow longer
3. **Scoring** - Each apple eaten adds 1 point to your score
4. **Game Over** - Collide with a wall or your own body to end the game
5. **Restart** - Press any key at the game over screen to play again

## Controls

| Key | Action |
|-----|--------|
| **↑** or **W** | Move Up |
| **↓** or **S** | Move Down |
| **←** or **A** | Move Left |
| **→** or **D** | Move Right |
| **ESC** | Exit Game |

## Building from Source

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)

### Build Instructions

1. **Clone or download this repository**

2. **Install required packages:**
   ```bash
   pip install pygame pyinstaller
   ```

3. **Generate the Windows executable:**
   ```bash
   pyinstaller --onefile --windowed --icon=wormy.ico wormy.py
   ```

4. **Locate the executable:**
   ```
   dist/wormy.exe
   ```

The executable will be found in the `dist/` folder and can be distributed standalone without requiring Python or dependencies.

### Build Output

- **`build/`** - Temporary build files (intermediate compilation artifacts)
- **`dist/`** - Final executable output (`wormy.exe`)
- **`wormy.spec`** - PyInstaller specification file

## Requirements

### For Running from Source

- Python 3.7+
- pygame 2.0+

### For Running the Executable

- Windows 7 or later
- No additional software required

### For Building

- Python 3.7+
- pygame 2.0+
- PyInstaller 5.0+

## Project Structure

```
wormy/
├── wormy.py              # Main game source code
├── wormy.ico             # Game icon (for title bar and executable)
├── wormy.png             # Alternative icon asset
├── README.md             # This file
├── .gitignore            # Git ignore configuration
├── build/                # Build artifacts (auto-generated)
├── dist/                 # Compiled executable output
└── screenshots/          # Game screenshots and media
```

## Game Technical Details

### Game Settings

- **Window Resolution** - 640x480 pixels
- **Cell Size** - 20x20 pixels
- **Grid Dimensions** - 32x24 cells
- **Frame Rate** - 15 FPS
- **Initial Worm Length** - 3 segments

### Color Scheme

| Element | Color |
|---------|-------|
| Background | Black |
| Grid Lines | Dark Gray |
| Worm | Green (outer), Dark Green (inner) |
| Apple | Red |
| Text | White |

## Troubleshooting

**Issue: Game won't run from Python**
- Ensure pygame is installed: `pip install pygame`
- Verify Python version: `python --version`

**Issue: Icon not showing in .exe**
- Ensure `wormy.ico` is in the same directory when building
- Rebuild using the provided command

**Issue: pygame import error**
- Install pygame-ce (community edition) if standard pygame fails:
  ```bash
  pip install pygame-ce
  ```

## Future Enhancements

Potential improvements and features:

- [ ] Difficulty levels with increasing speed
- [ ] High score tracking and persistence
- [ ] Sound effects and background music
- [ ] Different game modes (time attack, survival)
- [ ] Mobile/touchscreen support
- [ ] Multiplayer functionality
- [ ] Advanced graphics and animations

## Contributing

Feel free to fork, modify, and improve this project. Submit pull requests with enhancements or bug fixes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Author

Created as a classic game implementations using Python and Pygame.

---

**Enjoy the game and happy coding!** 🐛
