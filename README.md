## Implementation can run on Jupiter or Google Collab

# Poker-RL
Simplified Poker game using various Agents:

# Reinforcement Learning Agent:
Plays Poker by using Policy Iteration Algorithm

# Random Agent:
Plays Poker randomly

# Q-Learning Agent:
Learns and plays poker optimally using Q-Learning.

#Human Agent:
Plays poker by giving commands, using a UI.

# Poker Rules: 
Environment (Simplified Poker Game):

Assume 4-5 cards are used only: e,g, 10, J,Q,K,1 (adjust according to the solution time needed on colab or your PC) - In the final version this will be the entire deck.
Each player is dealt, only one card in hand which is private (in Texas Hold'em this will be two cards per player)
Only two cards will be set on the table (in Hold'em there'll be 5).
The betting rounds and how the table cards are uncovered will be as follows:
Round 1: Each player sees their own card, but the 2 table cards are still unknown; Player 1 can check or bet 1 token.
In case of check: Player 2 can also check, or raise one token. In the latter case, Player 1 can fold or bet 1 token too.
In case of betting: Player 2 can fold, bet 1 token also, or raise 1 token (i..e bet a total of 2). In the latter case, player 1 can fold, or bet that extra token (this is not a "re-raise", player 1 just "meets" the raise of player 2)
Round 2: Both table cards are Τηrevealed. Another betting round follows with the same rules as Round 1.
The winning rules are the following:
best combination is 3 of a kind
then 1 pair: highest pair wins (with order as usual: 1,K,Q,J,10). In case of same pair (but different suit), highest 3rd card wins.
If no pair by any player, highest card wins.
ignore "flush" (3 of same suit) for this simpler setup.
Ante: Assume that before even being dealt the initial card, each player must always bet 0.5 tokens. (You should think what would happen if there is no such "ante" and what the optimal policy is that your agent will - hopefully - learn).
Note: for implementing this environment, this python library was used: https://rlcard.org/

