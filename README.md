# Pier-Solar

Created for the two ridiculous "That's Slippery" and "Nerves of Steel" achievements.

Will be initially creating for the ChronuxMax on an Xbox One but feel free to commit a script for other platforms - be sure to include what peripheral you're using the script for.

[You can find the user manual/syntax here.](https://cronusmax.com/manual/gpc_guide.htm?ms=AgAAAAAAAAI%3D&st=MA%3D%3D&sct=MA%3D%3D&mw=MzIw#)

[You can find a tutorial here.](https://cronusmax.com/manual/a_simple_tutorial.htm)

I figured it would be best to create separate scripts for the two achievements to start off with. Once the two are working then they could just be merged I guess.


## Notes

Things I discovered whilst doing this; they're just for reference/backup.

 
The game map and all sprites are layed out in a square 'grid'. This script is to be run the moment you spawn in the map, and should finish you off infront of the NPC at the end of the map for you to press A and speak to. After which, you run the second script in order to make the journey back. This code should be set out so that the only buttons you should be pressing is Left Trigger to get to the end of the maz, and Right Trigger to go back to the beginning.

I also need to work out how much time there is to navigate across 1 block on the 'grid'. Your character can not stand/turn inbetween the 'squares' on the 'grid' both on land and whilst sliding, and so that amount of time needs to be measured. This will be trial and error, but once we figure out the measurement of "1", the rest will fall into place. I haven not yet determined if the sliding speed is the same as the walking speed on normal ground - this will be discovered in tests, when alternating between the very start of the map to the very start of sliding. Once discovering the timing of one block and how much time there needs to be between button presses.

Not sure if requed if the timing is correct, but I noticed when playing that the character will not turn whilst sliding unless the DPad button is held down when it is time to turn, meaning the DPad cannot be 'tapped' when required.

From my tests, it looks like navigating each sliding block is running at 250bpm, meaning each button input length must hold for 240ms.

I'm not sure what the limitations of the Chronus Max are, but due to the length of this script it might need things split up or condenseed....
