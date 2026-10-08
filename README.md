# Snakes & Ladders

A single-file browser game of Snakes & Ladders. Open `index.html` in any modern browser, no build step needed.

- 2–4 players, each human or computer-controlled, with typed-in player names
- Play on one device, or **online with friends**: host a room, share the 5-character code or link, and everyone plays from their own browser
- Sound effects (synthesised in the browser, toggle with the Sound button)
- Animated dice, hopping tokens, ladder/snake highlights and a win celebration
- Score history (leaderboard and recent games), stored in the browser
- Classic 10×10 board with 9 ladders and 10 snakes; exact roll needed to land on 100; a 6 gives another turn
- Press **Space** (or click the button) to roll

## Online play

Online rooms use [PeerJS](https://peerjs.com/) (WebRTC). The library and its free public matchmaking
server are used only to connect players; moves and names then go directly between browsers.
The host's browser rolls the dice for everyone. If a player disconnects mid-game, the computer takes over their seat.

## Play online (hosting)

Once GitHub Pages is enabled (Settings → Pages → Source: **GitHub Actions**), the game is served at
https://dasmraja.github.io/Claude-Cloud/ and redeploys on every push to `main`.
