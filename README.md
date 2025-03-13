# Simon Game

A classic memory game where players must repeat a growing sequence of colors. Each round, a new step is added to the sequence, challenging the player's memory and attention. The game offers both a strict mode (restart upon error) and a relaxed mode (repeat the sequence).

---

## Features

- **Interactive Gameplay:**  
  Follow the flashing sequence of colored buttons and try to replicate it.
  
- **Audio Feedback:**  
  Each color button produces a unique sound when activated.
  
- **Strict Mode Option:**  
  Toggle strict mode to either restart the game immediately after a mistake or repeat the current sequence.
  
- **Progress Display:**  
  The central display shows the current round number, error notifications (displaying "!!"), and a win message ("WIN") when the game is completed.

---

## Project Structure

# Simon
📂 SimonGame ├── 📜 index.html # Contains HTML, CSS, and JavaScript for the game.


---

## Technologies Used

- **HTML5:**  
  Structures the content and layout of the game.

- **CSS3:**  
  Styles the game elements for an appealing user interface.

- **JavaScript (ES6):**  
  Implements game logic using modern features such as classes and async/await for handling asynchronous sequences.

- **Web Audio API:**  
  Plays sound effects for each button press.

---

## How to Play

1. **Start the Game:**  
   Click the **"Start"** button to begin a new game.

2. **Repeat the Sequence:**  
   Watch and listen as the game flashes a sequence of colors. Click the corresponding buttons in the same order.

3. **Strict Mode:**  
   Toggle **Strict Mode** using the **"Strict: OFF"** button. In strict mode, a wrong input restarts the game; otherwise, the game repeats the sequence.

4. **Win Condition:**  
   Successfully complete 20 rounds to win the game.

---

## Code Breakdown

### Initialization
- **Event Listeners:**  
  The game sets up listeners for the start button, strict mode toggle, and color buttons.

- **Audio Setup:**  
  Sound files are loaded using the `Audio` object to provide immediate audio feedback.

### Game Logic
- **Starting the Game:**  
  The `startGame` method resets game variables and generates the first random step.

- **Playing the Sequence:**  
  The `playSequence` method uses an asynchronous loop (with a helper `delay` function) to flash the sequence to the player while disabling user input.

- **Handling User Input:**  
  As the user clicks the buttons, `handleInput` checks each entry against the sequence. On error, `handleWrongInput` manages feedback and either repeats the sequence or restarts the game (based on the strict mode setting).

- **Win Scenario:**  
  After 20 correct rounds, `handleWin` displays a win message before restarting the game.

### UI Updates
- **Display:**  
  The central display updates dynamically to show the current round number, errors, or win messages.
  
- **Button Feedback:**  
  When a button is activated, it is highlighted briefly, and its corresponding sound is played.

---

## Future Enhancements

- **Responsive Design:**  
  Improve mobile responsiveness for a better experience on smaller screens.

- **Enhanced Audio Control:**  
  Add volume control and sound effect improvements.

- **Additional Game Modes:**  
  Explore new difficulty levels or multiplayer functionality.

---

## License

This project is open-source and available under the **MIT License**.
# Simon
