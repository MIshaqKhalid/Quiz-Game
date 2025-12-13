## Quiz-Game
# QuizMaster 🧠
QuizMaster is a robust, console-based quiz game developed in C++. It features multiple categories, varying difficulty levels, a lifeline system, and persistent high-score tracking. The project demonstrates proficiency in file handling, array manipulation, and game logic implementation.

# 🚀 Features
Multiple Categories: Choose from History, Computer Science, IQ & Logic, Science, and Sports.

Dynamic Difficulty:

Easy: 10 pts per question (-2 penalty).

Medium: 20 pts per question (-3 penalty).

Hard: 30 pts per question (-5 penalty).

Lifeline System: Four unique lifelines to help players:

[5] 50/50: Removes two incorrect options.

[6] Skip: Skips the question without penalty.

[7] Swap: Replaces the current question with a new random one.

[8] Time+10: Adds 10 seconds to the timer.

# Scoring Mechanics
Includes streak bonuses (+5 points for 3 in a row, +15 for 5 in a row) and negative marking for incorrect answers.

Persistence:

**High Scores:** Tracks the top 5 players in high_scores.txt.

**Logging:** detailed session logs are saved to quiz_logs.txt.

**Review Mode:** Players can review the questions they got wrong at the end of the quiz.

# 🛠️ Tech Stack
**Language:** C++ (Standard std namespace)

**Concepts Used:** File I/O (fstream), Parallel Arrays, Randomization (srand), Time Management (clock), Input Validation.

# 📂 File Structure
quiz.cpp: The main source code containing game logic.

high_scores.txt: Stores the top 5 high scores (Rank, Name, Date, Score, Difficulty).

quiz_logs.txt: Stores a history of every game played.

Question Banks:

history.txt

computer.txt

iq.txt

# ⚙️ How to Compile and Run
**Prerequisites**
You need a C++ compiler (like GCC/MinGW for Windows or Linux).
**
Compilation**
Open your terminal or command prompt and run:

**Bash**

g++ quiz.cpp -o QuizMaster
Running the Game
Windows:

**Bash**

QuizMaster.exe
Linux/Mac:

**Bash**

./QuizMaster
# 📝 How to Add New Questions
The game loads questions dynamically from text files. You can add your own questions by editing the category files (e.g., computer.txt).

Format for adding a question: The program reads 7 lines per question block:

Difficulty Level: (1 = Easy, 2 = Medium, 3 = Hard)

Question Text: The actual question.

Option 1

Option 2

Option 3

Option 4

**Correct Answer Index:** (1, 2, 3, or 4)

Example:

Plaintext

1
Who is the founder of Microsoft?
Steve Jobs
Bill Gates
Elon Musk
Mark Zuckerberg
2
# 🎮 Game Controls
Answering: Type 1, 2, 3, or 4 and press Enter.

Lifelines:

Type 5 for 50/50.

Type 6 to Skip.

Type 7 to Swap.

Type 8 for extra Time.

Navigation: Follow the on-screen numbered menus.

# 🐞 Known Issues / Future Improvements
Category Files: Ensure all category text files (science.txt, sports.txt) exist in the same directory as the executable, otherwise the program will display an error when selecting those categories.

Input Validation: The game handles basic integer validation, but entering characters where numbers are expected may require a restart in some edge cases.

👨‍💻 Author
