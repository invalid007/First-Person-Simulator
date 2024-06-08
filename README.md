# First Person Simulator

This is a simple First-Person Shooter (FPS) simulator implemented in C++ using console graphics. It uses Wolfenstein's ray casting algorithm to render a 3D-like environment in the console window.

https://github.com/invalid007/First-Person-Simulator/assets/126184615/efa52b0d-e25e-4294-9c43-00d610ffccc1

## Features

- Basic 3D rendering using ray casting
- Simple movement controls (W, A, S, D)
- Basic collision detection with walls

![Simple_raycasting_with_fisheye_correction](https://github.com/invalid007/First-Person-Simulator/assets/126184615/e0f24cf1-d281-4b98-9717-7e63d9875a18)

-*A simple ray casting rendering similar to the Wolfenstein 3D engine. The red dot is the player's location. The orange area represents the player's field of view.*


![Screenshot 2024-06-08 172327](https://github.com/invalid007/First-Person-Simulator/assets/126184615/6e2c9b7a-2c49-40fd-9fce-dcc248ae6a5f)

## Requirements

- Windows OS
- Visual Studio (or any other C++ compiler supporting Windows API)
- Unicode support in the console

## Getting Started

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/fps-simulator.git
   cd fps-simulator
2. **Open the project in your C++ development environment (e.g., Visual Studio).**

3. **Build the project.**

### Running the Simulator

After building the project, you can run the executable. The simulator will open in a console window.

### Controls

- `W`: Move forward
- `S`: Move backward
- `A`: Rotate left
- `D`: Rotate right

## Code Overview

### Main Components

- **Screen Buffer**: A character array (`wchar_t* screen`) used to render the display.
- **Map**: A simple string representation of the game world, where `#` represents walls and `.` represents open space.
- **Player**: The player has a position (`fPlayerX`, `fPlayerY`) and an angle (`fPlayerA`).

### Game Loop

1. **Input Handling**: Reads the input from the user to move and rotate the player.
2. **Ray Casting**: Utilizes Wolfenstein's ray casting algorithm to determine the distance to the nearest wall for each column of the screen.
3. **Rendering**: Fills the screen buffer with the appropriate characters to represent walls, floors, and the player.

### Key Functions

- **Ray Casting**: Determines the distance from the player to the nearest wall for each column of the screen using Wolfenstein's ray casting technique.
- **Collision Detection**: Prevents the player from moving through walls.
- **Rendering**: Updates the screen buffer with the current game state and displays it.





