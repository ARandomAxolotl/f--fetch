# f--fetch

> a minimal shell script that assumes the userspace is stupid

## Tested environments : 

- Arch Linux

- My router that has 22MiB of RAM

- My jailbroken iPhone 8 plus

- Git bash

- Windows Recovery Environment (if you can locate and run `git bash`/`mingw64`)

- Archiso (`pacman -Sy git` first)

- iSH on the same iPhone 8 plus

## Installation : 

Download the script

Run it (`chmod +x` if required)

Move to directory that's in PATH if you want to (like `~/.local/bin`)

## Dependencies : 

### All : 

- A POSIX-compatible shell

### Linux/Windows(git bash/mingw64) : 

- nothing

### Darwin (iOS/macOS) : 

- sysctl must be in PATH

### Optional :

- uname, to distinguish kernels

- awk, to parse /proc and other stuff

- readlink, to distinguish init

- basename, to pretty the shell name and help distinguish init

- playerctl, to get music data

- wc, to count packages

- tty, to print tty information

## Customization : 

### Modules list : 

- Hostname

- OS

- Init

- Shell

- Pwd

- Terminal

- TTY

- Kernel

- Memory

- CPU

- Uptime

- Packages

- TimeDate

- Music

- Desktop

- Editor

- Visual

### Decoration modules list : 

- Line_break

- Break

- Prin

- Prin_no_endl

- Colors

<!-- Hidden modules -->

<!-- AkiyamaMizukiIsTuff -->

<!-- NightcordMembers -->
