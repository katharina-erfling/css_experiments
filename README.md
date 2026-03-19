# 🧪 CSS Experiments
 
Eine wachsende Sammlung von CSS-Spielereien, Hover-Effekten und Animationen – entstanden beim Lernen und Ausprobieren. Wird laufend erweitert.
 
---
 
## 📁 Projektstruktur
 
```
/
├── index.html              ← Übersichtsseite
├── css/
│   └── index.css
├── link-effects/           ← Link Hover-Effekte
│   ├── index.html
│   └── style.css
├── effects/                ← CSS Effekte
│   ├── index.html
│   └── style.css
└── todo/                   ← Animierte Checkbox
    ├── index.html
    └── style.css
```
 
---
 
## 🧩 Experimente
 
### 🔗 Link Hover-Effekte
6 verschiedene Hover-Animationen für Links – alle rein per CSS:
 
- **Farbslider** – `box-shadow: inset` expandiert von links und übermalt den Hintergrund
- **Textflip** – alter Text gleitet raus, neuer rein per `translate3d` und `data-replace` Attribut
- **Textmarker** – Hintergrund wächst von unten nach oben per `::before` Pseudo-Element
- **Right–Left Color Swap** – Farbe gleitet von rechts nach links per `background-clip: text`
- **Rainbow Underline** – Regenbogen-Unterstrich per `linear-gradient` und `scaleX(0→1)`
- **Passing Underline** – Unterstrich erscheint von links, verschwindet nach rechts per `transform-origin`
 
### ✨ CSS Effekte
- **Spinner/Loader** – `@keyframes` Animation mit `border-radius` und einfarbigem `border-bottom`
- **CSS Tooltip** – Tooltip per `position: absolute`, `opacity` und `transform` – kein JavaScript
- **Sibling-Fade** – Geschwister-Elemente verblassen per `:not(:hover)` Selektor
 
### ✅ Animierte Checkbox
- Checkmark-Animation per `border-width` und `opacity` Transition – kein JavaScript, rein per `:checked` Pseudo-Klasse
 
---
 
## 🛠️ Technologien
 
- **HTML5** – semantisches Markup
- **CSS3** – `::before`/`::after`, `@keyframes`, `transform`, `background-clip: text`, `:not()`, `:checked`, `transition`
- **Kein JavaScript**, kein Framework, kein npm
 
---
 
## 🚧 Work in Progress
 
Dieses Repo wächst mit – neue Experimente kommen regelmäßig dazu.
 
