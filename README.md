# ⚔ Continental Divide

A simple, browser-based turn-based strategy game — five colonial powers, thirty historical leaders, one continent. Every power is out for itself: there's no diplomacy here, just conquest.

It's a single self-contained HTML file. No build step, no dependencies, no server required.

## Play

Download or clone this repo, then just open `index.html` in any modern browser (double-click it, or drag it into a browser tab). Everything — markup, styling, and game logic — lives in that one file.

Or enable [GitHub Pages](#deploy-to-github-pages) for a shareable live link.

## The Powers

| Power | Capital | Flavor |
|---|---|---|
| British America | Boston | The Crown's thirteen colonies, ambitious and growing |
| New France | Quebec | Fur trade and faith along the St. Lawrence |
| New Spain | St. Augustine | Missions and garrisons guarding La Florida |
| New Netherland | New Amsterdam | Merchant traders of the Hudson River |
| Iroquois Confederacy | Onondaga | The Haudenosaunee, masters of the eastern woodlands |

Each power starts with 6 leaders (30 total), 2 home territories, and 150 gold. The remaining 4 territories on the map — Philadelphia, Fort Duquesne, Fort Detroit, and Charleston — start unclaimed and lightly garrisoned.

Seven leaders are legendary and fight 15% harder than their stats alone suggest: George Washington, Benjamin Franklin, and Francis Marion for British America; the Comte de Frontenac for New France; Bernardo de Gálvez for New Spain; Peter Stuyvesant for New Netherland; and Joseph Brant for the Iroquois Confederacy.

## How to Play

1. Pick a power on the start screen. The other four are played by the AI, and every one of them — including toward you — will attack whichever neighboring territory looks weakest. There are no allies here.
2. Click a territory you own — holding territory pays you gold every turn, the more you hold, the richer you get.
3. **Recruit** troops with gold (2 gold per troop).
4. **Train & Equip** a territory's militia (5 levels, rising cost) to fight harder, both attacking and defending.
5. **Assign** a reserve leader to a territory to boost its attack and defense. Legendary leaders (★) hit harder than their stats show.
6. **Move troops** between two territories you already own, Risk-style, to reinforce a threatened front.
7. **Attack** an adjacent rival or unclaimed territory. Battles weigh troop counts, training level, leader stats, defensive terrain, and a bit of randomness. Win, and you seize the territory — and sometimes the enemy leader, who may defect to your side!
8. Click **End Turn** to collect income and let the other four powers act — expect them to come after you and each other.
9. **The game is on a clock.** You start with 40 turns, but every territory you hold beyond your starting two extends the clock by 3 turns — expansion buys you more time. Conquer every territory, eliminate every rival, or simply hold the most ground when time runs out to win.

## Layout

The map sits front and center at the top and scales up with the window. Below it, a bar holds the territory panel (recruit, train, assign leaders, move troops, attack) alongside your Leaders roster. The Campaign Log runs as a full-height column on the right, so the play-by-play never crowds out the map.

## Project Structure

```
continental-divide/
├── index.html   # everything: markup, styles, and game logic
├── LICENSE
└── README.md
```

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save — your game will be live at `https://<your-username>.github.io/<repo-name>/`.

## License

MIT — see [LICENSE](LICENSE).
