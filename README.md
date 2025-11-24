# Portfolio

Ein persönliches Portfolio mit modularer, klar strukturierter SCSS-Architektur.  
Alle Seiten basieren auf denselben globalen Layout-, Navigations- und Footer-Strukturen.  
Seitenspezifisches Verhalten wird sauber über eigene SCSS-Module geregelt.

---

## 📁 Projektstruktur

root/
│── index.html
│── me.html
│── art.html
│── code.html
│── contact_me.html
│
│── styles/
│      ├── main.scss
│      ├── base/
│      │     ├── _reset.scss
│      │     ├── _fonts.scss
│      │     ├── _layout.scss
│      │     ├── _nav.scss
│      │     ├── _footer.scss
│      │     ├── _components.scss
│      │     └── _responsiveness.scss
│      │
│      ├── index/
│      │     ├── _index_shared.scss
│      │     └── _index_light.scss
│      │
│      ├── me/
│      └── contact_me/
│
├── pictures/
├── icons/

## 🧱 SCSS Architektur

### `base/`  
Globale Styles, die für **alle Seiten** gelten:
- Reset  
- Schriftarten  
- Layout  
- Navigation  
- Footer  
- Komponenten  
- Responsiveness (alle globalen Breakpoints)

### `index/`  
Alle spezifischen Styles nur für die Startseite:  
- Hintergrund-Animation  
- Header-Farbe  
- Startseitenlayout

### Weitere Seiten (`me/`, `contact_me/`, …)  
Jeder Bereich besitzt eigene SCSS-Module, um Logik/Design sauber zu trennen.


## ⚙️ SCSS lokal kompilieren


sass styles/scss/main.scss styles/main.css --watch


## ✅ To-Dos

* add art page
* rm boldness from nav
* fix contact me page
* fix background image and animation of pages
* make nav and footer on every page the same
* add art
* add projects
