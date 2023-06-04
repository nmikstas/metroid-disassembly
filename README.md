# metroid_disassembly

Disassembly of the NES version of Metroid. This started off as a disassembly of the game engine by Kent Hansen many years ago.
This is an attempt to improve the old disassembly I started over a decade ago. That disassembly is a mess!
There is a total of 8 banks in Metroid. Each bank is 16Kb in size.
Bank00 through Bank06 are swapped out in lower memory while Bank07 stays in upper memory.

## Folder Structure

* Completion_Map - Contains a .png file showing a visual representation of how much of the disassembly is complete.
* Ophis - The Ophis assembler.
* Output_Files - When the build script is run, the assembled output files are placed here.
* Source_Files - The disassembled Metroid files.

## Bank Descriptions

* Bank00 - Intro/End Game
* Bank01 - Brinstar
* Bank02 - Norfair
* Bank03 - Tourian
* Bank04 - Kraid Hideout
* Bank05 - Ridley Hideout
* Bank06 - Graphics
* Bank07 - Game Engine

## Assembling the Code

Running the build_script from the main directory will assemble the 8 bank files and create 8 binary files in the Output_Files directory.
An md5sum will also be calculated on the output binaries and compared to the md5sum of the original binaries.
