# Geometry Dash VGA Project
 In this project we coded a multi-level game inspired by Geometry Dash in C. This game is intended to operate on the DE1-SoC FPGA with the ARM A9 Processor. 

 This project can be deconstructed into three main parts:

**Graphic Development:** To display a landscape in the background of the game, a digital drawing was created and then converted into a pixel array via an online software. We then created a function to index into this array and plot the appropriate colour for each pixel on the display. To create the objects in this game we developed to functions, one to draw a box at a given x and y co-ordinate and another to draw a triangle at a given x and y co-ordinate.

**Game Logic:** This game has three levels of difficulty, each corresponding to different speeds of motion. Within all three modes the objective is the same: to avoid collision with the oncoming obstacles. We implemented a process to check when the points on the box were equal to those of the spikes in order to check for collision. For each obstacle avoided, the players score increases.

**Input and Output Interfacing:** There were several inputs and outputs used in this game. The primary input was the PS/2 keyboard, which was used to quit the game at any point (by pressing the letter Q), and to make the obstacle jump (by pressing the spacebar). A polling procedure was used to check the input values. The HEX display was used to output the player's score and display the words 'GAME OVER' when the player crashed into an obstacle. The buttons on the display were used to select the difficulty of gameplay.

We were able to successfully demo this project on the DE1-SoC:

https://github.com/hannahlila04/geometry-dash-vga-project/assets/68185417/72c7c7c9-c8f3-4165-bbb3-3ff59563decb

