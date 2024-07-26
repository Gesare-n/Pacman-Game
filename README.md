# Pacman Game

## Overview
This is a classic Pacman game implementation using HTML5 Canvas and JavaScript. The game features the iconic Pacman character navigating through a maze, eating dots, and avoiding ghosts. The project also includes the ability to render and move ghosts with simple AI behavior.

## Features
- **Pacman Character**: Move Pacman in four directions (Up, Down, Left, Right) and eat dots.
- **Ghosts**: Implemented with basic AI to move randomly or chase Pacman.
- **Collision Detection**: Handles collisions between Pacman, ghosts, and walls.
- **Score System**: Keeps track of the score as Pacman eats dots.

## How to Play
1. **Open the Game**: Open the `index.html` file in your web browser. This will load the game onto the canvas.
2. **Controls**: Use the arrow keys on your keyboard to move Pacman in the desired direction:
   - Arrow Up: Move Pacman up.
   - Arrow Down: Move Pacman down.
   - Arrow Left: Move Pacman left.
   - Arrow Right: Move Pacman right.
3. **Objective**: Eat all the dots on the screen to win. Avoid colliding with ghosts, which will cause the game to end.

## Red Circles Explanation
The red circles that appear around the view of the game are used for debugging purposes. They represent the range within which the ghosts are able to detect and chase Pacman. If you see these circles, it means the game is currently showing the detection range of the ghosts. To remove these circles in the final game version, you would need to modify the `draw()` method in the `ghost.js` file by removing or commenting out the following lines:

```javascript
canvasContext.beginPath();
canvasContext.strokeStyle = "red";
canvasContext.arc(
    this.x + oneBlockSize / 2,
    this.y + oneBlockSize / 2,
    this.range * oneBlockSize,
    0,
    2 * Math.PI
);
canvasContext.stroke();
## Files
- **`index.html`**: Main HTML file to render the game.
- **`pacman.js`**: JavaScript file defining the Pacman character and its behavior.
- **`ghost.js`**: JavaScript file defining the Ghost characters and their AI behavior.
- **`game.js`**: JavaScript file managing game updates and rendering.
- **`animations.gif`**: Image file used for Pacman’s animations.
- **`ghost.png`**: Image file used for the ghosts.

## Installation
1. **Clone the Repository**

    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2. **Open the Project**

   Open the `index.html` file in your web browser. You can use any modern web browser (Chrome, Firefox, Edge) to play the game.

## Project Structure
- **`index.html`**: Sets up the canvas and includes the necessary scripts.
- **`pacman.js`**: Handles Pacman’s movement, collision detection, and animations.
- **`ghost.js`**: Manages ghost behaviors, including random movement and collision detection.
- **`game.js`**: Coordinates the game loop, updates game state, and renders objects on the canvas.
- **`animations.gif`**: Provides animation frames for Pacman.
- **`ghost.png`**: Provides sprite frames for ghosts.

## Development
- **Code Editor**: Use any text editor or IDE of your choice (e.g., Visual Studio Code, Sublime Text).
- **Version Control**: The project uses Git for version control. Make sure to commit your changes and push to the repository regularly.

## Contributing
Feel free to contribute to the project by submitting issues or pull requests. Please follow the guidelines and code of conduct when contributing.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements
- The Pacman game concept and design.
- The HTML5 Canvas API for rendering graphics.
- The JavaScript language for game logic and interaction.
