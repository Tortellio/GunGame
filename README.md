# Gun Game (Arms Race)
Gun Game (sometimes known as Arms Race) is a plugin for Unturned server based of Gun Game and Arms Race for Counter-Strike.

All players start with the same gun and get new guns every time they kill someone. The win the game,a player has to get to the last level (Knife Level) and kill a player, this is usually difficult because most other players will still have guns when the knife level player only has a knife. Players can also get the ‘Over Powered’ perk if they get a kill streak. This perk gives them max skills making them faster and more capable of killing other players. As a players kill streak increases, the time of ‘OP’ mode increases.

If a player gets killed with a knife, they will loose a level and the killer will gain a level.

### Configuration:
This plugin is designed to be run on its own server, it completely disables the normal Unturned survival game mode.

It is highly recommended that you configure the Unturned server with this config file. Put this file in the root of the server directory you have installed the Gun Game plugin on.

### Spawning:
You can set custom spawn points with the “/addspawn” command but you will have to enable custom spawns in the config. This will stop players from being randomly spawned in the map and will only spawn them at the specified locations.

If you do decide to use random spawns, you should enable the “/unsick” command to unstick players if they get stuck while respawning. You can set the cool down and delay for this command in the config file.

### Translation:
You can change any of the in-game text through the translation file in “Plugins/Gungame”. You can also change the color of any of the in-game text by replacing the HEX color code with your own. Here is a tool to find the hex codes of colors. If a translation entry has a color of “000000” by default, it is probably only shown in console so colors don’t apply.

### Map:
This server can run any map but you will have to configure the arena border to get the desired location of the game.

I do not recommend using this plugin with an arena map because they interfere with each other by clearing items deleting walls etc. This can cause bugs where players do not have any guns.

### Time between rounds:
There is a delay between when a player wins causing the round to end and when it starts again. This delay can be changed in the config file.

### Arena Border:
There is a border that keeps players inside the desired arena. The border can be changed to any size you like with the 4 co-ordinate parameters in the “GunGameConfig.xml” file in the directory of “Plugins/GunGame”.

The arena border will stop any players going out side even if there is no barricade in the way, this does not apply to players who are admin.

The arena walls are re-generated when you use “/reset” or any of the border configuration commands.

If you change the borders in the “GunGameConfig.xml” file while the servers are running, you will need to do “/rocket reload” and “/reset” for these changes to take effect. This also applies if the server is not running while you change the config except you do not need to do “/rocket reload”.

You can also change the barricade that the wall is made of and you can change the spacing in between the barricades.

If you do not want any spacing between the barricades you have to set the width and height to that of the barricade you are using

Small plate width: 2.0

Small plate height: 2.0

Large plate width: 3.75

Large plate height: 3.75

Not sure if these are 100% accurate, please notify me if you know what the real sizes are. I have not had enough time to guess and check for all the sizes.

### Note:
The North wall co-ordinate must be bigger than the South wall co-ordinate and the East wall co-ordinate must be bigger than the West wall co-ordinate.

 

### Gun List:
The gun list is randomly ordered from a list of Item ID’s in the “GunGameConfig.xml” file in the directory of “Plugins/GunGame”.

By default, the list of guns will be generated in a random order from the config file but you can set it to be non-random, this means that the guns will go in the order that you put them in the config every time. This can be useful if you want pistols at the start of the round, rifles in the middle etc..

You can add, remove or change guns as you wish. This plugin has not been tested with custom workshop or mod guns but I think it should work.

### Commands:
__/reset__ – resets the game and re-generates the list of guns

**/op** – gives you the ‘Over Powered’ status in game for 20 seconds.

**/lvlu** – increases your Gun Game level as if you had killed a player. This gives you the next gun in the list.

**/lvld** – decreases your Gun Game level as if you had been killed with a knife. This gives you the previous gun in the list.

**/unstick** – If a player gets stuck inside an object while respawning, they can use this command to get spawned again.

### Arena boundary commands:
**/northwall** (“/nw”) – Sets the co-ordinate for the north wall of the arena.

**/southwall** (“/sw”) – Sets the co-ordinate for the south wall of the arena.

**/eastwall** (“/ew”) – Sets the co-ordinate for the east wall of the arena.

**/westwall** (“/ww”) – Sets the co-ordinate for the west wall of the arena.

Custom spawn commands:
**/addspawn** (“/as”) – Adds a spawn point to the list of custom spawns.

**/deletespawn** (“/ds”) – Deletes a spawn point from the list of custom spawns.
