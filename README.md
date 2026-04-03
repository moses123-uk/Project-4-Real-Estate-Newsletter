# 📧 Project 4: Hybrid-Responsive Real Estate Newsletter

**Category:** Content Marketing / Lead Generation  
**Goal:** To showcase multiple property listings in a high-end, gallery-style layout that remains functional and beautiful across 50+ email clients.

### 🛠️ Technical Highlights
* **Hybrid-Fluid Layout:** Developed a custom "Ghost Table" structure using **MSO conditional code** to allow a 2-column property grid on Desktop that automatically "stacks" into a single column on Mobile.
* **VML Background Hero:** Implemented a **VML Rectangle (`v:rect`)** for the hero banner. This allows for "Live Text" (Searchable/Selectable) to sit on top of the background image, ensuring the message is visible even if images are blocked.
* **Advanced Stacking Logic:** Used `display: inline-block` and `max-width` constraints on `<div>` containers to achieve responsiveness without relying solely on `@media` queries (which are often stripped by Gmail/Outlook).
* **Interactive Elements:** Features hover-effect simulated buttons and high-contrast dividers (`border-bottom`) to maintain brand consistency throughout a long-form scroll.

### 📱 Performance & Rendering
* **Cross-Client Tested:** Verified rendering for **Outlook 2013-2019 (Desktop)**, Gmail (iOS/Android), and Apple Mail.
* **Typographic Control:** Used a specific web-safe font stack (`Arial, Helvetica, sans-serif`) to ensure a premium look regardless of the user's operating system.
* **Asset Optimization:** Utilized 2x resolution imagery for property photos to ensure "Retina" clarity on modern smartphone displays.

---
**Technical Solution:** Solved the "Side-by-Side Breaking" issue in Outlook by wrapping `inline-block` divs in a 600px width-constrained MSO table, forcing a perfect desktop grid while allowing mobile fluidity.
