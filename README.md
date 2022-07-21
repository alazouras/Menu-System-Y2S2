# Menu-System-Y2S2
Tutorial on how the main and pause menu systems were created for '3D Blocks...' (Year 2 Semester 2)

# 1) Menu Script
First, create your script (I named it MenuTime) and input these components:

![image](https://user-images.githubusercontent.com/91538155/180264928-4a4cde63-79cc-4eee-ac52-b22c26dc7477.png)

After establishing those, in Start we need to make sure the character and camera controllers are acknowledged, and everything in-game is reset to 0:

![image](https://user-images.githubusercontent.com/91538155/180265106-f2e8e6cb-1db5-4032-9106-6d61d07d88d0.png)

Then, all that's needed in update is an if statement to activate the pause menu in-game when the escape button is pressed:

![image](https://user-images.githubusercontent.com/91538155/180265224-45ff1d15-5651-457f-a381-3cd3f6a1712c.png)

Then, we need functions for each menu option; Start/Resume Game, Pause Game and Quit Game. For Quit, the function is short:

![image](https://user-images.githubusercontent.com/91538155/180265438-3eeb642f-5798-498b-824b-fd41413bd1e6.png)

Similarly, for Start/Load game, the void is one line:

![image](https://user-images.githubusercontent.com/91538155/180265499-094b163c-c539-4615-93ea-9cf82534a7a4.png)

Then, for Pause Game, we need to open with the following if statement:

![image](https://user-images.githubusercontent.com/91538155/180265599-dc8eb8ec-f8d8-4a64-bc81-d20b910c9ac0.png)

This if statement is for what happens if Pause is disabled (the game is not paused), so we need to make sure the character and camera controller work, the pause window is hidden and the mouse is invisible. This is done like so:

![image](https://user-images.githubusercontent.com/91538155/180265818-881dc056-c575-4678-a04c-bfa8ce44bf77.png)

Finally, you need an else statement for any other scenario, the only one in this case being if the game is paused. For this we need the opposite; to stop the character and camera from moving, enable the mouse and load the pause menu window, therefore the code is the same but flipped:

![image](https://user-images.githubusercontent.com/91538155/180266122-b9424550-4e57-440c-a047-50720a9127ed.png)


# That is all that is needed for the Menu System
