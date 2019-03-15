# ghidra-gekko-broadway-lang
Language definition for the Gekko and Broadway CPU variant used in the Nintendo GameCube and Nintendo Wii respectively.

Supports the disassembly and decompilation of the paired singles instructions and the dcbz_l instruction.

For quantizations, two new PCode operations are defined like so:

    quantize(PS, type, scale)
    dequantize(EA, type, scale)

Where PS is a ps register, EA is the effective address of the load, type is the GQR type setting (4 = U8, 5 = U16, 6 = S8 and 7 = S16) and scale is the GQR scale setting. For clean decompilation output, consider setting the GQR values so it can properly assume their contents as most games will set them without changing them after.

# Installation

Copy all the files from the `data/languages` folder to `Ghidra/Processors/PowerPC/data/languages` of your Ghidra installation. To use the language, select it in the language selection menu which is PowerPC 32 bit big endian Gekko/Broadway variant. Upon using the language, the .sla file should be compiled automatically.
