# rubiks-cube-solver
JavaScript Rubik's Cube Solver with OOP implementation

# Rubik's Cube Solver

![Rubik's Cube Solver Screenshot](screenshot.png) *(add a screenshot later)*

An interactive 3D Rubik's Cube simulator with solving algorithm implementation in JavaScript.

## Features

- **3D Cube Visualization**: View the cube state from all angles
- **Manual Control**: Rotate any face with simple controls
- **Scramble Function**: Randomly scramble the cube with one click
- **Solver Algorithm**: Automatically solve the cube (basic implementation)
- **Step-by-Step Solution**: View each move in the solving process
- **Responsive Design**: Works on desktop and mobile devices

## Technologies Used

- HTML5, CSS3, JavaScript (ES6+)
- Object-Oriented Programming approach
- Custom-built cube rotation algorithms
- Glassmorphism UI design

## How to Use

1. **Manual Rotation**:
   - Click any face rotation button (F, B, U, D, L, R) to rotate that face
   - Add ' to rotate counter-clockwise (e.g., F')

2. **Scramble the Cube**:
   - Click the "Scramble Cube" button to randomize the cube

3. **Solve the Cube**:
   - Click "Solve Cube" to see the step-by-step solution
   - Each step shows the move and resulting cube state

4. **Reset**:
   - Click "Reset Cube" to return to a solved state

## Implementation Details

### Cube Representation
- The cube is represented as an object with 6 faces (U, D, F, B, L, R)
- Each face is a 3x3 array of color codes ('w', 'y', 'r', 'o', 'g', 'b')

### Rotation Logic
- Face rotations handle both clockwise and counter-clockwise turns
- Edge rotations update adjacent faces automatically
- Move history is tracked for solving/replay

### Solving Algorithm
- Basic layer-by-layer approach:
  1. Solve white cross (first layer edges)
  2. Solve white corners
  3. Solve middle layer edges
  4. Solve yellow cross
  5. Position last layer edges
  6. Position last layer corners
  7. Orient last layer corners

*(Note: The current solver is a simplified implementation - a complete solver would require more advanced algorithms)*

## Installation

No installation required! Simply open `index.html` in any modern web browser.

Alternatively, you can:
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/rubiks-cube-solver.git

