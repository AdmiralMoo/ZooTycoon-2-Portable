# ZooTycoon-2-Portable
A batch file that allows you to run Zoo Tycoon 2 from an external drive by automatically transferring your saves back and fourth from your drive to the appdata folder.

I made this for an undisclosed person who asked about how to do this on Discord.

HOW TO SET UP:

1. Copy your Zoo Tycoon 2 folder from "C:\Program Files (x86)\Microsoft Games\" (or wherever its installed) to the external drive you want to run it off of.
2. In the Zoo Tycoon 2 folder that is now located on your external drive, paste the batch file you just downloaded.
3. Create a folder within "Zoo Tycoon 2" called "PROFILES"
4. Navigate to "%appdata%\Microsoft Games\Zoo Tycoon 2\" and copy the profile(s) you want to use in your portable installation to the "PROFILES" folder.
5. Run the batch file and play!

HOW IT WORKS:
The batch file copies the directories and files within the "PROFILES" folder that you created in the folder your portable Zoo Tycoon 2 installation to where Zoo Tycoon 2 looks for savegames in %appdata%. The whole point of this batch file is to save yourself the trouble of copying the savegames from your drive to the appdata folder, which is a pain to access.

After it copies the files, it will run Zoo Tycoon 2 from the portable installation, which is in the same location as the batch file.

Finally, when you close the game, it will copy the savegames from appdata back to the PROFILES folder and delete the files it copied over originally in appdata, leaving no trace it was ever there.

NOTES:
This is a messy solution to the problem. Batch can't handle long file names and its been that way since DOS, so profiles longer than 6 (or so) characters will be cut off. For example, Default Profile will become DEFAUL~1. To prevent this, just create a profile thats shorter than six characters to avoid duplicates and complications.
Also, Zoo Tycoon 2 will boot to Default Profile, so you'll have to select the portable profile from the top of the main menu when you start the game.

CONCLUSION:
Like I said, this is a pretty messy solution and I'm not sure if it will work every time. If theres any problems, I'll try my best to fix this the best I can.
