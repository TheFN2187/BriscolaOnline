# Web-Based Briscola 🃏

A fully playable, interactive web-based version of the classic Italian card game **Briscola**. Built entirely with vanilla HTML, CSS, and JavaScript, this project requires no external libraries, frameworks, or backend servers. 

It features an intelligent rule-based AI with three difficulty levels, smooth CSS animations for card tossing and trick clearing, and dynamic visual state management.

## Features
* **Full Briscola Rule Engine:** Accurately handles trick resolution, trump (briscola) prioritization, point values, and scoring.
* **Three AI Difficulties:**
  * *Easy:* Plays completely at random.
  * *Medium:* A heuristic AI that avoids throwing away high-value cards and uses trumps defensively.
  * *Hard:* A strategic AI that bleeds the player's hand, protects high-power trumps, and actively tries to steal the player's high-value cards (Aces and 3s).
* **Polished UI/UX:** Features a gradient baize table, responsive layout, and smooth CSS keyframe animations to simulate the physical feeling of tossing cards onto a table and sweeping up won tricks.

## Setup & Installation

Because this game relies entirely on client-side rendering, you do not need a server to run it.

1. Clone or download this repository to your local machine.
2. Ensure your directory structure looks like this:
   ```text
   /BriscolaGame
   ├── briscola.html
   └── /images
       ├── coins_ace.png
       ├── coins_2.png
       ├── ... (40 face cards)
3. Double-click briscola.html to open it in any modern web browser (Chrome, Firefox, Safari, Edge).

## How to Play
1. **Objective:** A standard Briscola deck has 120 points. The goal is to collect 61 or more points to win.

2. **Card Values:**
* Ace: 11 Points
* 3: 10 Points
* King: 4 Points
* Knight: 3 Points
* Jack: 2 Points
* 7, 6, 5, 4, 2: 0 Points

3. **Gameplay:** The player and the AI each start with 3 cards. The suit of the card placed face-up under the deck is the "Briscola" (Trump) suit.

4. **Winning a Trick:**
* If both cards are the same suit, the highest power card wins.
* If the cards are different suits (and neither is the Briscola), the card that was played first wins.
* If any card is the Briscola suit, it beats any non-Briscola card. If both are Briscolas, the higher power wins.

## Technologies Used
* **HTML5:** For semantic structure and layout.
* **CSS3:** For the radial gradients, flexbox grid system, dynamic text wrapping, and animation transitions (transform, opacity, translate).
* **Vanilla JavaScript (ES6):** For array management, state tracking, DOM manipulation, asynchronous timing (setTimeout), and the AI logic engines.

## Attribution and Assets
The card face imagery used in this project is based on the Triestine (Tršćanske) regional pattern.

**Image Source & Licensing:**
The card assets are attributed to user CCCKKK and are licensed under CC BY-SA 4.0, via Wikimedia Commons.

Note: The physical card backs are generated procedurally using CSS repeating linear gradients, mitigating the need for an external image file.
