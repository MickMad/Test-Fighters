Test-Fighters 0.1.1a
=============
by MickMad

Controls:
WASD - move red player
G - punch red player
H - kick red player
SPACE -  jump red player

ARROWS - move blue player
R_ALT - punch blue player
R_CONTROL - kick blue player
R_SHIFT - jump blue player

Changes from 0.1:
-New graphics for player
-Added support for animated graphics
-Added KICK movement
-Fixed bug which would get the player off the bounding area if jumping near the bottom of the area
-Player's collision area will increase accordingly to the width of the current rendered frame

Changes from 0.1.1:
-Fix bug which would get the player not to jump correctly if near the top of the bounding 
-Adding a baseline between the player's feet which will stay under the player and not follow its direction if it's jumping, to be used for movement correctness checks and for drawing a shadow under the player
-Separate the collision area from the movement correctness checks
-Improve collision detection (control if player has hit during the entire animation, not only at the beginning)
-Delegate input checks to the Player class

Plans for future release:

-Use a data structure to keep the informations about the keys used by the player (define the keys at runtime, not at compile time, eg. to enable keys customization by the user via a menu)