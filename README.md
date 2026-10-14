# catch-mew
Generates a save file for Japanese Pokémon Emerald that has the Old Sea Map Faraway Island event active.

**TID/SID generation:** Not all TID/SID pairs are valid because of the way Emerald generates them. The *Generate IDs* button emulates the method the game uses, but you can override and use (potentially) invalid IDs by entering them yourself.

## Usage
### If you just want a save that you can use to catch Mew:
1. Enter a trainer name
2. Set the trainer gender
3. Click the *Randomize IDs* button
4. Click the *Generate Save* button

### If you have known trainer name, gender, TID, and SID you want to use:
1. Enter the known trainer name
2. Set the known trainer gender
3. Enter the known TID
4. Enter the known SID
5. Click the *Generate Save* button

### If you have an existing save file and want the same trainer name, gender, TID, and SID:
1. Click the *Load From Save* button
2. Select your current save file
 - 128 KiB save files in *.sav* or *.srm* format with or without a 16-byte RTC timestamp at the end of the save file. Save states are not supported.
3. Click the *Generate Save* button

### Save file format
The generated save file will have a *.sav* extension. If you need it to be *.srm* you can just rename the file extension.

## What to do next
### Travel to Faraway Island and catch Mew
1. Go to ミナモシティ (Minamo City, English: Lilycove City, between routes 121 and 124)
2. Go inside the harbor building (the most southwest building)
3. Talk to the NPC in front of the タイドリップ号 (Tiderip, English: SS Tidal)
4. After some dialog ハギ老人 (Old Man Hagi, English: Mr. Briney) will take you to Faraway Island
4. Walk through the trees and enter the encounter area, startling Mew
5. Chase Mew until you have it cornered and save before pressing A

## Acknowledgements (in no particular order)
* [**Project Pokemon**](https://projectpokemon.org) so much info
* [**PKHeX**](https://github.com/kwsch/pkhex) save file research
* [**PKHeXWC3Plugin**](https://github.com/Bl4ckSh4rk/PKHeXWC3Plugin) event injection research
* [**JS-Finder**](https://github.com/lincoln-lm/JS-Finder/) Emerald TID/SID research
* [**Bulbapedia**](https://bulbapedia.bulbagarden.net/) sprites, event research
* [**Emerald decomp**](https://github.com/pret/pokeemerald) more details about save files