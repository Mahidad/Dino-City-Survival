# 🦖 Dino-City-Survival
3D game implemented by OpenGL

A thrilling 3D survival game where you control a dinosaur navigating through a procedurally generated city, collecting eggs, avoiding enemies, and surviving catastrophic meteor showers!

🌟 Features
🎯 Core Gameplay (16 Features)

1. 🦕 Dinosaur Movement & Control - Smooth WASD movement with jumping mechanics
2. 🥚 Egg Collection System - Collect randomly spawning eggs throughout the city
3. 💪 Stamina Management - Monitor and manage your dino's energy levels
4. ❤️ Enhanced Health System - 3 lives with two distinct death animations (normal & meteor death with fire effects)
5. 👾 Enemy Dinosaur AI - Intelligent enemies that chase and grow stronger over time
6. ⚔️ Combat System - Throw collected eggs to defeat enemies
7. 🌈 Egg Types & Power-ups - Four egg types with different effects (normal, golden, stamina, power)
8. 🔄 Enemy Spawn System - Dynamic enemy respawning maintaining constant challenge
9. 🏙️ City Building System - Procedurally generated 3D city environment
10. ☄️ Meteor Shower Events - Periodic catastrophic events with safe zones
11. 🎁 Bonus Round System - Special rounds triggered by golden eggs
12. 🌓 Day-Night Cycle - Dynamic lighting that changes over time
13. ⚡ Egg Conversion System - Convert eggs to stamina for survival
14. 🎯 Throw Mechanics & Physics - Realistic projectile physics for egg throwing
15. 🎥 Camera System - Multiple camera modes (first-person and third-person)
16. 🔓 Cheat Mode System - Various cheat options for testing and fun

🎮 Controls

Key Action Description
WASD Movement Move dinosaur forward, backward, strafe
Mouse Look Around Control view direction (first-person mode)
Left Click Throw Egg Throw collected eggs (when aiming)
Right Click Aim Mode Enter/exit aiming mode
Space Jump Jump over obstacles
C Convert Eggs Convert eggs to stamina
F Camera Toggle Switch between first/third person views
Tab Cheat Mode Toggle cheat mode on/off
R Restart Game Restart after game over
P Pause Game Pause/resume gameplay
+/- Zoom Zoom camera in/out

📖 Game Rules

Objective

Survive as long as possible by collecting eggs, avoiding enemies, and surviving meteor showers. Your score increases with each collected egg and defeated enemy.

Game Mechanics

· Egg Collection: Collect eggs to increase score and gain special abilities
· Stamina System: All actions consume stamina; convert eggs to replenish it
· Combat: Throw eggs at enemies (5 hits to defeat)
· Meteor Showers: Every 60 seconds, seek the green safe zone within 15 seconds
· Bonus Rounds: Collect 3 golden eggs to trigger 30-second bonus rounds
· Enemy Growth: Enemies grow larger and faster over time

Death Conditions

· Enemy Attack: Lose 1 life when caught by enemy dinosaur
· Meteor Impact: Lose 1 life when hit by meteor outside safe zone
· Game Over: When all 3 lives are lost

🛠️ Installation & Setup

Prerequisites

· Python 3.7 or higher
· PyOpenGL library
· GLUT libraries

Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/dino-city-survival-3d.git
   cd dino-city-survival-3d
   ```
2. Install required packages:
   ```bash
   pip install PyOpenGL PyOpenGL_accelerate
   ```
3. Install GLUT (depending on your OS):
   Windows:
   · Download freeglut from: http://freeglut.sourceforge.net/
   · Place freeglut.dll in your System32 folder or project directory
   macOS:
   ```bash
   brew install freeglut
   ```
   Linux (Ubuntu/Debian):
   ```bash
   sudo apt-get install freeglut3 freeglut3-dev
   ```
4. Run the game:
   ```bash
   python main.py
   ```

🎯 How to Play

Getting Started

1. Press SPACE at the start screen to begin
2. Use WASD to move your dinosaur around the city
3. Collect eggs (🥚) to increase your score and inventory

Survival Tips

· Always monitor your stamina - running out leaves you vulnerable
· Convert eggs to stamina when running low (press C)
· During meteor showers, immediately head for the green glowing safe zone
· Golden eggs are valuable - collect 3 to trigger bonus rounds
· Aim carefully when throwing eggs at enemies
· Use buildings as cover from enemies

Cheat Mode

Press Tab to enable cheat mode with:

· Eggs automatically move toward you
· One-hit kill enemies
· Infinite stamina
· Skip meteor showers

🏗️ Project Structure

```
dino-city-survival-3d/
├── main.py                 # Main game file
├── README.md               # This file
├── requirements.txt        # Python dependencies
├── assets/                 # Game assets (if any)
│   └── (textures, sounds)
├── modules/                # Optional modular structure
│   ├── game_objects.py    # Dinosaur, eggs, enemies classes
│   ├── city_generator.py  # Procedural city generation
│   ├── physics_engine.py  # Collision and movement physics
│   └── ui_renderer.py     # UI and HUD rendering
└── screenshots/           # Game screenshots
```

🧠 Technical Details

Built With

· Python 3.x - Core programming language
· PyOpenGL - 3D graphics rendering
· OpenGL Utility Toolkit (GLUT) - Window management and input handling
· Standard Python Libraries - math, random, time

Graphics Pipeline

· Uses immediate mode OpenGL rendering
· Vertex-based primitive drawing (GL_QUADS, GL_TRIANGLES)
· Transformation matrices for 3D positioning
· Depth buffering for proper 3D rendering
· Texture-less shading with colored primitives

Performance Features

· Efficient collision detection using spatial partitioning
· Object pooling for frequent creations (eggs, particles)
· Frame-rate independent movement calculations
· Optimized rendering with display lists


Survive, Collect, Thrive - Be the Last Dino Standing!

Last Updated: [Date]
