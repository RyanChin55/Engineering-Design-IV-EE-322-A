# Engineering-Design-VI-CPE-322-A
Lab 1 - GHDL and GTKWave
![215637050-99fff18b-db58-4818-96e1-9f6105d51d07](https://user-images.githubusercontent.com/98351372/236329742-a78acd64-a226-4075-8399-215501ab1de5.jpg)
![215637314-429526d2-4dd4-4ef8-bcc6-df8d55c6983e](https://user-images.githubusercontent.com/98351372/236329770-0846ec9e-43f4-48e6-8c84-b37f7f037b57.jpg)
![215922535-51b057cb-b620-4328-a0d8-d7ac483074b9](https://user-images.githubusercontent.com/98351372/236329787-35f6bf79-2892-4d36-a3cd-b504d3c0e614.jpg)

Lab 2: Command Line

env
```auto
PWD=/home/ryanc
COLORTERM=truecolor
DEBUGINFOD_URLS=https://debuginfod.archlinux.org 
XDG_SESSION_ID=1
ALACRITTY_SOCKET=/run/user/1000/Alacritty-wayland-1-31289.sock
XDG_DATA_DIRS=/home/ryanc/.local/share/flatpak/exports/share:/var/lib/flatpak/exports/share:/home/ryanc/.local/share/flatpak/exports/share:/var/lib/flatpak/exports/share:/home/ryanc/.local/share/flatpak/exports/share:/var/lib/flatpak/exports/share:/home/ryanc/.local/share/flatpak/exports/share:/var/lib/flatpak/exports/share:/usr/local/share:/usr/share
XDG_VTNR=1
I3SOCK=/run/user/1000/sway-ipc.1000.956.sock
TERM_PROGRAM=tmux
XDG_SEAT_PATH=/org/freedesktop/DisplayManager/Seat0
MOZ_ENABLE_WAYLAND=1
SWAYSOCK=/run/user/1000/sway-ipc.1000.956.sock
ZK_NOTEBOOK_DIR=/home/ryanc/Documents/zk/
LOGNAME=ryanc
EDITOR=nvim
XCURSOR_THEME=Qogir-dark
XDG_CURRENT_DESKTOP=sway
XDG_SESSION_DESKTOP=
WLR_RENDERER_ALLOW_SOFTWARE=1
OMNETPP_TKENV_DIR=/opt/omnetpp/src/tkenv
XDG_SESSION_PATH=/org/freedesktop/DisplayManager/Session0
TMUX_PANE=%2
SHLVL=3
STARSHIP_SESSION_KEY=2663619447823618
TMUX=/tmp/tmux-1000/default,31377,0
ALACRITTY_LOG=/tmp/Alacritty-31289.log
WAYLAND_DISPLAY=wayland-1
TERM=alacritty
XDG_SEAT=seat0
TERM_PROGRAM_VERSION=3.3a
STARSHIP_SHELL=fish
USER=ryanc
PATH=/home/ryanc/.local/share/nvim/mason/bin:/home/ryanc/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/bin:/var/lib/flatpak/exports/bin:/usr/lib/jvm/default/bin:/opt/omnetpp/bin:/usr/bin/site_perl:/usr/bin/vendor_perl:/usr/bin/core_perl
XDG_SESSION_TYPE=wayland
XDG_ACTIVATION_TOKEN=ac481531b372b9ad55f9ff95ebb55899
XDG_SESSION_CLASS=user
WINDOWID=94533639563376
XDG_RUNTIME_DIR=/run/user/1000
TMUX_PLUGIN_MANAGER_PATH=/home/ryanc/.config/tmux/plugins/
LC_MEASUREMENT=en_US.UTF-8
SHELL=/usr/bin/fish
QT_QPA_PLATFORM=wayland;xcb
OMNETPP_IMAGE_PATH=/opt/omnetpp/images
LC_NUMERIC=en_US.UTF-8
LC_NAME=en_US.UTF-8
MOTD_SHOWN=pam
LC_TIME=en_US.UTF-8
DISPLAY=:1
MAIL=/var/spool/mail/ryanc
LC_TELEPHONE=en_US.UTF-8
LC_ADDRESS=en_US.UTF-8
LC_PAPER=en_US.UTF-8
LC_MONETARY=en_US.UTF-8
LC_IDENTIFICATION=en_US.UTF-8
LANG=en_US.UTF-8
ALACRITTY_WINDOW_ID=94533639563376
WLR_NO_HARDWARE_CURSORS=1
HOME=/home/ryanc
XCURSOR_SIZE=24
DESKTOP_SESSION=sway
DBUS_SESSION_BUS_ADDRESS=unix:path=/run/user/1000/bus
BROWSER=qutebrowser
```
ps
```auto
  PID TTY          TIME CMD
56960 pts/2    00:00:01 fish
69193 pts/2    00:00:00 ps
```

pwd
```auto
/home/ryanc
```

git clone <remote_repo_url>
```auto
Cloning into 'iot'...
remote: Enumerating objects: 17485, done.
remote: Counting objects: 100% (199/199), done.
remote: Compressing objects: 100% (81/81), done.
remote: Total 17485 (delta 91), reused 174 (delta 80), pack-reused 17286
Receiving objects: 100% (17485/17485), 27.37 MiB | 13.86 MiB/s, done.
Resolving deltas: 100% (11822/11822), done.
```

ls
```auto
apps
cases
economics
hype
lesson1
lesson10
lesson2
lesson3
lesson4
lesson5
lesson6
lesson7
lesson8
lesson9
projects
README.md
special_problems
standards
tools
```

df
```auto
Filesystem     1K-blocks     Used Available Use% Mounted on
devtmpfs            4096        0      4096   0% /dev
tmpfs            8076028   499756   7576272   7% /dev/shm
tmpfs            3230412     3652   3226760   1% /run
/dev/dm-0      999170768 39151560 958271976   4% /
/dev/dm-0      999170768 39151560 958271976   4% /home
tmpfs            8076028    24596   8051432   1% /tmp
/dev/dm-0      999170768 39151560 958271976   4% /var/cache
/dev/dm-0      999170768 39151560 958271976   4% /var/log
/dev/nvme0n1p1   1021984   194312    827672  20% /efi
tmpfs            1615204       56   1615148   1% /run/user/1000
```
mkdir <folder> : Makes an empty folder at the path specified
nano <file> : Invokes the nano text editor on the file given. If the file doesn't exist it will be created when the user saves the file
cat <files...> : Concatenate files and prints them to the standard output
cp <file1> <file2> : Copy files from one location to another (can also copy directories)
mv <file1> <file2> : Move files from one location to another (can also copy directories)
rm <files...> : Remove files or directories
clear : Clears the terminal's screen, as well as its scroll back buffer, if applicable

man : Opens the system manuals for the given program
```auto
UNAME(1)                                                                                   User Commands                                                                                   UNAME(1)

NAME
       uname - print system information

SYNOPSIS
       uname [OPTION]...

DESCRIPTION
       Print certain system information.  With no OPTION, same as -s.

       -a, --all
              print all information, in the following order, except omit -p and -i if unknown:

       -s, --kernel-name
              print the kernel name

       -n, --nodename
              print the network node hostname

       -r, --kernel-release
              print the kernel release

       -v, --kernel-version
              print the kernel version

       -m, --machine
              print the machine hardware name

       -p, --processor
              print the processor type (non-portable)

       -i, --hardware-platform
              print the hardware platform (non-portable)

       -o, --operating-system
              print the operating system

       --help display this help and exit

       --version
              output version information and exit

AUTHOR
       Written by David MacKenzie.

REPORTING BUGS
       GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
       Report any translation bugs to <https://translationproject.org/team/>

COPYRIGHT
       Copyright © 2022 Free Software Foundation, Inc.  License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>.
       This is free software: you are free to change and redistribute it.  There is NO WARRANTY, to the extent permitted by law.

SEE ALSO
       arch(1), uname(2)

       Full documentation <https://www.gnu.org/software/coreutils/uname>
       or available locally via: info '(coreutils) uname invocation'

GNU coreutils 9.1                                                                          November 2022                                                                                   UNAME(1)
```
