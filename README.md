

# GoBoard Arena — Decentralized Strategy Engine

GoBoard Arena is an open-source strategy platform that merges the complete rule engine of ancient Go (Weiqi / Baduk) with modern Web3 technologies and a lightweight 2D Canvas rendering architecture. It operates entirely on native HTML5 Canvas, Vanilla JavaScript, and Solana Web3.js infrastructure with zero external game framework dependencies.

---

## 🚀 Key Features

* **Comprehensive Rule Engine:**
  * **Liberty Calculation:** Recursive/queue-based flood-fill analysis to track connected stone chains and group liberties after every move.
  * **Capture Mechanics:** Dynamic removal of surrounded stone groups from the board, highlighted with custom particle burst animations.
  * **Suicide Prevention:** Strict validation that rejects self-destructive moves unless they result in an immediate opponent capture.
  * **Ko Repetition Guard:** Board state hashing and history tracking to prevent infinite repeating loops under the classical Ko rule.
* **Dynamic Board Configurations:** Seamless support for 9×9 (Speed Strategy), 13×13 (Medium Board), and 19×19 (Official Professional Standard) with accurate star-point (Hoshi) positioning.
* **Zero-Dependency 2D Canvas Engine:** Built without the overhead of heavy frameworks; features procedural wood texture styling, radial gradient shaded stones with realistic depth, last-move indicators, and a custom particle engine.
* **Web3 Profile Integration:** Wallet detection and session persistence (`localStorage`) supporting Phantom, Solflare, and Backpack, along with an instant Guest mode.
* **Cross-Platform Responsive Design:** Dynamic coordinate translation optimized for both touch devices and desktop mouse/keyboard inputs.

---

## 🛠️ Architecture & Technical Stack

| Component | Technology / Details |
| :--- | :--- |
| **UI & Rendering** | Vanilla HTML5, CSS3 Custom Properties, Canvas 2D API |
| **State Machine** | 2D matrix-based deterministic game state controller |
| **Web3 Layer** | `@solana/web3.js` (Provider Detection & Public RPC Fallbacks) |
| **Particle Physics** | Native `requestAnimationFrame` particle scattering system |
| **Deployment** | Zero-build static asset pipeline (GitHub Pages / Vercel ready) |

---

## 📦 Getting Started

No bundlers, package managers, or build steps are required to run the project locally.

1. Clone the repository:
   ```bash
   git clone [https://github.com/inandenizturk/goboardgame.git](https://github.com/inandenizturk/goboardgame.git)
   cd goboardgame
