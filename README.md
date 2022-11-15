# Showdown-BDSP-Converter
Converts a base copy of Pokemon BDSP's masterdatas into a more readable and editable Pokemon Showdown Format.
Download the latest release [here](https://github.com/Aldo796/Showdown-BDSP-Converter/releases)

## Formatting
Pokemon Showdown Format (Which is the format they use to import and export pokemon) can be easily acquired by:
- going to the [Pokemon Showdown Teambuilder](https://play.pokemonshowdown.com/teambuilder)
- creating a team that support BDSP (don't use illegal moves, don't use gen5+ pokemon)
- pressing the import/export button right next to the same

### You should end up with something that looks like:
- Garchomp (F) @ Yache Berry
- Ability: Rough Skin
- Level: 78
- EVs: 52 HP / 252 Atk / 204 Spe 
- Jolly Nature
- IVs: 0 SpA 
- \- Dragon Claw
- \- Earthquake
- \- Swords Dance
- \- Poison Jab

(That's Cynthia's Garchomp as an example)

## Use
To use the converter, first you have to have a dumped version of either Pokemon Brilliant Diamond or Shining Pearl.
The file that contains the trainers is called 'masterdatas' and is located in the Dpr folder in a dump
Once that's acquired
- Put masterdatas in the same folder as extract.exe, then run extract.exe
- Once finished it should create three folders, TrainerType, TrainerData, and TrainerPoke, ignore the first two as TrainerPoke contains the actual trainer pokemon data
- After opening TrainerPoke you should see text files named 1-705.txt, each one corresponds to a trainer in the game listed [here](https://docs.google.com/spreadsheets/d/17scGmh9vqeCGClY6ZBdY3mHlT3pfacRigc2mmfgDHwg/edit?usp=sharing)
- For each trainer that you want to change, open the file and replace whatever is in it with your new team (instructions for generating a team listed up above)
- After editing all the trainers you want to edit, run repack.exe to generate a file called "masterdatasEDITED" this file contains all your edited trainers

**Do Not** Edit these files by hand, moves are very strictly typed, and most likely will break if edited by hand, all pokemon data should be autogenerated to ensure the data gets imported

## Other Files
Other included .exes in this toolkit are Verify.exe and MaxAI.exe
- Verify.exe Verifies that all changes were done correctly, usually these mistakes will be caught in Repack.exe but it's there in case you need to check if it works
- MaxAI.exe is used to maximize the AI of all trainers so it doesn't need to be done by hand. This program will only work if "masterdatasEDITED" has already been generated and generated a new file called "masterdatasMAXAI"

## Notes
Genders are imported and exported wrong sometimes
As of now, the exporter and importer do not take into account for added trainers, so if in the future they figure out how to add more trainers to BDSP, this tool will not work until updated
