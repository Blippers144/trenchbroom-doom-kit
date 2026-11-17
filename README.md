TrenchBroom for Doom II map making for those who prefer TB over Ultimate Doom Builder or Slade.

TrenchBroom Doom Kit (Download is in releases)



WAIT! Before you download trenchbroom-doom-kit.zip, make sure you have these ready:



1. A copy of DOOM2.WAD (Not DOOM.WAD)

2. TrenchBroom: https://github.com/TrenchBroom/TrenchBroom/releases

3. UZDoom: https://github.com/UZDoom/uzdoom

4. Node.js: https://nodejs.org/en/download



------------------------------------------------------------



Setup



Unzip the kit somewhere permanent and double-click Install.cmd.



- Runs 100% offline on your PC. Needs no internet connection, account, or external services.

- Works from whatever folder you unzip it into.



------------------------------------------------------------



How the Pieces Fit Together



- TrenchBroom is the map editor.

- UZDoom plays the compiled levels.

- DOOM2.WAD supplies the textures and monsters.

- Node.js runs the kit's JavaScript tools (the installer and the converter).



------------------------------------------------------------



What Does Node.js Do?



Node.js is a free program that runs JavaScript code on your PC outside of a web browser. Since Windows cannot run the kit's JavaScript files directly, Node.js handles them. It runs nothing in the background and only activates during setup or when you compile a map.



The kit uses Node.js for two jobs:



1. The installer (Install.cmd runs setup.js):

- Finds UZDoom and DOOM2.WAD.

- Reads DOOM2.WAD and saves its textures and monster/item pictures as image files that TrenchBroom can display.

- Adds "Doom" to TrenchBroom's game list, complete with all placeable entities and Compile options.



2. The converter (map2wad.js):

- Runs each time you press Compile in TrenchBroom (usually in well under a second).

- Reads your TrenchBroom map and calculates the Doom floors, ceilings, walls, slopes, and bridges.

- Writes a .wad file and launches UZDoom with it.

(Download is in releases)
