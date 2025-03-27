# ShantaeHero
A WIP matching decompilation of Shantae: Half Genie Hero

# Tasks
- Repository setup for objdiff
- Source layout
- Figure out how to include private third party libraries in the repo (FMOD, Steamworks, etc.)
- Decompilation

# ShantaeHero source tree
ShantaeHero is split up into 2 parts:
- `engine`, which contains all 3rd party libraries and WayForward's proprietary engine (`wfEngine`)
- `src`, which contains the source code of the game.

wfEngine uses 3 different C++ file formats, `.cpp`, `.h`, and `.inl`. Any inline function implementations in wfEngine must go in an appropriate `.inl` file.

However, `src` does not use `.inl` files. It only uses `.cpp` and `.h` files.

Refer to ShantaeHero.pdb for source info.