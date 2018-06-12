# lispi

lisp-based baremetal os for raspberry pi zero

## Aims for the project.

Simple Codebase... 

Minimal C interpreter with as much of the OS functionality written in Lisp.

< 100 lines per file 

Environment is a hash table / dictionary equivalent to  Dictionary<String, IntPtr>

All Lists are simple unidirectional lists

Each position in List is a Typed cons pairs (Object . PointToNext)
Primitive data types are:
Symbol (32-bit Ptr To First character)
List (32-bit Ptr to first element in Cons Pair List)
Integer (32-Bit Int)
float (32-Bit)
String (32-Bit Ptr To First Character)
Object (32-Bit)


### A bare metal USB & Screen driver for Raspberry Pi
[A bare metal USB driver for Raspberry Pi written in C - https://github.com/rsta2/uspi](https://github.com/rsta2/uspi)

### SD Card Access
https://github.com/jncronin/rpi-boot

### Fat32 - Overview
[Understanding FAT32 Filesystems - https://www.pjrc.com/tech/8051/ide/fat32.html](https://www.pjrc.com/tech/8051/ide/fat32.html)

### Fat32 - Library
[FAT16/32 File System Library - http://ultra-embedded.com/fat_filelib/](http://ultra-embedded.com/fat_filelib/)

Hopefully, use Fat32 library to read either SD card or USB Drives
