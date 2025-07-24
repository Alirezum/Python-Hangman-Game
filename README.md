# ASCII Hangman 🪓

A classic command‑line Hangman game implemented in Python, featuring step‑by‑step ASCII art of the gallows and man. Guess the hidden word one letter at a time before the full hangman is drawn!

## 🔎 Description

- **Language:** Python 3.x  
- **Gameplay:**  
  1. A random word is selected from a supplied word list (`wordslist.words`).  
  2. The player enters single‑letter guesses; correct letters fill in the blanks, incorrect guesses advance the ASCII hangman.  
  3. Enter `quit` at any prompt to exit early.  
- **ASCII Art:** Displays a 3‑line “hangman” figure that progressively builds with each wrong guess.

## ⚙️ Features

- Random word selection from your custom `wordslist` module  
- Dynamic ASCII‑art hangman (0–6 wrong guesses)  
- Input validation (single letters only, no repeats)  
- “Quit” option to exit at any time  
- Win/lose detection with end‑game summary  

## 🚀 Getting Started

### Prerequisites

- Python 3.6 or higher

### Installation & Setup

1. **Clone the repo**  
```bash
   git clone https://github.com/your-username/ascii-hangman.git
   cd ascii-hangman
```

2. **Prepare your word list**
    
    - Edit `wordslist.py` so that it defines a `words` list, e.g.:
        
        ```python
        words = ["python", "hangman", "challenge", "developer"]
        ```
        

### Running the Game

```bash
python hangman.py
```

- At each prompt, type a single letter and press Enter.
    
- Type `quit` to exit the game at any time.
    

## 🗂️ Project Structure

```
ascii-hangman/
├── hangman.py        # Main game script
├── wordslist.py      # Defines `words` list for random selection
└── README.md         # Project overview & instructions
```

## 🎓 How It Works

1. **`display_man(wrong_guess)`** draws the current ASCII stage.
    
2. **`display_hint(hint)`** shows guessed letters and underscores.
    
3. Input is checked for validity, duplicates, and membership in the answer.
    
4. Game ends when the word is fully revealed (win) or max wrong guesses reached (lose).
    

## 🛡️ License

This project is released under the MIT License. See LICENSE for details.

