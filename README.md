# pipeline

> The Astor Design System. One colour. Maximum whitespace. Sub-5KB philosophy.

---

## What is this

pipeline is the shared visual language for everything built under the Astor umbrella.

One accent colour (`#0EFFAF`). Near-black backgrounds. Whitespace that costs something. Type that carries the load.

Used across: VexID, VexConnect, neuais, ContinuuAI, The Zookeeper.

---

## Design principles

```
1. One colour owns you — #0EFFAF
2. White space is the expensive part
3. The accent does one job: pull the eye
4. Type does the heavy lifting
5. Asymmetry with intention
6. Two fonts maximum
7. Every page sub-5KB renderable
```

---

## What's in here

| File | Description |
|------|-------------|
| `design-system.css` | The full CSS system — tokens, reset, type scale, components |
| `demo-diagrams.html` | Architecture diagram demos |
| `demo-zookeeper-ch1.html` | Book rendering demo (Tufte style) |
| `excel.html` | Data table demo |
| `*.png` | Brand assets for all Astor projects |
| `A_Tufte_Style_Book_*/` | Tufte-style book layout experiments |

---

## CSS tokens

```css
:root {
  --accent:     #0EFFAF;   /* the only colour that matters */
  --bg-dark:    #0A0A0A;   /* near-black */
  --fg-dark:    #E8E4DE;   /* warm white */

  /* Type scale — minor third (1.2x) */
  --step-0: clamp(1rem, 0.93rem + 0.33vw, 1.15rem);
  /* ...steps -2 through +6 */
}
```

---

## Usage

Drop `design-system.css` in your project. Use the CSS custom properties. Don't add a second accent colour.

```html
<link rel="stylesheet" href="design-system.css">
<body class="dark">
  <span style="color: var(--accent)">this pulls the eye</span>
</body>
```

---

## Philosophy

Every page in the Astor ecosystem should be readable on a 2G connection in a browser from 2015. Anything heavier than 5KB of CSS is a choice that needs justification.

This system has none of that weight.
