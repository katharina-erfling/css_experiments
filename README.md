<img width="1014" height="515" alt="Screenshot 2026-03-19 115643" src="https://github.com/user-attachments/assets/7418fbf4-6b53-4212-8d77-79683288e549" />

# 🧪 CSS Experiments
Eine wachsende Sammlung von CSS-Spielereien, Hover-Effekten und Animationen – entstanden beim Lernen und Ausprobieren.

## 🚧 Work in Progress
Dieses Repo wächst mit – neue Experimente kommen regelmäßig dazu.

---

## 📁 Projektstruktur
```
/
├── index.html                  ← Übersichtsseite
├── css/
│   └── index.css
├── link-effects/               ← Link Hover-Effekte
│   ├── index.html
│   └── style.css
├── effects/                    ← CSS Effekte
│   ├── index.html
│   └── style.css
├── todo/                       ← Animierte Checkbox
│   ├── index.html
│   └── style.css
├── carousel/                   ← CSS Only Carousel
│   ├── index.html
│   └── style.css
├── text-effekte/               ← Text-Effekte
│   ├── index.html
│   └── style.css
├── infinite-carousel/          ← Infinite Carousel
│   ├── index.html
│   └── style.css
├── glass-effect/               ← Glass Morphism Effekt
│   ├── index.html
│   └── style.css
└── 3D-Carousel/                ← 3D Carousel
    ├── images/
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

### ✍️ Text-Effekte
- **Schreibmaschinen-Effekt** – Text tippt sich Zeichen für Zeichen per `width`-Animation und `steps()` ein
- Cursor blinkt per `border-right` Animation
- Replay-Button setzt die Animation per JavaScript zurück (`animation: none` → Reflow erzwingen → neu setzen)
- Wird laufend um weitere Texteffekte ergänzt

### 🎡 Infinite Carousel
- **Horizontales Auto-Scroll Carousel** – nahtloser Loop per `@keyframes` und `translate`, zwei identische Gruppen für den Infinite-Effekt
- **Vertikale Auto-Scroll Carousels** – vier Spalten im Wechsel hoch und runter per `translateY`
- Fade-Effekt oben und unten per `mask-image` Gradient
- `aria-hidden="true"` auf duplizierten Gruppen für Screenreader
- Fallback per `@supports not (translate: 0)` für ältere Browser
- `prefers-reduced-motion` verlangsamt statt stoppt

### 🪟 Glass Morphism
- Milchglas-Effekt per `backdrop-filter: blur()` und halbtransparenter Hintergrundfarbe
- Subtile Border-Highlights per `border-top` und `border-left` mit `rgba()`
- `-webkit-backdrop-filter` für Safari-Kompatibilität
- Responsive Card per `min()` und `clamp()`
- `prefers-reduced-motion` Support

### ⚡ 3D Carousel
- Rotierendes 3D-Bilderkarussell per `perspective`, `transform-style: preserve-3d` und `rotateY`
- 10 Bilder gleichmäßig im Kreis verteilt per `calc()` und CSS Custom Properties (`--position`, `--quantity`)
- Automatische Rotation per `@keyframes` mit `rotateX(-15deg)` für den Kippwinkel
- Neon-Typografie per `::after` Pseudo-Element mit `-webkit-text-stroke` und `rgba()` Overlay
- Hintergrundbild positioniert per `background-position: top center` und `background-size: auto 130%`
- `z-index`-Schichtung für Tiefenwirkung zwischen Slider, Typografie und Hintergrundbild

---

## 🛠️ Technologien
- **HTML5** – semantisches Markup
- **CSS3** – `::before`/`::after`, `@keyframes`, `transform`, `translate`, `background-clip: text`, `:not()`, `:checked`, `transition`, `scroll-snap`, `::scroll-button()`, `::scroll-marker`, `@supports`, `mask-image`, `steps()`, `backdrop-filter`, `min()`, `clamp()`, `perspective`, `rotateY`, `translateZ`, `-webkit-text-stroke`
- **JavaScript** – minimal, nur für Animation-Reset (Text-Effekte)
