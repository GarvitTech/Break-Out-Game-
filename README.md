# Hand Breakout Deluxe 🎮

A modern twist on the classic Breakout game featuring **hand gesture controls** using computer vision and MediaPipe. Control the paddle with your hand movements detected through your webcam!

![Game Preview](https://img.shields.io/badge/Python-Pygame-blue) ![Computer Vision](https://img.shields.io/badge/Computer%20Vision-MediaPipe-green) ![AI Powered](https://img.shields.io/badge/AI%20Powered-Hand%20Tracking-orange)

## 🎯 Features

### Core Gameplay
- **Classic Breakout mechanics** with modern graphics
- **Hand gesture controls** - control paddle with your hand
- **Multiple levels** with increasing difficulty
- **Sound effects** for all game actions
- **Particle effects** and screen shake for immersive experience

### Power-ups
- 🔵 **Big Paddle** - Increases paddle size temporarily
- 🟡 **Slow Motion** - Reduces ball speed for easier control
- 🟣 **Multi Ball** - Creates additional balls for more action

### Technical Features
- **Real-time hand tracking** using MediaPipe
- **Smooth paddle movement** with filtering
- **Camera preview** showing detected hand landmarks
- **Responsive design** with 60 FPS gameplay
- **Cross-platform compatibility**

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- Webcam for hand tracking
- macOS/Linux/Windows

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/GarvitTech/Break-Out-Game-.git
   cd Break-Out-Game-
   ```

2. **Install dependencies**
   ```bash
   pip install pygame opencv-python mediapipe
   ```

3. **Run the game**
   ```bash
   python main.py
   ```

### Camera Permissions
On macOS, you may need to grant camera permissions:
1. Go to **System Preferences** → **Security & Privacy** → **Privacy**
2. Select **Camera** from the left sidebar
3. Check the box next to **Python** (or your terminal application)
4. Restart the game

## 🎮 How to Play

### Hand Tracking Mode (main.py)
1. **Start**: Raise your hand in front of the camera to start the game
2. **Control**: Move your hand left and right to control the paddle
3. **Goal**: Break all bricks without losing all your balls
4. **Power-ups**: Catch falling power-ups for special abilities

### Controls
- **Hand gestures**: Move your hand left/right to control paddle
- **Camera**: Your hand must be visible for the game to work
- **Restart**: Press `R` when game over
- **Quit**: Press `Q` when game over

## 🎨 Game Elements

### Visual Effects
- **Dynamic brick colors** across levels
- **Particle explosions** when bricks break
- **Screen shake** on brick hits
- **Smooth animations** for all game objects

### Sound Design
- 🔊 **Brick breaking** sound effect
- 🎾 **Paddle hit** audio feedback
- 💥 **Lose ball** notification sound
- ⚡ **Power-up collection** audio cue

## 🛠️ Technical Implementation

### Architecture
- **Object-oriented design** with clear class separation
- **Real-time hand detection** using MediaPipe
- **Smooth filtering** for natural paddle movement
- **Modular game state** management

### Key Classes
- `Paddle`: Hand-controlled paddle with smooth movement
- `Ball`: Physics-based ball movement and collision
- `Brick`: Destructible game elements
- `PowerUp`: Special ability items
- `Particle`: Visual effects system
- `Game`: Main game loop and state management

### MediaPipe Integration
- **HandLandmarker** for real-time hand detection
- **Index finger tracking** for paddle control
- **Confidence-based filtering** for reliable detection
- **Video stream processing** for smooth performance

## 📁 Project Structure

```
Break-Out-Game-/
├── main.py                    # Main game file with hand tracking
├── hand_landmarker.task       # MediaPipe hand tracking model
├── brick.wav                  # Sound effect for brick breaking
├── paddle.wav                 # Sound effect for paddle hits
├── lose.wav                   # Sound effect for losing ball
├── powerup.wav                # Sound effect for power-ups
└── README.md                  # This file
```

## 🔧 Dependencies

- **pygame**: Game engine and window management
- **opencv-python**: Camera access and image processing
- **mediapipe**: Hand tracking and computer vision
- **numpy**: Numerical computations for image processing

## 🎯 Demo Mode

If camera access is unavailable, a demo version with AI-controlled paddle is available:

```bash
python main_demo.py
```

The AI automatically controls the paddle to demonstrate all game features.

## 🏆 Game Mechanics

### Scoring System
- **10 points** per brick destroyed
- **Bonus points** for power-up collection
- **Level progression** with increasing brick count

### Lives System
- **3 lives** per game
- **Life lost** when ball falls below screen
- **Automatic respawn** with new ball

### Difficulty Progression
- **Level 1**: Standard brick layout
- **Level 2+**: Increased ball speed and brick count
- **Power-up frequency** increases with level

## 🐛 Troubleshooting

### Camera Issues
- **Camera not detected**: Check camera permissions and drivers
- **Hand not detected**: Ensure good lighting and hand visibility
- **Slow performance**: Lower camera resolution or close other applications

### Common Solutions
- **Install missing dependencies**: `pip install -r requirements.txt`
- **Camera permission denied**: Grant permissions in system settings
- **Game crashes**: Check Python version compatibility

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup
1. Fork the repository
2. Create your feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- **MediaPipe** for hand tracking technology
- **Pygame** community for the excellent game framework
- **OpenCV** for computer vision capabilities

## 🎉 Have Fun!

Enjoy playing Hand Breakout Deluxe! Experience the future of gaming where your hands become the controller. Break some bricks and have an amazing time!

---

**Made with ❤️ by GarvitTech**

