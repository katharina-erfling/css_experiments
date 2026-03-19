<img width="1014" height="515" alt="Screenshot 2026-03-19 115643" src="https://github.com/user-attachments/assets/7418fbf4-6b53-4212-8d77-79683288e549" />

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
├── todo/                   ← Animierte Checkbox
│   ├── index.html
│   └── style.css
└── carousel/               ← CSS Only Carousel
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
- **CSS Tooltip** – Tooltip per `position: absolute`, `opacity` und `transform`
- **Sibling-Fade** – Geschwister-Elemente verblassen per `:not(:hover)` Selektor

### ✅ Animierte Checkbox
- Checkmark-Animation per `border-width` und `opacity` Transition – rein per `:checked` Pseudo-Klasse

### 🎠 CSS Only Carousel
- Vollständiges Karussell ohne JavaScript – mit den brandneuen Pseudo-Elementen `::scroll-button()` und `::scroll-marker`
- Navigations-Buttons und Dot-Indikatoren komplett per CSS
- Fallback per `@supports not (selector(::scroll-button()))` – Scrollbar wird automatisch eingeblendet wenn der Browser das Feature nicht unterstützt
- `prefers-reduced-motion` Support
- Aktuell unterstützt in Chrome Canary

---

## 🛠️ Technologien

- **HTML5** – semantisches Markup
- **CSS3** – `::before`/`::after`, `@keyframes`, `transform`, `background-clip: text`, `:not()`, `:checked`, `transition`, `scroll-snap`, `::scroll-button()`, `::scroll-marker`, `@supports`

---

## 🚧 Work in Progress

Dieses Repo wächst mit – neue Experimente kommen regelmäßig dazu.
