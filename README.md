# ghidra-gekko-broadway-lang
Language definition for the Gekko and Broadway CPU variant used in the Nintendo GameCube and Nintendo Wii respectively.

Currently, only the disassembly of the paired singles instructions work as the semantics aren't defined.

# Installation

Copy all the files from the `data/languages` folder to `Ghidra/Processors/PowerPC/data/languages` of your Ghidra installation. To use the language, select it in the language selection menu which is PowerPC 32 bit big endian Gekko/Broadway variant. Upon using the language, the .sla file should be compiled automatically.
