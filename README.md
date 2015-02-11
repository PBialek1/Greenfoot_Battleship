# Greenfoot_Battleship
//worldGen

//establish char array for the grid, fill it with 'e' for empty
char[] grid = new char[10][10];
for (int row=0; row<10; row++){
    for (int column=0; column<10; column++){
        grid[row][column]== 'e';
  }
}
//placement of ships

//firing/hit registration
greenfoot.ask("Input firing code")
/* values for char array:
    e empty
    h hit
    m miss
    c carrier
    b battleship
    d destroyer
    s submarine
    p patrol boat
*/
