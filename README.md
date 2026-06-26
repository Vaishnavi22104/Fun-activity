# ☁️ GDG Cloud Nagpur - Live Vibe Event Activity

A playful, interactive, real-time web application built for GDG Cloud events. Attendees scan a QR code to join the "Cloud Vibe," sending floating, physics-enabled bubble cards with their names onto a big projector screen. The host can then trigger a dynamic lottery animation to pick 10 random winners from the live pool.

---

## 🚀 Live Demo Links
Anyone visiting this repository can open and test the application instantly:
* 📱 **Attendee Join Screen (Mobile):** [gdg-cloud-activity.vercel.app](https://gdg-cloud-activity.vercel.app)
* 🖥️ **Presentation Screen (Projector View):** [gdg-cloud-activity.vercel.app/projector.html](https://gdg-cloud-activity.vercel.app/projector.html)
* 🔒 **Event Manager Dashboard (Admin):** [gdg-cloud-activity.vercel.app/host.html](https://gdg-cloud-activity.vercel.app/host.html)  
  *(Default Host Password: `gdgcloud`)*

---

## ✨ Features
* **Real-time Synchronization:** Powered by Firebase Realtime Database, syncing attendee joins and lottery phases across all client screens simultaneously.
* **Dynamic 2D Physics Engine:** Interactive floating bubbles that repel, bounce, and collide organically within screen boundaries.
* **Auto-Scaling Bubble Radius:** Gracefully shrinks bubble sizes as more attendees join so the presentation screen never overflows.
* **Centripetal Drift:** Subtle center-gravity pulling bubbles into a centralized cluster for optimal viewing.
* **3-Phase Lottery Reveal:**
  1. **Roulette:** Bubbles snap-blink randomly with glowing color animations.
  2. **The Focus:** All non-winners fade out while the 10 selected winners grow to 1.35x scale and pop forward.
  3. **Winner Grid:** Transition into a celebratory winner list with individual and full-screen confetti bursts.
* **Playful GDG Vibe:** Glassmorphism card aesthetics, a subtle dotted background in brand colors, and animations for Google Android mascots.

---

## 🛠️ Tech Stack
* **Frontend:** Vanilla HTML5, CSS3, ES6 JavaScript modules.
* **Styling:** Tailwind CSS via CDN.
* **Database:** Firebase Realtime Database.
* **Animations & Effects:** HTML Canvas Confetti API.
* **Deployment:** Vercel.

---

## 📂 File Structure
* `index.html`: Mobile join screen that transitions into an attendee's personal live bubble view.
* `projector.html`: Purely visual projector screen displaying live attendee bubbles and lottery results.
* `host.html`: Host panel for triggering roulette, revealing winners, resetting the display, or wiping database records.
* `ASSETS/`: Graphics, branding elements, and Google Antigravity logo assets.

---

## 🔧 Local Setup & Run
1. Clone this repository:
   ```bash
   git clone https://github.com/Vaishnavi22104/gdg-cloud-activity.git
   cd gdg-cloud-activity
   ```
2. Run a local server (e.g., using Python or Node):
   * **Python:** `python -m http.server 8000`
   * **Node (npx):** `npx live-server`
3. Open `index.html`, `projector.html`, and `host.html` side-by-side in your browser.

---
*Made with 💖 and Google Antigravity*
