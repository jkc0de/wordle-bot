# Wordle-bot

Wordle-bot is a Python + Selenium bot for solving wordle puzzles for https://www.nytimes.com/games/wordle/index.html


https://user-images.githubusercontent.com/88771772/209678765-ba59c312-8f11-481a-b3cd-98930a5ea4e9.mov


## Description
1. Bot chooses from 2409 possible answers, Wordle uses CSW19 5-letter words as wordlist.
2. Bot opens official Wordle website and enters 5-letter guess.
3. Bot analyzes and gets result from first guess which returns 3 lists, absent(grey), present(yellow) and correct(green).
4. Bot algorithm will use the results gathered to calculate the next possible list of answers.
5. Bot continues step (2-4) until Wordle puzzle is completed successfully.

## Getting Started

Use the package manager + virtual environment [pipenv] to install required packages.
<br>
Download ChromeDriver from https://chromedriver.chromium.org/downloads based on system's Google Chrome version

For macOS

Extract ChromeDriver and transfer into /usr/local/bin folder

Allow ChromeDriver in terminal 

```bash
xattr

https://user-images.githubusercontent.com/88771772/209678165-69d4c179-de49-43f2-97b8-309b153e7f91.mov

 -d com.apple.quarantine /usr/local/bin/chromedriver
```

## Usage

Call executeBot() function to start bot, hard-coded first 5-letter guess will be "React"

```python
python3 app.py
```

