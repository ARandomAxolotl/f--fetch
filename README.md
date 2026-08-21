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

- date, to get uptime on Darwin and current date

- timedatectl, to get local time and timezone

- pwd, to get the absolute path of the directory containing the script

## Usage : 

./f--fetch : print the pretty fetch

--verbose : print the fetch with logs and errors

--gen-config [path] : create default config, will create a file called `config` at the directory the script is currently inside or override [path] if provided

-c [config] : use config at [config]

> Note : `--gen-config` and `-c` can be combined with `--verbose` with `--verbose` as the first argument

## Customization : 

Edit the main() function in the script or put your config at `~/.config/f--fetch/f--fetch`, `[the directory that contains the script]/config` or use `-c`

### Configuration : 

WARNING : the config will be **executed as shell code**

> it can execute stuff

It's just like editing main()

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

<!-- CrrMoonPhrase -->

<sup><sub> Please dont be genderism Mizuki is very tuff </sub></sup>
