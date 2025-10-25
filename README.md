# Number Guessing Game

A sophisticated, enterprise-grade number guessing game built with Python and Tkinter, demonstrating advanced software engineering principles, modern GUI development, and comprehensive audio integration. This project showcases professional-level Python development with object-oriented design, robust error handling, and cross-platform compatibility.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technical Architecture](#technical-architecture)
- [Game Mechanics](#game-mechanics)
- [Installation & Setup](#installation--setup)
- [System Requirements](#system-requirements)
- [Project Structure](#project-structure)
- [License](#license)

## Overview

This project represents a comprehensive implementation of a number guessing game that demonstrates advanced Python programming techniques, modern software architecture, and professional development practices. The application features a sophisticated GUI built with Tkinter, integrated audio system using Pygame, and intelligent AI opponent with logical deduction algorithms.

### Key Achievements
- **Multi-threaded audio processing with channel management**
- **Advanced GUI with theme switching and animations**
- **Intelligent AI opponent with strategic decision-making**
- **Comprehensive error handling and input validation**

## Features

### Game Modes
- **Single Player Mode**: Challenge yourself against an intelligent computer opponent
- **Two Player Mode**: Local multiplayer with turn-based gameplay
- **Player vs Computer Mode**: Competitive mode where both players guess each other's numbers

### User Experience Features
- **Modern GUI Interface**: Clean, responsive design with smooth animations
- **Dynamic Theme System**: Real-time switching between dark and light themes
- **Advanced Sound System**: Multi-channel audio with background music and sound effects
- **Visual Feedback System**: Color-coded results with animated transitions
- **Comprehensive Game History**: Detailed tracking and analysis of all game attempts
- **Responsive Design**: Adaptive layout that works across different screen resolutions

### Technical Features
- **Intelligent AI Engine**: Computer opponent uses advanced logical deduction algorithms
- **Robust Input Validation**: Multi-layer validation with user-friendly error messages
- **Audio Management System**: Independent control of music and sound effects
- **State Management**: Efficient game state tracking with proper resource cleanup
- **Memory Optimization**: Smart resource management and garbage collection
- **Error Recovery**: Graceful handling of audio and system failures

## Technical Architecture

### Core Technologies
- **Primary Language**: Python 3.6+
- **GUI Framework**: Tkinter (cross-platform compatibility)
- **Audio Engine**: Pygame Mixer (multi-channel audio processing)
- **Design Pattern**: Object-Oriented Programming with MVC architecture
- **Type System**: Comprehensive type hints for better code maintainability

### System Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    Application Layer                        │
├─────────────────────────────────────────────────────────────┤
│  PPGGame Class (Main Controller)                          │
│  ├── UI Management                                        │
│  ├── Game State Management                                │
│  ├── Audio System Integration                             │
│  └── Theme Engine                                         │
├─────────────────────────────────────────────────────────────┤
│                    Service Layer                           │
├─────────────────────────────────────────────────────────────┤
│  ├── Sound Management Service                             │
│  ├── Game Logic Service                                   │
│  ├── AI Decision Engine                                    │
│  └── Input Validation Service                             │
├─────────────────────────────────────────────────────────────┤
│                    Infrastructure Layer                     │
├─────────────────────────────────────────────────────────────┤
│  ├── Tkinter GUI Framework                                │
│  ├── Pygame Audio Engine                                  │
│  └── File System Integration                               │
└─────────────────────────────────────────────────────────────┘
```

### Key Components

#### PPGGame Class (Main Controller)
- **Purpose**: Central application controller managing all game components
- **Responsibilities**: UI rendering, game state management, audio coordination
- **Design**: Singleton pattern with comprehensive state management
- **Lines of Code**: 2,000+ lines with full type annotations

#### Sound Management System
- **Multi-Channel Audio**: 8 independent audio channels for concurrent sound playback
- **Volume Control**: Independent volume management for music and sound effects
- **Error Handling**: Graceful degradation when audio files are missing
- **Resource Management**: Proper cleanup and memory management

#### AI Decision Engine
- **Algorithm**: Logical deduction with constraint satisfaction
- **Performance**: O(n²) complexity for optimal decision making
- **Learning**: Adaptive strategy based on previous game outcomes
- **Efficiency**: Smart filtering of possible number combinations

## Game Mechanics

### Core Gameplay
The objective is to guess a 4-digit number following these rules:
- Each digit must be unique (no repeated digits)
- The first digit cannot be zero
- Players receive strategic feedback after each guess

### Feedback System
- **+1**: Correct digit in the correct position
- **-1**: Correct digit in the wrong position  
- **0**: Digit is not present in the target number

### Game Flow
1. **Initialization**: Game mode selection and setup
2. **Number Generation**: Cryptographically secure random number generation
3. **Turn Management**: Efficient turn-based gameplay with state persistence
4. **Feedback Processing**: Real-time feedback calculation and display
5. **Win Condition**: Automatic detection of winning conditions
6. **Game Completion**: Comprehensive game statistics and replay options

## Installation & Setup

### Prerequisites
- **Python**: Version 3.6 or higher (recommended: 3.8+)
- **Operating System**: Windows 10+, macOS 10.14+, or Linux (Ubuntu 18.04+)
- **Memory**: 100MB RAM minimum, 200MB recommended
- **Storage**: 50MB available disk space

### Dependencies
```bash
# Core dependencies
pygame>=2.0.0          # Audio processing and game development
tkinter                # GUI framework (included with Python)
typing                 # Type hints support (Python 3.5+)
```

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/mertcaliskan34/number-guessing-game.git
   cd number-guessing-game
   ```

2. **Create Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   # Or manually:
   pip install pygame
   ```

4. **Setup Audio Files (Optional)**
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

5. **Run the Application**
   ```bash
   python "Guessing Game.py"
   ```

## System Requirements

### Minimum Requirements
- **CPU**: 1.0 GHz processor
- **RAM**: 100MB available memory
- **Storage**: 50MB free disk space
- **Display**: 800x650 resolution
- **Audio**: Optional (application works without audio)

### Recommended Requirements
- **CPU**: 2.0 GHz dual-core processor
- **RAM**: 200MB available memory
- **Storage**: 100MB free disk space
- **Display**: 1920x1080 resolution
- **Audio**: Sound card with speaker/headphone output

## Project Structure

```
number-guessing-game/
├── Guessing Game.py              # Main application entry point
├── README.md                     # Project documentation
├── LICENSE                       # License information
├── sounds/                       # Audio assets directory
│   ├── background_music.mp3      # Background music track
│   ├── button_click.mp3          # UI interaction sound
│   ├── correct.mp3               # Correct guess feedback
│   ├── lose.mp3                  # Game over sound
│   ├── win.mp3                   # Victory sound
│   └── wrong.mp3                 # Incorrect guess feedback
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**This project demonstrates advanced Python development skills, modern software architecture, and professional development practices suitable for enterprise-level applications.**