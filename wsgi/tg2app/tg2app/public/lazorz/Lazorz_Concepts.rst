Vin's Thoughts
==============
Lazorz Ideas: 1-4 players, 3x3 OVERALL grid so a total of 9 game boards. For
one player, 8 of 9 are locked, and the object is to unlock the surrounding
boards and ultimately complete the middle puzzle. For 2 players, each player
has an initial board unlocked and they have to solve the other 3 in order to
unlock the middle board together, where they will then cooperate to solve the
final multi laser puzzle. Also, as the player number increases, the number of
game boards could increase as well.

Now taking that overall gameplay, I think the most fitting idea (theme) would
be like a tomb or temple. Just stoney and ancient looking. Players would start
in their own temple room, and to succeed would need to complete their lazor
puzzle to unlock the door to the next puzzle, a more difficult temple room.
Once a player complete's their required temple rooms, their laser would be
projected into the lock of the final middle room and when all players lasers
hit the lock of the middle room, it is unlocked and they are required to use
all four lasers to solve the puzzle and unlock a relic. This adds a story
element in the way that you're trying to explore the temples and solve the
puzzles to ultimately retrieve the relic/prize within. Temple rooms could
contain enemies that need to be defeated in order to proceed like big spiders,
or even mummies, or ghosts.

Now to flip that completely and make the game a bit more of a competition
rather than working together, you could have the players starting in the middle
each with their own lazor and have them fighting to see who can escape the
temple the fastest by completing temple rooms, which could be another story
element to the previous idea. Have them work together to reach the relic, that
when removed causes a collapse or something to change where now it's somewhat
of a race of who can get out the fastest. Points could be awarded for having
the relic when you finish, finish the fastest, using the least mirrors or
objects to complete the puzzle etc.

I definitely think the temple, ancient esque theme is the best route. It
carries that idea of exploration that all kids enjoy.

Lorin's Thoughts
================
We have a grid, some tiles, a beam of sorts, and the potential for various
mirrors and other obstacles and objects. What do we do now?

Sticking with our initial idea of the player having a start and end point, and
the only goal is to solve the puzzle by manipulating the objects, changing the
direction of the beam: The theme could appear very space oriented. The
background of the grid is like a typical moon surface pattern. The character
was an astronaut, exploring a distant planet and discovered some sort of cave
(does the back story need that much detail since we aren't showing it?) where
they are trapped and these puzzles (sort of like Indiana Jones on the moon) are
their only way to get out. If we're playing with multiple players then they're
all trapped and trying to get out together by solving their own interlocking
puzzles to make it out. Once one puzzle is solved, then the one's outside of it
are unlocked and they are playing from center tile outward on a larger game
grid.

This game type would allow for cooperative multi-player, and focus solely on
the principles of reflection using flat, concave, and convex mirrors.

Another method is all the players trying to contain the threat or object of
some sort. Maybe in one game play style you are trying to escape, and in the
other the players are acting as the "bad guys" and are trying to trap AI
characters in the room (puzzle). This keeps the focus always on solving the
puzzle to progress in unlocking tiles, but allows for both sides of the story
to be played.

There could be different tile sets in terms of tools depending on which side
you are on, but otherwise the game plays the same.

Remy's Thoughts
===============

3x3 sudoku style grid

1 Player
2 Player
4 Player Max

Lobby
    Auto-Grouping
    Request Grouping

Overlay for messages/text

Leaderboard
    Least # of Tiles/Turns
    Most Levels
    Fastest(?)

I love the Indiana Jones-esque theme. Making Temple/Ruin tiles will be fun.

Resources
=========


Beam Engine
-----------

     ::
        <!DOCTYPE html>
        <html>
        <body>

        <canvas id="myCanvas" width="200" height="100" style="border:3px solid #c3c3c3;">
        Your browser does not support the canvas element.
        </canvas>

        <script type="text/javascript">

        var c=document.getElementById("myCanvas");
        var ctx=c.getContext("2d");
        ctx.globalAlpha=0.1;
        ctx.lineJoin='bevel';
        ctx.lineWidth=10;
        ctx.moveTo(10,10);
        ctx.lineTo(150,50);
        ctx.lineTo(10,50);
        ctx.stroke();

        </script>

        </body>
        </html>
        </code>

Overlay
-------

     ::

     <html>
     <head>
     <script type=”application/x-javascript”>
     function draw() {
     var canvas = document.getElementById(“canvas”);
     if (canvas.getContext) {
     var ctx = canvas.getContext(“2d”);

     ctx.fillStyle = “rgb(40,0,0)”;
     ctx.fillRect (20, 20, 65, 60);

     ctx.fillStyle = “rgba(0, 0, 160, 0.5)”;
     ctx.fillRect (40, 40, 65, 60);
     }
     }
     </script>
     </head>
     <body onLoad=”draw();”>
     <canvas id=”canvas” width=”150″ height=”150″></canvas>
     </body>
     </html>

Canvas Stack
------------

    http://arc.id.au/CanvasLayers.html
