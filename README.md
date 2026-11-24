# Math Quiz — Scoring and Turns

A later two-player multiplication quiz with intended answer checking and turn switching.

**Repository created:** 2021-09-19  
**Project status:** Learning project / historical snapshot  
**Earliest recorded commit (author date):** 2021-09-19

## Features and implementation

- Calculate the product.
- Generate prompts.
- Implement score-update branches and alternate question/answer turns.

## Technologies

HTML, CSS, JavaScript, Bootstrap, jQuery.

## How the code works

`addUser()` stores both player names; `send()` generates a multiplication question; `check()` contains the intended answer-validation and turn-switching logic.

## Project structure

| File | Purpose |
| --- | --- |
| [`gamepage.html`](gamepage.html) | Quiz game interface |
| [`gme.js`](gme.js) | Question and game logic |
| [`index.html`](index.html) | Main page and user interface |
| [`main.js`](main.js) | Project-specific JavaScript |
| [`style.css`](style.css) | Page styling |

Key functions in the source:
- `gme.js`: `send()`, `check()`.
- `main.js`: `addUser()`.

## Run or explore locally

```bash
git clone https://github.com/Avenger-Sonic123/Math_Quiz_Completed.git
cd Math_Quiz_Completed
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in your browser. The local server requires Python 3; browser-based dependencies may also require internet access.

Enter two names and generate a question; answer checking requires the fix noted above.

## Current status and limitations

The Check function compares undefined variables (`answer` and `word`) rather than the computed answer, so scoring and turn changes need debugging.

## Related project snapshots

Other repositories in this project family:
- [Math_Quiz_1.0](https://github.com/Avenger-Sonic123/Math_Quiz_1.0) — repository created 2021-08-23
- [Math_Quiz-2.0](https://github.com/Avenger-Sonic123/Math_Quiz-2.0) — repository created 2021-09-05
- [Math_Quiz-3.0](https://github.com/Avenger-Sonic123/Math_Quiz-3.0) — repository created 2021-09-05

---

Source reference: [`67b5113b`](https://github.com/Avenger-Sonic123/Math_Quiz_Completed/tree/67b5113b441f77da445561db5d4d526dd9330a0d) on `main`, verified against GitHub on 2026-11-24. Documentation is based on static source review; runtime behavior has not been tested.
