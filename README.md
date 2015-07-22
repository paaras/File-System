File System
=================

Overview
------------
In this project I wrote a file system driver for Linux.

Operating systems generally support many different file systems, from old-school FAT (common in DOS machines) to new formats such as Linux's ext3. Each file system type is written to fit a common interface, called the VFS layer. (File systems are often implemented using object oriented techniques.) To understand how a real VFS layer works I filled out a simple file system implementation. The file system module is loaded into the kernel which mounts the file system and allows access to the file system with usual Unix commands like cat. The file system driver stores its data in a built-in RAM disk.

This project implements the routines that handle:

* free block management
* changing file sizes
* read/write to the file
* reading a directory file
* deleting symbolic links
* creating files
* conditional symlinks.
