# Ice Cube Melting in a Drink — Demo Calculator

An interactive single-file web simulator that estimates how fast an ice cube melts inside a drink.

The model simulates:

- Heat transfer from liquid → ice (depends on stirring and surface area)
- Heat exchange from ambient air ↔ drink (depends on container type)
- Ice enthalpy (warming to 0°C + phase change)
- Dynamic cube shrinkage during melting

The goal is educational demonstration — intuitive, visual, and physically grounded.

---

## 🔧 Current Default Setup

- Ambient temperature: **5°C**
- Liquid temperature: **5°C** (fridge condition)
- Ice initial temperature: **-5°C**
- Cube size: **2.5 cm**
- Drink volume: **250 mL**
- Chart display window: **30 minutes (fixed)**

---

## 🎨 Visual Features

### Dynamic Background Theme (based on ambient temperature)

| Ambient Temperature | Background | Color Theme |
|--------------------|------------|-------------|
| < 0°C              | ❄️ Snow    | Blue        |
| 1–5°C              | 🧊 Ice     | Blue        |
| 6–10°C             | 🧥 Jackets | Blue        |
| 11–20°C            | 👕 Warm    | Yellow      |
| 21–25°C            | 🩱 Swim    | Orange      |
| > 25°C             | 🔥 Fire    | Red         |

The theme color dynamically adjusts the page gradient.

---

## 📊 Chart

The chart shows:

- **Solid line** → Drink temperature (°C)
- **Dashed line** → Ice remaining (%)
- Background → White (scientific clarity)
- Time axis → Fixed to 30 minutes

---

## 🧠 Physics Model Overview

The simulator integrates a time-stepping heat balance:

### Liquid energy balance

m_liq * cp * dT/dt = - q_liq→ice + q_ambient

### Ice melting

Ice mass decreases according to:

dm/dt = q_liq→ice / L_eff

Where:

- L_eff = latent heat + warming energy from initial ice temperature
- Ice surface area shrinks dynamically as cube melts
- Heat transfer coefficient depends on stirring level

This is not lab-grade precision — it is a demonstration-level thermal model.

---

## 🚀 How to Run

Simply open:

index.html:

No build process required. No dependencies.

---

## 🌐 How to Publish

### Option 1 — GitHub Pages

1. Create a new repository
2. Upload `index.html`
3. Go to Settings → Pages
4. Deploy from `main` branch (root)
5. Share your URL

---

### Option 2 — Netlify Drop

Drag `index.html` into Netlify’s manual deploy interface.

---

### Option 3 — CodePen

Paste file contents into the HTML panel.

---

## 📦 File Structure
index.html
README.md
LICENSE

Single-file architecture by design.

---

## ⚠️ Disclaimer

This simulator:

- Assumes homogeneous liquid
- Uses simplified convection coefficients
- Does not simulate stratification or turbulence explicitly
- Is intended for educational demonstration

---

## 📄 License

This project is licensed under the MIT License.
See the LICENSE file for details.