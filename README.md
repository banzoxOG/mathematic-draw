# ∑ Mathematic Draw

A browser-based math visualizer that lets you **plot functions** with an on-screen keyboard and **extract math from images** using AI.

🔗 **Live site:** [banzoxog.github.io/mathematic-draw](https://banzoxog.github.io/mathematic-draw)

---

## Features

### 📈 Plot functions
- Type any math expression using `x` as the variable
- On-screen keyboard — no need to remember syntax
- Plot multiple curves at once, each in a different color
- Zoom in/out and set custom x-axis range
- Live graph renders instantly on a full-screen canvas

### 🖼 Image → Math
- Upload any image containing math (handwritten or printed)
- AI reads the image and extracts all equations, formulas, and functions
- Detected plottable functions can be sent directly to the graph with one click

---

## How to use

### Plotting a function
1. Open the **Plot** tab
2. Use the on-screen keyboard to build an expression (e.g. `sin(x)`, `x^2 - 4`)
3. Press **Plot** — the curve appears on the graph
4. Add more curves or remove them with the × button
5. Use **+** / **−** to zoom, or set the x range manually

### Analyzing an image
1. Open the **Image → Math** tab
2. Drop or upload a photo of any equation or graph
3. Press **Analyze image**
4. Read the extracted math in the result box
5. If a plottable function is found, press **↗ Plot detected expression** to graph it

---

## Supported functions

| Category | Examples |
|---|---|
| Arithmetic | `+`, `-`, `*`, `/`, `^` |
| Trigonometry | `sin(x)`, `cos(x)`, `tan(x)`, `asin(x)`, `atan(x)`, `cot(x)` |
| Powers & logs | `x^2`, `sqrt(x)`, `cbrt(x)`, `exp(x)`, `log(x)`, `log2(x)`, `ln(x)` |
| Other | `abs(x)`, `floor(x)`, `ceil(x)`, `round(x)`, `sign(x)`, `mod(x, n)` |
| Constants | `pi`, `e` |

**Example expressions:**
```
sin(x)
x^2 - 4
exp(-x^2)
1/x
tan(x)
sin(x) * cos(x)
x^3 - 3*x
sqrt(abs(x))
floor(x)
```

---

## Tech stack

- **Vanilla HTML/CSS/JS** — no frameworks, single file
- **[math.js](https://mathjs.org/)** — expression parsing and evaluation
- **Canvas API** — graph rendering
- **Anthropic Claude API** — AI-powered image analysis (`claude-sonnet-4`)

---

## Project structure

```
mathematic-draw/
└── index.html     # entire app — layout, keyboard, canvas, AI call
```

---

## Local development

No build step needed. Just clone and open:

```bash
git clone https://github.com/banzoxog/mathematic-draw
cd mathematic-draw
# open index.html in your browser
```

Or use a local server:

```bash
npx serve .
```

---

## Deployment

Hosted on **GitHub Pages** directly from the `main` branch.

Any push to `main` automatically updates the live site at  
[banzoxog.github.io/mathematic-draw](https://banzoxog.github.io/mathematic-draw)

---

## License

MIT — free to use and modify.
