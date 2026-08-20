# f--fetch

> a minimal shell script that assumes the userspace is stupid

## Supported environments :

- Linux

- Darwin (macOS/iOS)

- Windows (Git Bash/MSYS/Cygwin)

- probably your toaster

## Tested environments : 

- Arch Linux

- My router that has 22MiB of RAM

- My jailbroken iPhone 8 plus

- Git bash

- Windows Recovery Environment (if you can locate and run `git bash`/`mingw64`)

- Archiso (`pacman -Sy git` first)

- iSH on the same iPhone 8 plus

- Android (BlissOS x86) with termux

## Installation : 

Download the script

Run it (`chmod +x` if required)

Move to directory that's in PATH if you want to (like `~/.local/bin`)

## Dependencies : 

### All : 

- A POSIX-compatible shell

### Linux/Windows(git bash/mingw64)/Android : 

- nothing

### Darwin (iOS/macOS) : 

- sysctl must be in PATH

### Optional :

- uname, to distinguish kernels

- awk, to parse /proc and other stuff

- basename, to pretty the shell name

- playerctl, to get music data

- wc, to count packages

- tty, to print tty information

- od, to get 32 bytes from /dev/random

- curl, to fetch artwork

- chafa, to render artwork

- lspci, to get gpu name 

- grep, sed, to parse lspci for gpu name

- date, to get uptime on Darwin

- timedatectl, to get local time and timezone

## Usage : 

./f--fetch : print the pretty fetch

./f--fetch --verbose : print the fetch with logs and errors

## Customization : 

Edit the main() function in the script

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

### Logo customization

`LogoLongestLine=x`

Sets the logo width.

`LogoFromArtwork=1|0`

Enables or disables using music artwork as the logo.

<!-- Hidden modules -->

<!-- AkiyamaMizukiIsTuff -->

<!-- NightcordMembers -->

<!-- TransFlag -->

<!-- CheeseCakeFight -->
