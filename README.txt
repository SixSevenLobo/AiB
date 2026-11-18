ALICE IN BORDERLAND — PLAYABLE DIAMOND CARDS

Files
- index.html: the complete standalone game collection. Both playable games, all HTML, CSS, and JavaScript are included in this file.
- README.txt: these instructions and the implemented rules.

No libraries, build tools, server, API key, or external assets are required. Open index.html in a modern desktop or mobile browser.

CURRENTLY PLAYABLE CARDS

1. KING OF DIAMONDS (K♦) — BEAUTY CONTEST
- Five participants: you and four independent local strategy agents.
- Each active player chooses a whole number from 0 to 100.
- The target is 0.8 times the mean of all active players' selections.
- The closest eligible player(s) win the round; other active players lose one point.
- Everyone starts with 10 points and is eliminated at zero.
- After 1 elimination: duplicate selections are invalid; players who chose a duplicated number lose one point and cannot win that round.
- After 2 eliminations: an exact target selection makes every other player lose two points.
- After 3 eliminations: with two players remaining, choosing 100 defeats a 0 selection.
- Equally close eligible players share the round win.

2. QUEEN OF DIAMONDS (Q♦) — THE PARADOX AUCTION
Original fan-made game concept.
- Five participants: you and four individual local strategy agents.
- Everyone starts with 15 points. A player is eliminated at zero.
- Each active player secretly submits a bid from 0 to 5 and predicts how many OTHER active players will bid at least 3.
- A unique highest bidder wins the auction. If the highest bid is tied, nobody wins the auction and nobody pays.
- The unique auction winner receives the current auction reward and pays the second-highest bid. Their net auction points are reward minus payment.
- An exact prediction earns +2 points; an incorrect prediction costs 1 point. This prediction adjustment applies to every active player, including the auction winner.
- Rounds 1–6 have a +4 auction reward.
- Rounds 4–6 show a statistical bulletin based on an incomplete sample with deliberate random distortion. It may be misleading.
- From round 7 onward, the Queen secretly selects a +2, +4, or +6 auction reward. It is revealed after submissions are locked.
- The last surviving player wins. If 15 rounds finish with multiple survivors, the surviving player(s) with the highest score win.

QUEEN'S LOCAL AI STRATEGIES
- The Economist: conservative value-based, second-price auction bidding.
- The Manipulator: tracks recent player behavior and adjusts bids/predictions to exploit patterns.
- The Probabilist: uses smoothed historical bid distributions and Monte Carlo expected-utility estimates.
- The Chaos Agent: randomized mixed bidding and prediction strategy.
- The four agents are implemented as local JavaScript strategies; they are not external LLMs and need no API key or internet connection.

HOW TO PLAY
1. Open index.html.
2. Select King of Diamonds (K♦) or Queen of Diamonds (Q♦) from the 52-card deck.
3. Read the corresponding rules and start the game.
4. Submit your choice(s) and review the revealed round results.
5. Continue until the game ends, then restart or return to the deck.

GITHUB PAGES HOSTING
1. Create a GitHub repository.
2. Upload index.html (and optionally README.txt) to the repository root.
3. In repository Settings > Pages, choose Deploy from a branch, select the main branch and root folder, then save.
4. Open the published Pages URL after deployment.

This is a fan-made, non-commercial adaptation/concept, not affiliated with or endorsed by the rights holders of Alice in Borderland.
