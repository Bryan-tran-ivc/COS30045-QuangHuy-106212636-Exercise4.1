# Exercise 4.1 — notes to practise

| In the drawing | In the code | What to say |
| --- | --- | --- |
| Whole scene | `<svg viewBox="0 0 1000 620">` | The top left is `(0,0)`; x grows right and y grows down. CSS scales the same viewBox to fit the page. |
| Wall, sun, cloud | `<rect>`, `<circle>`, `<ellipse>` | A rectangle starts at `x,y`; circles and ellipses use `cx,cy` for their centre. |
| Sun ray, roof | `<line>`, `<polygon>`, `<polyline>` | A line has two endpoints; the polygon is filled, while the polyline traces the roof edge without filling it. |
| Front walk | `<path d="M450 530 C... Z">` | `M` places the first point, `C` curves the path, and `Z` closes it. |
| Number plate | `<rect class="number-plaque">` and `<text class="number-text">` | The plate is at `(420,297)`; the text `106212636` is centred at x = 485. |
| Two windows | `<g class="windows">` containing two `<g class="window">` | Each window has the same rectangle and two lines. Child `translate(...)` sets its position; `.window` CSS styles both alike. |
| Browser DOM | DevTools → Elements | The SVG and both window groups are real DOM nodes and can be highlighted in the browser. |

Try changing the sun's `cx`, the roof's `fill`, or the second window's `translate(570 325)`, then refresh to explain the result.
