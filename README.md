# Instructions for playing on the Minecraft Server:

1. Install Minecraft normally.
2. Play Game and get to the title screen; exit game.
3. Run the 'forge-xxx-universal.jar' in this folder and install as Client.
4. Once done, press WINDOWS KEY + R, type '%APPDATA%', hit ENTER, open the '.minecraft' folder.
5. Within this folder, copy the files from the 'mods' and 'config' folder respectively the .minecraft folder.
6. Go back and open the Minecraft.exe.
7. Click 'Edit Profile' on the bottom right.
8. Change 'Use Version' to 'release 1.7.10-Forge...' (should be at the very bottom).
9. For the JVM Argument, copy and paste the following `-Xmx4G -XX:+UseConcMarkSweepGC -XX:+CMSIncrementalMode -XX:-UseAdaptiveSizePolicy -Xmn128M`
  * If you are having performance issues, change the -Xmx4G to -Xmx3G.
10. Click 'Save Profile' and click 'Play Game'.
11. Be patient because Java is stupid.
12. Multiplayer > Add Server > Add 'aeternum.ddns.net' as the address.
13. Enjoy!

If you read down to here and think the text instruction is too confusing, please consult the zip with images of these instructions.

## Easily update mods and config when changes are made

Create symlinks

* `ln -s path-to-repo/mods path-to-mc-folder/mods`
* `ln -s path-to-repo/config path-to-mc-folder/config`

Now you can just use `git pull` to get your mods and config up-to-date.
