# merlinjack

Original source:
http://nand2tetris-questions-and-answers-forum.32033.n3.nabble.com/My-chapter-9-project-td4034929.html

## Magic Square

The goal of the Magic Square game is to finish with the game state as a square. 

Start by choosing a difficulty level corresponding to about how many steps to
reach the solution on the left.  Each choice of a pip inverts itself and two or
more neighboring pips.  For example a corner pip (1, 3, 7, or 9) inverts each
of its three neighboring pips as well as itself.  The center pip, #5, inverts
itself and pips 2, 4, 6, and 8.  Finally, the middle edge pips, invert all pips
of its edge.

History:  This game was one of the built-in games in the late 1970's Parker
Bros. handheld game, Merlin.  This implementation was inspired by the assembly
language version in the book "6502 Games" (c) 1980 by Rodney Zaks.

### Interesting Implementation Notes

- The user is asked to pick a difficulty in order to generate a uP tick count
  to help in seeding a random generator.
- Python script is included to generate Jack code from a TIFF file.
- Graphical font elements (pip numbers) are from the Apple ][.
