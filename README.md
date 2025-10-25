# Number Guessing Game

A number guessing game built with Python and Tkinter, featuring multiple game modes, sound effects, and a clean GUI with theme switching. This project demonstrates Python GUI development, audio integration with Pygame, and basic game logic implementation.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Game Mechanics](#game-mechanics)
- [Installation & Setup](#installation--setup)
- [System Requirements](#system-requirements)
- [Project Structure](#project-structure)
- [License](#license)

## Overview

This is a number guessing game where players try to guess a 4-digit number with unique digits. The game includes multiple modes (single player, two player, and vs computer), sound effects, and a responsive GUI with dark/light theme support.

### Key Features
- **Multiple game modes**: Single player, two player, and vs computer
- **Sound effects**: Background music and game sound effects
- **Theme switching**: Dark and light mode support
- **Clean GUI**: User-friendly interface built with Tkinter
- **Input validation**: Proper error handling and user feedback

## Features

### Game Modes
- **Single Player**: Play against the computer
- **Two Player**: Local multiplayer with turn-based gameplay
- **Player vs Computer**: Both players guess each other's numbers

### User Experience
- **GUI Interface**: Clean, responsive design with animations
- **Theme System**: Switch between dark and light themes
- **Sound System**: Background music and sound effects
- **Visual Feedback**: Color-coded results and feedback
- **Game History**: Track of all attempts and results

### Technical Features
- **AI Opponent**: Computer uses logical deduction
- **Input Validation**: Error checking with user-friendly messages
- **Audio Management**: Independent control of music and sound effects
- **State Management**: Game state tracking and cleanup

## Game Mechanics

### How to Play
The objective is to guess a 4-digit number following these rules:
- Each digit must be unique (no repeated digits)
- The first digit cannot be zero
- You receive feedback after each guess

### Feedback System
- **+1**: Correct digit in the correct position
- **-1**: Correct digit in the wrong position  
- **0**: Digit is not present in the target number

### Game Flow
1. Select game mode
2. Enter your guess (4-digit number)
3. Receive feedback
4. Continue until you guess correctly or run out of attempts

## Installation & Setup

### Prerequisites
- **Python**: Version 3.6 or higher
- **Operating System**: Windows, macOS, or Linux
- **Memory**: 50MB RAM minimum
- **Storage**: 10MB available disk space

### Dependencies
```bash
# Core dependencies
pygame>=2.0.0          # Audio processing
tkinter                # GUI framework (included with Python)
```

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/mertcaliskan34/number-guessing-game.git
   cd number-guessing-game
   ```

2. **Install Dependencies**
   ```bash
   pip install pygame
   ```

3. **Setup Audio Files (Optional)**
   ```bash
   # Create sounds directory
   mkdir sounds
   
   # Add audio files to sounds/ directory:
   # - background_music.mp3
   # - button_click.mp3
   # - correct.mp3
   # - lose.mp3
   # - win.mp3
   # - wrong.mp3
   ```

4. **Run the Application**
   ```bash
   python "Guessing Game.py"
   ```

## System Requirements

### Minimum Requirements
- **CPU**: Any modern processor
- **RAM**: 50MB available memory
- **Storage**: 10MB free disk space
- **Display**: 800x650 resolution
- **Audio**: Optional (game works without audio files)

### Recommended Requirements
- **CPU**: 1.0 GHz processor
- **RAM**: 100MB available memory
- **Storage**: 20MB free disk space
- **Display**: 1024x768 resolution
- **Audio**: Sound card with speaker/headphone output

## Project Structure

```
number-guessing-game/
├── Guessing Game.py              # Main application
├── README.md                     # Project documentation
├── LICENSE                       # License information
├── sounds/                       # Audio files directory
│   ├── background_music.mp3      # Background music
│   ├── button_click.mp3          # Button click sound
│   ├── correct.mp3               # Correct guess sound
│   ├── lose.mp3                  # Game over sound
│   ├── win.mp3                   # Victory sound
│   └── wrong.mp3                 # Wrong guess sound
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**This project demonstrates Python GUI development, audio integration, and basic game programming concepts.**