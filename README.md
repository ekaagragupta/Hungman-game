
# 🎮 Hangman Game in C

A simple, interactive console-based Hangman game written in C. This program randomly selects a secret word along with a hint and allows the user to guess it letter by letter. If too many incorrect guesses are made, the player loses and the full hangman figure is drawn.

---

## 🧠 Game Concept

The classic game of **Hangman** challenges a player to guess a hidden word by suggesting letters. For each incorrect guess, a part of the hangman is drawn. The player wins by guessing the word before the figure is completed.

---

## 🛠️ Features

* 🎯 Random word and hint generation.
* ✏️ Letter-by-letter guessing.
* ❌ Tracks incorrect guesses and shows a growing hangman figure.
* ✅ Displays correctly guessed letters in position.
* 🧠 Includes hints for each word.
* 🔠 Validates repeated and invalid inputs.
* 🚫 Max 6 incorrect tries before losing.

---

## 📷 Gameplay Example

```plaintext
Welcome to Hangman!
Hint: A popular Italian dish

Word: _ _ _ _ _
  _______
 |/      |
 |        
 |        
 |        
 |
_|___

Enter a letter: p
Nice! 'p' is in the word.

Word: p _ _ _ _
...
🎉 You got it! The word was "pizza".
```

---

## 📂 File Structure

```
📁 hangman
├── hangman.c       # Main C source file
├── README.md       # Project documentation
```

---

## 🚀 Getting Started

### 🔧 Requirements

* A C compiler (GCC or Clang)
* A terminal or command prompt

### ⚙️ Compile the Program

```bash
gcc -std=c99 -o hangman hangman.c
```

### ▶️ Run the Game

```bash
./hangman
```

---

## ✏️ How It Works

1. A random word and its hint are chosen from a predefined list.
2. The user is shown a series of underscores representing unguessed letters.
3. The user enters one letter at a time:

   * If correct: the letter is revealed in the word.
   * If incorrect: a part of the hangman is drawn.
4. The game ends when:

   * The word is fully guessed (Victory 🎉)
   * The user makes 6 wrong guesses (Game Over ☠️)

---

## 🧩 Word List Customization

You can add more words and hints to the array in `wordList[]`:

```c
struct WordWithHint wordList[] = {
    { "geeksforgeeks", "Computer coding" },
    { "elephant", "A large mammal with a trunk" },
    { "pizza", "A popular Italian dish" },
    { "beach", "Sandy shore by the sea" },
    { "matrix", "Sci-fi movie and math concept" },
    { "python", "Popular programming language" },
    // Add more here...
};
```

---

## 🛡️ Input Safety

* Only alphabetic characters are accepted.
* Repeated guesses are detected.
* Invalid inputs are ignored with a message.

---

## 🤖 Author

Made by **Ekaagra gupta**
Language: C
Last updated: 2025

