# Wordle Clone by Aadhya Anand

A Python-based Wordle clone that challenges players to guess a 5-letter word in 6 attempts. Features colored feedback, replayability, and game statistics. Built for Google Colab/Jupyter notebooks.

---

## Features
- 🟩 **Colored Feedback**:  
  - **Green**: Correct letter & position.  
  - **🟨 Yellow**: Correct letter, wrong position.  
  - **⬛ Gray**: Letter not in the word.  
- 🔄 **Replayability**: Play multiple games with tracked statistics.  
- 📊 **Statistics**: Win distribution and game history.  
- ❓ **Help Menu**: Instructions with examples (`h` to view).  
- 📖 **Dynamic Alphabet Display**: Tracks remaining letters with color-coded hints.  
- ✅ **Input Validation**: Ensures guesses are valid 5-letter words.  

---

## Installation & Setup
1. **Google Colab**:  
   - Open the provided `.ipynb` file in [Google Colab](https://colab.research.google.com/).  
   - Run all cells to start the game.  

2. **Local Jupyter Notebook**:  
   - Ensure `google-colab` is installed for screen-clearing functionality:  
     ```bash
     pip install google-colab
     ```  
   - Clone the repository and run the notebook.  

---

## How to Play
1. Start the game by running the `wordle()` function.  
2. **Guess a 5-letter word** (e.g., `CRANE`).  
3. Use commands:  
   - `h`: View instructions during gameplay.  
   - `q`: Quit the game.  
4. Receive color feedback after each guess:  
   - 🟩 `W E A R Y` → `W` is correct.  
   - 🟨 `P I L L S` → `I` is in the wrong spot.  
   - ⬛ `V A G U E` → `U` is incorrect.  
5. Win by guessing the word in 6 tries or fewer.  

---

## Code Structure
### Key Functions
- `game_instructions()`: Prints rules and examples.  
- `user_input()`: Validates guesses and handles commands.  
- `progress()`: Updates the game interface (remaining attempts, guessed words, alphabet).  
- `wordle()`: Main game loop with win/loss logic and statistics.  

### Dependencies
- `random`: Random word selection from the `WORDS` list.  
- ANSI escape codes for terminal coloring.  
