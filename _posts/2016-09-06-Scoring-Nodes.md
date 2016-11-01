---
layout: post
title: Scoring Moves
date: 2016-09-06 11:03:41
---

So now I have a functioning decision tree, without any optimizations like alpha-beta pruning quite yet. Let's take a given node, say, a bishop taking rook. How are we supposed to score each decision the tree makes?

First, we need to consider any constraints:

1. The score must be an uint32_t
2. The score must be calculated in almost negligible time, in order to maximize move search time
3. The scoring must only be accomplished with two inputs, board and graveyard

Next, we need to think a bit about what makes a certain game state advantageous. This will be a stand-in for later use of machine learning to develop a scoring mechanism.

1. Some pieces are more valuable than others, and at certain points in the game.
2. Location, location. Piece development matters, if a piece is actually on the board matters, who can drop the piece matters.
3. Forcing check is an advantage
4. etc.

