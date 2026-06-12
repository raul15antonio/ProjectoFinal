# Raul Vivaldi — Programming Paradigms Portfolio

A personal web portfolio developed for the **Introduction to Computer Science** course at the **University of Puerto Rico, Mayagüez (UPRM)**. The site contains 7 interactive programs that run directly in the browser, each demonstrating a different programming paradigm.



---

## About the Project

The goal of this project is to explore and practice programming under four different paradigms:

- **Imperative** — step-by-step instructions, mutable state, explicit loops
- **Functional** — pure functions, no side effects, function composition
- **Logic** — facts, rules, and queries using a logic engine
- **Object-Oriented** — classes, inheritance, and encapsulation

All programs run entirely in the browser — no backend, no installation required.

---

## The 7 Programs

| # | Program | Paradigm | Language / Technology |
|---|---------|----------|-----------------------|
| 1 | Bubble Sort | Imperative | JavaScript (C-style) |
| 2 | Functional Pipeline | Functional | JavaScript (pure functional) |
| 3 | Prolog Queries | Logic | Prolog via [Tau Prolog](https://tau-prolog.org/) |
| 4 | Bank Simulator | Object-Oriented | JavaScript ES6 Classes |
| 5 | Fibonacci Visualizer | Extra | JavaScript |
| 6 | Expression Calculator | Extra (URL I/O) | JavaScript |
| 7 | Curriculum Vitae | CV (any paradigm) | JavaScript + JSON + jsPDF |

### Program Details

**1. Bubble Sort (Imperative)**
Visualizes the Bubble Sort algorithm step by step. Uses mutable variables, nested loops, and explicit swaps — classic imperative style similar to C. Draws a bar chart of the sorted result and shows the number of swaps and comparisons.

**2. Functional Pipeline (Functional)**
Chains `map`, `filter`, and `reduce` into a reusable pipeline using pure functions with no mutation. Inspired by Haskell-style function composition. Choose an operation (square evens, sum odds, double if > 5) and apply it to a list of numbers.

**3. Prolog Queries (Logic)**
Runs real Prolog code in the browser using the Tau Prolog engine. Defines a family knowledge base with facts like `parent(tom, bob)` and rules like `grandparent`, `ancestor`, and `sibling`. Select a query and the engine performs logical inference to answer it.

**4. Bank Simulator (Object-Oriented)**
Demonstrates OOP with classes, inheritance, and encapsulation. `BankAccount` is the base class; `SavingsAccount` and `CheckingAccount` extend it. The balance is a private field (`#balance`). Supports create, deposit, withdraw, and status operations.

**5. Fibonacci Visualizer (Extra)**
Computes the Fibonacci sequence using both iterative and recursive approaches, plots the values on a line chart, and measures the execution time of each method for comparison.

**6. Expression Calculator (Extra)**
Evaluates math expressions typed in the input box or passed directly through the URL using the `?expr=` parameter.
```
```
Supports `sqrt()`, `abs()`, `pi`, `e`, and exponents (`^`).

**7. Curriculum Vitae (CV)**
Reads data from `cv.json` and renders a full resume on the page using the `printCVHTML()` function. Each entry has a `"show": true/false` flag to control visibility. Includes a **Download PDF** button powered by jsPDF that generates a styled PDF version of the resume.

---

## File Structure

```
portfolio/
├── index.html       # Main page — all 7 programs
└── cv.json          # CV data (name, education, skills, etc.)
```

---

## How to Run Locally

No installation needed. Just open `index.html` in any modern browser.

If you want to test the CV JSON loading correctly, serve it with a simple local server:
```bash
# Python 3
python -m http.server 8000
```
Then open `http://localhost:8000` in your browser.

---

## Technologies Used

- **HTML5 & CSS3** — structure and styling
- **JavaScript (ES6+)** — all program logic
- **[Tau Prolog](https://tau-prolog.org/)** — Prolog interpreter running in the browser
- **[jsPDF](https://github.com/parallax/jsPDF)** — PDF generation for the CV
- **[Google Fonts](https://fonts.google.com/)** — Space Grotesk & Space Mono
- **GitHub Pages** — free hosting

---

## Author

**Raul Antonio Vivaldi Santana**
Computer Science Student — UPRM, 2023–2027
📧 Raulvivaldi2005@gmail.com
🐙 [github.com/raul15antonio](https://github.com/raul15antonio)

---

## References & Credits

- Tau Prolog — Prolog interpreter for JavaScript: https://tau-prolog.org/
- jsPDF — PDF generation library: https://github.com/parallax/jsPDF
- Family tree knowledge base — classic Prolog introductory example from standard logic programming textbooks
- Bubble Sort algorithm — standard computer science algorithm (public domain)
