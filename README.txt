KING OF DIAMONDS — BEAUTY CONTEST

Files
- index.html: complete standalone game. No libraries, server, API key, or external assets required.

How to play
1. Open index.html in a modern desktop or mobile browser.
2. Select the King of Diamonds (K♦) from the 52-card deck.
3. Read the rules and select Enter the game.
4. Choose an integer from 0 to 100 and lock it in.
5. Review the revealed choices, target, point changes, and newly unlocked rules.
6. Continue until one player remains.

Rules implemented
- Five participants: you and four independent local strategy agents.
- The target is 0.8 times the mean of all active players' selections.
- Closest eligible player(s) win the round; all other active players lose one point.
- Everyone starts with 10 points and is eliminated at zero.
- After 1 elimination: duplicate selections are invalid and the players who selected the duplicate number lose one point.
- After 2 eliminations: an exact target selection makes every other player lose two points.
- After 3 eliminations: when two players remain, choosing 100 defeats a 0 selection.
- Equally close eligible players share the round win.

AI note
The four opponents are four distinct, history-aware JavaScript strategy agents (level-k reasoning, Bayesian-style forecasting, best response, and a randomized mixed strategy). They run locally in the browser and are not external LLM/API models.

Hosting on GitHub Pages
- Create a GitHub repository.
- Upload index.html (and optionally this README.txt) to the repository root.
- In repository Settings > Pages, choose Deploy from a branch, select the main branch and root folder, then save.
- Open the published Pages URL after deployment.

This is a fan-made adaptation, not affiliated with or endorsed by the rights holders of Alice in Borderland.
