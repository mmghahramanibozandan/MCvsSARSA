# MC vs SARSA
Comparison between Monte Carlo algorithm, SARSA- λ  and SARSA- λ  with action-value function approximation.

## Game rules:

- The game is played with an infinite deck of cards (i.e. cards are sampled
with replacement)


- Each draw from the deck results in a value between 1 and 10 (uniformly
distributed) with a colour of _red_ (probability 1/3) or _black_ (probability
2/3).


- There are no aces or picture (face) cards in this game (no issues with usable aces!)


- At the start of the game both the player and the dealer draw one black
card (fully observed)


- Each turn the player may either **stick** or **hit**:
    - If the player hits then he draws another card from the deck
    - If the player sticks he receives no further cards and its turn ends


- The values of the player’s cards are added (if black card) or subtracted (if red
card)


- If the player’s sum exceeds 21, or becomes less than 1, then he “goes
bust” and loses the game, with a reward of -1


- If the player sticks then the dealer starts taking turns, same rules apply to him. The dealer always
sticks on any sum of 17 or greater, and hits otherwise. If the dealer goes
bust, then the player wins, with a reward of 1; otherwise, the outcome – _win_ (reward 1),
_lose_ (reward -1), or _draw_ (reward 0) – is given by the player with the largest sum.

![MC](https://github.com/mmghahramanibozandan/MCvsSARSA/blob/main/download.png)

