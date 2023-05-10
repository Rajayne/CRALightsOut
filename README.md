# CRALightsOut

Clicking on a cell toggles that light, as well as the lights above, beside, and below it. (Cells on an edge or corner won’t flip as many lights, since they are missing some neighbors).

## Plan

Before reading further, take a moment to think about how you would design this, component-wise.

## Code

This game will be built from three components:

### App

Renders the board component.

### Board

Holds state for lights-on/off for cells.

### Cell

Renders a `<div>` where the CSS classes will indicate whether this cell is lit or unlit.

- Click toggles lights-on/off

When the game is won, hide game board with “You Won” message showing in its place.

## Further Study

### Default Properties

Add default properties for the board sizes and how likely it is that a light on the initial board is turned on or off.

### Add Tests

Add tests for:

- rendering a Cell properly
- rendering the starter Board
- handling cell-clicking: non-shallow render the Board, find a cell, then ensure that clicking it causes the right cells to flip.
- checking for a win and showing a “You won!” message

### Improve CSS

Try including better colors, rounded shapes, or CSS animations

### Ensure A Game Is Winnable

Depending on the size of the board, some on/off starting configurations may not be solvable (see [here](https://ida.mtholyoke.edu/xmlui/bitstream/handle/10166/693/375.pdf?sequence=1&isAllowed=y) for information on solvability).

Figure out how to do this.
