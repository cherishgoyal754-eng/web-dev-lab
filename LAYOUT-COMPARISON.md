# Practical P13: Choosing Between Flexbox and CSS Grid

**Student:** Cherish Goyal  
**Institution:** Bosscoder School of Technology  
**Assignment:** Module 3 (CSS Layout Systems)

---

## 1. Core Structural Differences

| Characteristic | CSS Flexbox | CSS Grid |
| :--- | :--- | :--- |
| **Dimensions** | **One-Dimensional (1D)**: Arranges elements along a single axis (row OR column). | **Two-Dimensional (2D)**: Aligns elements along rows AND columns simultaneously. |
| **Design Concept** | **Content-First**: Sizing is determined by child contents. | **Layout-First**: Container defines strict tracks/grid lines. |
| **Row/Column Alignment** | Wrapped rows do not align vertically with items in other rows. | Strict two-axis alignment across every row and column. |
| **Best Application** | Navbars, buttons, form controls, tag badges. | Full page layouts, magazine layouts, auto-fitting card grids. |

---

## 2. Flexbox Implementations in This Project
- **Navigation Bar (`.navbar`):** Used `display: flex; justify-content: space-between;` to distribute the logo and navigation links.
- **Hero Banner (`.hero-block`):** Used flexbox to arrange the introductory copy alongside the profile badge card.
- **Footer Columns (`.footer-columns`):** Responsive multi-column layout using `flex-wrap: wrap;` and `flex: 1 1 200px;`.

---

## 3. CSS Grid Implementations in This Project
- **Projects Grid (`.projects-layout-grid`):** Auto-fitting responsive columns using `repeat(auto-fit, minmax(280px, 1fr));`.
- **Featured Card Span:** Applied `grid-column: span 2` to highlight the primary project on larger viewports.
- **Newspaper Layout (`.newspaper-editorial-grid`):** Employed `grid-template-areas` with fractional tracks (`2fr 1.2fr 1fr`) to reconstruct a classic 3-column front page.

---

## 4. Architectural Summary
Modern web design leverages both engines together: **CSS Grid designs the macro page scaffold**, while **Flexbox organizes the micro components** inside each container.
