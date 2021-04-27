# puzzlescript-bfs


A BFS (Bread-First-Search) demo for puzzle script. BFS is a search algorithm that's one of the simplest way to find the minimum 
path between two nodes in a network assuming all steps are weighted the same.

![https://raw.githubusercontent.com/vexorian/puzzlescript-bfs/main/mazesolver2.gif](GIF preview)

## Try it

* Paste the [puzzlescript source code](https://github.com/vexorian/puzzlescript-bfs/blob/main/source.puzzlescript) file into: https://pancelor.com/PuzzleScript/editor.html
* Click run.
* "Play" the levels, you are the blue square, the red squares will kill you if they touch you and you'll notice they are quite smart.
* To "win" (skip to next level) press X.

## How does it work?

There are no queues in puzzle script, so we have to simulate one. By using a couple of adjacency rules with conditions, the level is basically filled with dummy objects with two variations in order of distance to the player. If there is a wall or a monster, the search no longer spreads the adjacency rule.

