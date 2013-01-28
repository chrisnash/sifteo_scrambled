### About Scrambled

_scrambled_ is an entry for the Experimental Gameplay Project Sifteo competition.

The idea behind _scrambled_ was to construct a puzzle game using three Sifteo cubes that
would use the cube's capabilities to produce a game that was only possible on the cubes.
_scrambled_ is based on familiar puzzle games that slide tiles or roll colored balls.
However, using the cubes, we can produce a game board that change by moving the cubes
around.

### Launching

The _scrambled_ proof-of-concept demo may be launched by downloading the file
[scrambled.elf][scrambled_elf]. If the Sifteo SDK is installed, It may be executed in the Sifteo simulator
either from the icon or with

    $ siftulator scrambled.elf

or installed on the Sifteo Base to be played on real hardware with

    $ swiss install scrambled.elf

### How To Play

Each cube contains a section of pipe, each with several different colored balls. There are
a different number of balls in each pipe, and a corresponding number of balls of each color.

![Initial layout][initial]

Pipes may be joined in pairs to form closed loops by rotating the cubes and neighboring
the open sides of the pipes together (drag and rotate the cubes with the mouse, or click
and tap space to quickly rotate).

![Neighbor two cubes][neighbor]

Balls may be rolled around the pipes by tilting one of the neighbored cubes up or down
to rotate the balls in either direction (right-drag or shift-drag the cube). Don't worry,
a single tilt will just rotate the balls one notch around the loop.

![Tilt a neighbor][tilt]

![Result of the tilt][aftertilt]

The initial configuration of the balls may be randomly shuffled by shaking one of the cubes.
To make this easier to do in the siftulator, you may also flip a cube face down to shuffle
(while mouse clicking on a cube, press X).

![Flip or shake to shuffle][flip]

Of course, the object of the game is to restore the balls to their original configuration,
each pipe in a single color. One pipe is reasonably easy; all three pipes presents a genuine
challenge. The puzzle is always solvable!

There are three difficulty levels in the demo. Just touch one of the screens to switch to
a different level. The game starts on easy, with 24 balls. If you think you can manage that,
how about 36? Or even 66?

![Medium level: 36 balls][medium]

![Hard level: 66 balls][hard]

### Suggestions

The idea is to present a very tactile game; the tilt operation will be a natural 'twist'
when holding the two cubes together, one in each hand. This might require some adjustments
of the tilt sensitivity to give the most satisfying 'feel' to the puzzle in the player's
hands.

The game readily extends to more cubes, by adding more pipes and more colors. With sufficient
cubes, the game may be played cooperatively (each player working on a subset of the cubes)
or competitively (by having two or more separate games running simultaneously on a group
of the cubes for each player). The number of cubes is limited by the amount of video memory
required to perform the animations and to store the graphics for all the balls; that should
support quite a fair amount of cubes.

For added challenges, the individual balls may be labelled, for example, requiring the
players to not only place the colors correctly but also in the right order. A thematic
element may be to label the cubes with letters, thus requiring solving an anagram.

One suggestion for a game setting would be something like in Word Caravan. Each puzzle
solved (a 'small' reward for a single color solution, a larger reward for an all colors
solution) would reveal a piece of an image - for example, prehaps retrieving pieces of
a work of art in an art gallery. Complete the puzzle to unlock harder levels.

The number of puzzles available can be quite large. Each pipe can contain anywhere between
4 and 23 balls. While the dynamics of the puzzles remain the same, the moves to be
discovered to master each puzzle and completely solve it can depend a lot on the number
of balls in each cube, especially if the balls are individually labelled.

And yes, for those who are interested, there are indeed as many as 23 balls moving on
each cube on the hardest level, and no, they are not all sprites. Another part of the
challenge for me was to make everything animate as smoothly as possible on the cubes.

[scrambled_elf]:	https://github.com/chrisnash/sifteo_scrambled/raw/master/scrambled.elf	"Scrambled ELF file"
[initial]:		https://github.com/chrisnash/sifteo_scrambled/raw/master/initial.png	"Initial display"
[neighbor]:		https://github.com/chrisnash/sifteo_scrambled/raw/master/neighbor.png	"Neighbor cubes"
[tilt]:			https://github.com/chrisnash/sifteo_scrambled/raw/master/tilt.png	"Tilt a neighbored cube"
[aftertilt]:		https://github.com/chrisnash/sifteo_scrambled/raw/master/aftertilt.png	"Result after a tilt"
[flip]:			https://github.com/chrisnash/sifteo_scrambled/raw/master/flip.png	"Flip or shake to shuffle"
[medium]:        	https://github.com/chrisnash/sifteo_scrambled/raw/master/medium.png	"Medium level: 36 balls"
[hard]:        		https://github.com/chrisnash/sifteo_scrambled/raw/master/hard.png	"Hard level: 66 balls"
