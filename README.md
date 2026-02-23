# ice-in-drink melt demo calculator

Single-file web tool (`index.html`) to demonstrate how fast an ice cube melts inside a drink given:
- ambient temperature
- liquid temperature
- ice starting temperature
- cube size
- drink volume
- stirring/motion
- container type (insulation proxy)

It simulates heat flow from liquid→ice and ambient↔liquid with a simple ODE integrator (1 second timestep).

## Publish (share a link)

### GitHub Pages (recommended)
1. Create a GitHub repo (e.g., `ice-melt-demo`)
2. Upload `index.html`
3. Settings → Pages → Deploy from branch → `main` / root
4. Share the resulting URL.

### Netlify Drop
Drag & drop `index.html` into Netlify’s manual deploy UI and share the generated link.

### CodePen
Paste `index.html` contents into the HTML panel.

## Notes
This is for demos. Stirring and liquid temperature dominate melt rate in real drinks.


## Styling
The background changes based on ambient temperature (snow/ice/jackets/blouses/shirts/swim/fire).
