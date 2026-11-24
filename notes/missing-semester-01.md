# Missing Semester 01 — Course overview + the shell (2026-11-23)

## My notes (written from memory)

BASH IS called born again shell its a way for users to access advanced low level functions or programs or whatever doesnt necessarly
have a GUI for it .
we have programms , programs are known to the system because he looks up the name trougth the path which is an ENV variable
we learned about all different programs and cmds
like cd to move , mkdir to make directory , ls to view , pwd for present directory , date for date , cat for reading file , echo to print
sudo to do as super user , xdg -open to open file using the correct program
we learned about the < > operators , these will take the output of a program and feed it into a file , the direction of the feed matters
we also learned about piping which takes the output and puts it to another program . so that we can have a chain reaction
the sys directory has files that are part of the kernel , they can act on hardware directly , liek brightness , led , sound etc
you can link that to other programs to have some pretty cool stuff going on
we can cp a file to copy using source and target dir
we can move or rename a file using the mv cmd
we can look at permission for a file  read r , write w , execute x .
same for directory , read to see whats inside , write to add or remove , exectue to exectue any subfile
man is the manual for that function or whatever
-help also explains it mroe
all files are from the root /
the dollar sign is for regular users # is for root

## Corrections from review

- Bash = **Bourne Again SHell**, a pun on the older Bourne shell (`sh`) it replaced.
- `>` sends a program's output **into a file** (overwrites); `>>` **appends**; `<` feeds a file **into a program** as its input.
  Example: `sort < names.txt > sorted.txt`.
- Directory `x` permission means you can **enter/traverse** it (`cd` into it, reach files inside by path) — not "execute subfiles".
  Directory `r` lists names; `w` lets you create, delete or rename entries.
- `/sys` is a **virtual filesystem**: files the kernel generates on the fly to expose devices and kernel settings. Writing usually needs root.
  In WSL many hardware entries (like backlight) don't exist, because WSL has no real screen hardware.
- The help flag is `--help` (two dashes), e.g. `ls --help`. `man ls` is the full manual.
- `xdg-open` (no space) opens a file with its default app; in WSL use `explorer.exe .` or `wslview` instead.
- Permissions are shown in `ls -l` as three groups: owner, group, others, e.g. `-rwxr-x---`.
