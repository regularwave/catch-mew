# catch-mew
Generates a save file for Japanese Pokémon Emerald that has the Old Sea Map Faraway Island event active.

**TID/SID generation:** 
Not all TID/SID pairs are valid because of the way Emerald generates them. Clicking the *Randomize IDs* or *Generate Save* button with both ID fields blank attempts to generate a TID/SID pair by modeling the ID relationship on the method the game uses. You can override this behavior by manually entering a TID/SID pair or providing a save file from which the pair can be imported.

## Usage
### If you just want a save that you can use to catch Mew:
1. Enter a trainer name
2. Set the trainer gender
3. Leave both ID fields blank, or click *Randomize IDs* to preview a new pair
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

### Trainer names
The preview shows how the trainer name will be rendered in game. Trainer names are limited to five characters *after* encoding and normalization. While leading, internal, and trailing spaces are preserved, a name cannot consist entirely of spaces. ASCII letters, digits, spaces, and `! ? . / :` become their fullwidth equivalents. Dashes (`-` and `−`) are converted to the Japanese long-vowel mark `ー`. The `‥` and `⋯` characters are converted to `…`. Halfwidth kana and combining dakuten/handakuten are normalized where a matching game character exists.

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
* [**Emerald decomp**](https://github.com/pret/pokeemerald) more details about save files and TID/SID generation