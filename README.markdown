# Recommended Items INI Packages for League of Legends
With Patch V1.0.0.124 of League of Legends, you can change the recommended items for each of your Champions, for 3 different game modes (Classic, Dominion, and Proving Grounds (ARAM).
Please note that this way of changing the UI is not officially supported by Riot and does not guarantee support if something fails.

This repository will contain **my** _recommended items_ for League of Legends champions as I play with them.
The INI files are built per instructions of http://leagueoflegends.wikia.com/wiki/Recommended_item_code with my own additions such as comments showing the statistics of each item, as well as total costs.
Manually adding these should help with seeing if any stats are missing for a character build.

## Usage Instructions
### Installation
Find the directory where you've installed League of Legends (for instance **`G:\Games\League of Legends\`** ) and go down to the **`RADS\solutions\lol_game_client_sln\releases\VERSION.NUMBER\deploy\DATA`** directory and clone this repository there as 'Characters'.<br />
Let's say the _VERSION.NUMBER_ is 0.0.0.174, you could use the following command prompt commands (assuming you have installed Git):
```
$ cd G:\Games\League of Legends\RADS\solutions\lol_game_client_sln\releases\0.0.0.174\deploy\DATA
$ git clone git://github.com/FiXato/LeagueOfLegendsRecItems.git Characters
```
**The VERSION.NUMBER folder may change its name every time the client is patched.**

### Creating your own files
**To create a custom recommended item list for a champion you need three things:**

1. The name of the Champion (as inside the `Disp_name` column of the champion list) _(leaving out any spaces and punctuation, e.g. ChoGoth)_
2. The game mode _(Classic, Dominion, ARAM)_
3. The ID numbers of the items in the game _(see http://leagueoflegends.wikia.com/wiki/Recommended_item_code)_

**Create a text file for your builds, in a directory named after your champion _(see point 1)_ and name it:**

1. `RecItemsCLASSIC.ini` - For Classic League of Legends _(Summoner's Rift and Twisted Treeline)_
2. `RecItemsODIN.ini` - For Dominion _(Crystal Scar)_
3. `RecItemsARAM.ini` - For the Proving Grounds _(which basically is an All Random All Mid)_

Each file should have at least a single block as follows:

```
[ItemSet1]
SetName=Set1
RecItem1=1028
RecItem2=3111
RecItem3=3044
RecItem4=3116
RecItem5=3124
RecItem6=3100
```

See the files included in this project for a more extensive format as examples.

## Contribute
Please don't comment on how the selected items suck; just fork the project if you think you can do better. ;-)