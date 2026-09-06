cmake_minimum_required(VERSION 4.3)
project(disassembler)

set(CMAKE_CXX_STANDARD 20)

add_executable(disassembler main.cpp
        src/elf/ELF.cpp
        src/elf/ELF.h
        src/macho/MachO.cpp
        src/macho/MachO.h
        src/low_level/Binary.cpp
        src/low_level/Binary.h
        src/low_level/Disassembly.cpp
        src/low_level/Disassembly.h
        src/low_level/Patcher.cpp
        src/low_level/Patcher.h
        src/display/PatchDialog.cpp
        src/display/PatchDialog.h
        src/display/MainWindow.cpp
        src/display/MainWindow.h
        src/util/format.h
        src/util/binary_types.h)
