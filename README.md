# [Dark Elegance] // DOCTRINE OPERATIONAL MANUAL

### Tactical Minimalism. Cinematic Intent.
This repository houses the front-end style guide and asset doctrine for the **RyanrealAF** brand identity. It is a blueprint for **Operational Clarity** and serves as the single source of truth for all visual, tonal, and structural decisions. Every element must earn its place. No clutter. No compromise.

---

## 🎯 SECTION 01: THE DOCTRINE (GOAL)

This is not a mere mood board; it is a **Command Center** rendered in code. Its core function is to establish and enforce the following constraints:

* **Aesthetic Discipline:** Monochrome foundation (Charcoal, Matte Black) with **Metallic Bronze** reserved only for primary calls-to-action (CTAs) and critical focus points.
* **Structural Friction:** Utilizing default-open/default-closed states (`<details>`) to manage information density, forcing the user to deliberately engage with secondary reference material.
* **Rhythmic Flow:** Utilizing the `Playfair Display` header font for cinematic emphasis and `Inter` or `Segoe UI` for fast, efficient reading (Tactical Minimalism).

---

## 🛠️ SECTION 02: DEPLOYMENT (SETUP)

To deploy the Doctrine successfully, follow the constraints below. Failure to adhere to the file structure will result in the code rendering errors previously observed.

### I. Dependencies
* **Fonts:** Google Fonts inclusion (Inter, Playfair Display).
* **Assets:** Logo (`./images/ryanrealfv.png`) must be present in the root directory's `images/` folder.
* **Images:** All referenced images are currently linked via Unsplash URLs (mood-board references) and can be hot-linked or replaced with local assets.

### II. Installation & Execution
1.  **Clone the Repository:**
    `git clone [REPO_URL]`
2.  **Verify File Structure:** Ensure the main style guide is located at `/index.html`.
3.  **Local Execution:** Open `index.html` directly in your browser.
4.  **Deployment (GitHub Pages):** Push the code to the primary branch (`main` or `master`). Ensure the repository settings are configured to serve content from the **Root** branch.

---

## ⚙️ SECTION 03: KEY COMMANDS (VARIABLES)

The entire aesthetic is governed by the CSS variables defined in the `:root` block. To maintain the **integrity of the Doctrine**, changes must only be made to these specific tactical assignments.

| Variable Name | Hex Code | Purpose |
| :--- | :--- | :--- |
| `--bg` | `#0d0d0d` | **Foundation:** Deepest ambient black. |
| `--panel` | `#151515` | **Container:** Standard module background. |
| `--text` | `#e8e6e3` | **Clarity:** Primary readable text color. |
| `--bronze` | `#d4af37` | **The Weapon:** Exclusive color for CTAs, focus, and open states. |
| `--glow` | `0 0 24px...` | **Cinematic Intent:** Shadow for critical, active elements. |

### The Critical Rule
The `var(--bronze)` must never be used on non-actionable text or purely decorative elements. Its presence must trigger immediate **user priority**.

---

## 💥 SECTION 04: TROUBLESHOOTING (FAILURE ANALYSIS)

### Symptom: Raw Code Display
If CSS or HTML content is visible as text on the live page, the deployment framework is failing.

| Fault Line | Action |
| :--- | :--- |
| **Parsing Error** | Move all CSS from `<style>` to an external `style.css` file and link it. This decouples the aesthetic from the HTML body. |
| **Template Conflict** | Verify no external templating engine (Jekyll, Liquid) is wrapping your `index.html` and accidentally breaking the `<head>` closure. |
| **Improper Encoding** | Ensure file is saved using UTF-8 encoding, and verify no stray characters exist before `<!DOCTYPE html>`. |

***

### Lyrical Constraint (The Core Function)
This ReadMe is the system by which you ensure **Authenticity Ain't Optional.** It is the rigid structure that allows the vulnerability in your content to shine through. The framework must be unforgiving, so the message can be true.
