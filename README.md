# Greenfoot_Battleship
Worldgen
pic of grid
grid 12x12 We can do this easily with a matrices
Look at this if confused
Declared as columns or rows
array[] []/list? : sea ship hit miss
objects : ships, shots(hit/miss)
Placement
destroyer 3x1 or 1x3, sub 3x1 or 1x3, carrier 5x1 or 1x5, battleship 4x1 or 1x4, patrol boat 2x1 or 1x2
state ship type, input endpt1 and endpt2 or endpt1 and direction
checks that pts are in line and proper ship length
checks all pts in ship are empty
creates ship object, fills array/list elements with ship type
random placement option
Objects
ship (type, length, player1/player2 (i.e. hidden or not), hits, sunk bool)
sea (sea, miss, hidden ship, hit ship)
firing
array check or collision detection?
short delay
notify player when ship sunk
AI
search  mode
pseudo random search pattern

attack mode
check surrounding spots
follows ships until destroyed
Objects
ship (type, length, player1/player2 (i.e. hidden or not), hits, sunk bool)
sea (sea, miss, hidden ship, hit ship)
Misc
animations (explosions, sinking)
sounds (hit, firing, explosion, sinking, victory, loss)
images 
generic ship square or image for each ship?





Notes
What we need to decide right away is whether we want to utilize an array/list or if we want to rely on object collision. I’m inclined to go with the array route because I think it will be easier, especially with the hidden ships, and it will be more reliable. However we may want to go with collisions to better fit the requirements. We could easily satisfy the checkCollision() requirement with placement.


Do we want to have ship objects in the world. We definitely want them but I think they should just be in the background to be used for placement and to determine when a ship is sunk. Actually placing ships in the world would be a pain, we could just create one square object in each space in the grid which would just change image depending on what is in that square.

I think we rely on object collision. The array list thing, while being easier, doesn’t help us with the rubric at all. And as for the ships as an object, that is what I was planning on but I guess I am open to anything, but we do need to have at least three kinds of objects according to the rubric

The rubric says we need to use checkCollision at least once. We will use it for the placement of ships to make sure none of them overlap. So we can still use the array. Even if we use object collision I still feel like a list could be useful. Let’s start programming and see what we think as we work on it.

Ok
