**Pongy**


Overview
================
You know what $Pong$ is. $Pongy$ is literally just $Pong$, except the paddles can move horizontally as well as vertically.
Plus, the direction you're moving affects the speed and trajectory of the ball when you hit it.

In $Pongy$, two players share the same keyboard and play together. Player 1 uses ESDF and Player 2 uses the Arrow Keys.
The first player to 10 points wins.


Running the Game
================
$Pongy$ is compiled for Windows and Linux. Download & extract 'em, and they should just run.


Gameplay
================
Horizontal motion wouldn't add a lot to $Pong$ if it didn't give you greater control over the ball's speed. 
If you're moving forward when you hit it, it will bounce back at a faster rate. If you're moving up or down, that will affect the ball's trajectory.

*!!! tip: Growing Intensity*
    There is no limit to how fast the ball can go, so it can go faster and faster as the round drags on. 
    This prevents the game from stagnating - even expert players can have quick, intense bouts.

After every goal, the location and speed of the paddles and ball are reset. 
After this reset, the ball will always be headed directly towards the paddle of the player who just scored. 
This eases the disorientation from having your paddle teleport.

*!!! note: Gameplay Testing*
    Feedback compelled me to reset the position of the paddles after every point scored - originally, only the ball was reset.
    This caused problems, because sometimes the ball would spawn behind your paddle. This caused frustration from aggressive players.

*!!! tip: Tension Loop*
    Because of the reset after every goal, game has a built-in loop of tension, release. Tension, release.

*!!! tip: Precise Strategy*
    You're not just worried about hitting the ball, but about manipulating it. This encourages players to make strategic decisions and precise movements.


Menus
================
The game has two menus. The first is a title screen, with a `start game` button.

*!!! note: Menu Testing*
    User testing also revealed the importance of including a tutorial on the title screen.

The second is an end screen, which appears after one player scores 10 points and is declared the winner. It includes a `new game` button.
The end screen can also be triggered manually by using the escape key.

*!!! warning: No Pause Button*
    There is no way to pause a current game and resume it later.
    Ending the game early results in a draw.


Limitations
================

*!!! warning: ESDF vs. WASD*
    You may have noticed I used ESDF instead of WASD. The professor for my Game Engine Architecture class said, because of how keyboard keys are typically mapped, some inputs can be lost if there are two many at once.
    ESDF has this problem less often than WASD. This is important since Pongy requires two players to share a keyboard.
    However, ESDF can be confusing to some players. There is currently no way to remap those keys.

*!!! error: Bug*
    If you manage to hit the ball with the top or bottom of your paddle, the ball will sometimes drag your paddle along all the way into your own goal.
    I didn't prioritize fixing this. After all, if you've hit the ball with the top or bottom of your paddle, you've already missed it anyway. 
    This bug isn't making you lose any points you haven't already lost.

Credits
================

Pongy Created by: Cordell King.
Pong Original Creators: Allan Alcorn & Nolan Bushnell.
Pongy Art by: Juan Linietsky, Ariel Manzur and the Godot community.
Pongy Game Engine: Godot.
