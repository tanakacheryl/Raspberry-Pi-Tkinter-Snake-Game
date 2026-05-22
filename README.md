<h1>Raspberry Pi Tkinter Snake Game</h1>

<h2>Description</h2>
This project is a Python-based embedded gaming system that combines a graphical Snake game with physical GPIO button controls on a Raspberry Pi. The game uses the Tkinter library to create a real-time game window where the player controls the snake using external push buttons connected to the Raspberry Pi GPIO pins. Each button press changes the snake’s movement direction, while a dedicated start button can instantly restart the game.

The system continuously updates the snake’s position, generates random apples on the game grid, and detects collisions with the snake’s own body. As the snake eats apples, its tail grows longer, increasing the game difficulty over time. The game also includes screen-wrap movement, allowing the snake to reappear on the opposite side when reaching the edge of the display.

The project uses Python together with the GPIO Zero library for hardware button input handling and Tkinter for graphical rendering and event management. Real-time gameplay is achieved using timed game loops and event-driven programming techniques. Overall, the project combines embedded hardware interaction, GUI programming, and game logic to create an interactive Raspberry Pi gaming system.
<br />


<h2>Technologies Used</h2>

- Python
- Tkinter GUI
- GPIO Zero
- Raspberry Pi GPIO
- Event-Driven Programming
- Real-Time Game Loop Logic
- Embedded Systems Programming

<h2>Hardware Used</h2>

- Raspberry Pi
- Push buttons
- Breadboard
- Jumper wires
- Display monitor
- USB keyboard (optional for keyboard controls)
- 
<br/>

<h2>🔌 Wiring Connections (GPIO Pins)</h2>

<table>
  <tr>
    <th>Control Button</th>
    <th>GPIO Pin</th>
  </tr>
  <tr>
    <td>Up</td>
    <td>GPIO 26</td>
  </tr>
  <tr>
    <td>Down</td>
    <td>GPIO 12</td>
  </tr>
  <tr>
    <td>Left</td>
    <td>GPIO 25</td>
  </tr>
  <tr>
    <td>Right</td>
    <td>GPIO 18</td>
  </tr>
  <tr>
    <td>Start / Restart</td>
    <td>GPIO 24</td>
  </tr>
</table>  

<br/>

<h2>How It Works</h2>

The game creates a graphical Snake interface using Python and the Tkinter library. A continuous game loop updates the snake’s movement, redraws the game screen, and checks for collisions in real time.

Physical push buttons connected to the Raspberry Pi GPIO pins are used to control the snake’s direction:
- Up
- Down
- Left
- Right

When a button is pressed, the GPIO Zero library detects the input and changes the snake’s movement direction instantly. The game also supports keyboard arrow-key controls through Tkinter event handling.

Random apples are generated on the game grid, and each time the snake eats one, its tail increases in length. If the snake collides with its own body, the game automatically resets to its starting position.

A dedicated start button connected to the Raspberry Pi can also restart the game at any time.

<br/>

---

<!--
```diff
- red text (errors)
+ green text (adds)
! orange text (warnings)
# gray text (notes)
@@ purple bold text (important)@@
