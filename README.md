# Friends Quiz ☕

A Y2K-style trivia game for fans of *Friends*. Pick one of the six friends (Rachel, Ross, Phoebe, Monica, Chandler or Joey) and answer 10 multiple-choice questions about them.

## Features
- Friends-themed, Y2K-inspired homepage in the show's color palette
- One 10-question quiz per character, with instant right/wrong feedback, a progress bar and a live score
- Results screen with a score-based message, plus "Play again" and "Pick a friend"
- Answer order is shuffled every time (True/False and Yes/No questions keep their order)
- Fits the screen without scrolling, on desktop, tablet and phone

## Run it
No build step or dependencies. Open `index.html` in a browser. The Google Fonts (Bagel Fat One, Nunito, VT323) need an internet connection.

## Project structure
```
index.html   the whole app: HTML, CSS and JavaScript
images/      character photos and the FRIENDS logo
```

## Editing the quizzes
Quiz data lives in the `QUIZZES` object in `index.html`. Each question looks like this:

```js
{ q: "What is Rachel's last name?", a: ["Green", "Buffay", "Geller", "Bing"] }
```

The first option in `a` is the correct answer; the options are shuffled when shown. For two-option questions, list the options in the order you want and add `ans`:

```js
{ q: "Did Mike try to propose to Phoebe?", a: ["Yes", "No"], ans: "Yes" }
```

## Credits
Questions and answers are adapted from [FunTrivia](https://www.funtrivia.com). This is an unofficial fan project. *Friends*, its characters, images and logo belong to Warner Bros. and their respective owners.
