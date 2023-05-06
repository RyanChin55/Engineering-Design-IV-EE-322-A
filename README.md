# Engineering-Design-VI-CPE-322-A
# Lab 1 - GHDL and GTKWave
![215637050-99fff18b-db58-4818-96e1-9f6105d51d07](https://user-images.githubusercontent.com/98351372/236329742-a78acd64-a226-4075-8399-215501ab1de5.jpg)
![215637314-429526d2-4dd4-4ef8-bcc6-df8d55c6983e](https://user-images.githubusercontent.com/98351372/236329770-0846ec9e-43f4-48e6-8c84-b37f7f037b57.jpg)
![215922535-51b057cb-b620-4328-a0d8-d7ac483074b9](https://user-images.githubusercontent.com/98351372/236329787-35f6bf79-2892-4d36-a3cd-b504d3c0e614.jpg)

# Lab 2: Command Line

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
mkdir <folder> : 
```auto
Makes an empty folder at the path specified
```
nano <file> : 
```auto
Invokes the nano text editor on the file given. If the file doesn't exist it will be created when the user saves the file
```
cat <files...> : 
```auto
Concatenate files and prints them to the standard output
```
cp <file1> <file2> : 
```auto
Copy files from one location to another (can also copy directories)
```
mv <file1> <file2> : 
```auto
Move files from one location to another (can also copy directories)
```
rm <files...> : 
```auto
Remove files or directories
```
clear : 
```auto
Clears the terminal's screen, as well as its scroll back buffer, if applicable
```

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
       Written by Ryan Chin.

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

uname
```auto
Linux krypton 6.1.9-arch1-2 #1 SMP PREEMPT_DYNAMIC Fri, 03 Feb 2023 18:49:53 +0000 x86_64 GNU/Linux
```
  
ifconfig
```auto
enp0s31f6: flags=4099<UP,BROADCAST,MULTICAST>  mtu 1500
        ether f8:75:a4:35:c9:8a  txqueuelen 1000  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
        device interrupt 16  memory 0xea200000-ea220000  

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 8065  bytes 12805787 (12.2 MiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 8065  bytes 12805787 (12.2 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

wlan0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.0.118  netmask 255.255.255.0  broadcast 192.168.0.255
        inet6 fe80::cf56:78ff:4b11:bb0d  prefixlen 64  scopeid 0x20<link>
        ether 50:eb:71:c4:5c:25  txqueuelen 1000  (Ethernet)
        RX packets 282558  bytes 200078345 (190.8 MiB)
        RX errors 0  dropped 2  overruns 0  frame 0
        TX packets 65997  bytes 10034315 (9.5 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

ztc3q7w5bl: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 2800
        inet 172.24.233.60  netmask 255.255.0.0  broadcast 172.24.255.255
        inet6 fe80::84:9cff:fef7:9b55  prefixlen 64  scopeid 0x20<link>
        ether 02:84:9c:f7:9b:55  txqueuelen 1000  (Ethernet)
        RX packets 1240  bytes 678053 (662.1 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1279  bytes 98362 (96.0 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
```
ping <ip>
```auto
PING localhost(localhost (::1)) 56 data bytes
64 bytes from localhost (::1): icmp_seq=1 ttl=64 time=0.092 ms
64 bytes from localhost (::1): icmp_seq=2 ttl=64 time=0.099 ms
64 bytes from localhost (::1): icmp_seq=3 ttl=64 time=0.101 ms
64 bytes from localhost (::1): icmp_seq=4 ttl=64 time=0.101 ms
64 bytes from localhost (::1): icmp_seq=5 ttl=64 time=0.101 ms
64 bytes from localhost (::1): icmp_seq=6 ttl=64 time=0.097 ms
64 bytes from localhost (::1): icmp_seq=7 ttl=64 time=0.135 ms
64 bytes from localhost (::1): icmp_seq=8 ttl=64 time=0.101 ms
64 bytes from localhost (::1): icmp_seq=9 ttl=64 time=0.104 ms
64 bytes from localhost (::1): icmp_seq=10 ttl=64 time=0.102 ms
64 bytes from localhost (::1): icmp_seq=11 ttl=64 time=0.131 ms

--- localhost ping statistics ---
11 packets transmitted, 11 received, 0% packet loss, time 10129ms
rtt min/avg/max/mdev = 0.092/0.105/0.135/0.013 ms
```

netstat
```auto
Active Internet connections (w/o servers)
Proto Recv-Q Send-Q Local Address           Foreign Address         State      
tcp        0      0 krypton:51380           lga25s74-in-f14.1:https ESTABLISHED
udp        0      0 krypton:bootpc          _gateway:bootps         ESTABLISHED
Active UNIX domain sockets (w/o servers)
Proto RefCnt Flags       Type       State         I-Node   Path
unix  3      [ ]         STREAM     CONNECTED     34825    @/tmp/.X11-unix/X1
unix  3      [ ]         STREAM     CONNECTED     25098    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25809    
unix  3      [ ]         STREAM     CONNECTED     27687    
unix  3      [ ]         STREAM     CONNECTED     27686    
unix  3      [ ]         STREAM     CONNECTED     32119    
unix  3      [ ]         STREAM     CONNECTED     23048    
unix  3      [ ]         STREAM     CONNECTED     34176    
unix  3      [ ]         STREAM     CONNECTED     21194    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24972    
unix  3      [ ]         STREAM     CONNECTED     25094    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     20102    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     294485   
unix  3      [ ]         STREAM     CONNECTED     294481   
unix  3      [ ]         STREAM     CONNECTED     25137    
unix  3      [ ]         STREAM     CONNECTED     26730    
unix  3      [ ]         STREAM     CONNECTED     26731    /run/user/1000/at-spi/bus_1
unix  3      [ ]         STREAM     CONNECTED     18821    
unix  3      [ ]         STREAM     CONNECTED     26558    
unix  3      [ ]         STREAM     CONNECTED     20150    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     20201    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     20147    
unix  3      [ ]         STREAM     CONNECTED     26728    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     120767   /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     118313   
unix  3      [ ]         STREAM     CONNECTED     20080    
unix  3      [ ]         STREAM     CONNECTED     21069    
unix  3      [ ]         STREAM     CONNECTED     20980    
unix  3      [ ]         STREAM     CONNECTED     28529    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     22772    
unix  3      [ ]         STREAM     CONNECTED     28105    
unix  3      [ ]         STREAM     CONNECTED     124397   
unix  3      [ ]         STREAM     CONNECTED     21217    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     24901    
unix  3      [ ]         STREAM     CONNECTED     24762    
unix  3      [ ]         STREAM     CONNECTED     120040   /run/user/1000/sway-ipc.1000.956.sock
unix  3      [ ]         STREAM     CONNECTED     294492   
unix  3      [ ]         STREAM     CONNECTED     294491   
unix  3      [ ]         STREAM     CONNECTED     23832    
unix  3      [ ]         STREAM     CONNECTED     121628   
unix  3      [ ]         STREAM     CONNECTED     25797    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     122905   /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     25805    
unix  3      [ ]         STREAM     CONNECTED     26739    
unix  3      [ ]         STREAM     CONNECTED     22778    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     18137    
unix  3      [ ]         DGRAM      CONNECTED     18030    
unix  3      [ ]         STREAM     CONNECTED     33247    
unix  3      [ ]         DGRAM      CONNECTED     18833    
unix  3      [ ]         STREAM     CONNECTED     34057    @/tmp/.X11-unix/X1
unix  2      [ ]         DGRAM      CONNECTED     981      
unix  3      [ ]         STREAM     CONNECTED     118608   
unix  3      [ ]         STREAM     CONNECTED     27648    
unix  3      [ ]         STREAM     CONNECTED     20062    
unix  3      [ ]         STREAM     CONNECTED     18140    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24028    
unix  3      [ ]         STREAM     CONNECTED     29656    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     31464    
unix  3      [ ]         STREAM     CONNECTED     25865    
unix  3      [ ]         SEQPACKET  CONNECTED     117559   
unix  2      [ ]         DGRAM      CONNECTED     24976    
unix  3      [ ]         STREAM     CONNECTED     29662    
unix  3      [ ]         STREAM     CONNECTED     23834    
unix  3      [ ]         STREAM     CONNECTED     23833    
unix  3      [ ]         STREAM     CONNECTED     120039   /run/user/1000/sway-ipc.1000.956.sock
unix  2      [ ]         DGRAM                    25754    /run/user/1000/systemd/notify
unix  3      [ ]         STREAM     CONNECTED     21215    
unix  3      [ ]         STREAM     CONNECTED     120204   
unix  3      [ ]         STREAM     CONNECTED     20176    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     26803    
unix  3      [ ]         STREAM     CONNECTED     26682    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     18136    /run/dbus/system_bus_socket
unix  4      [ ]         DGRAM      CONNECTED     15401    /run/systemd/notify
unix  3      [ ]         STREAM     CONNECTED     20177    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     19734    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     33245    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     19980    /run/dbus/system_bus_socket
unix  3      [ ]         DGRAM      CONNECTED     15403    
unix  3      [ ]         STREAM     CONNECTED     118315   
unix  2      [ ]         DGRAM      CONNECTED     20981    
unix  3      [ ]         STREAM     CONNECTED     31465    
unix  3      [ ]         STREAM     CONNECTED     20113    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     33828    
unix  3      [ ]         STREAM     CONNECTED     25896    
unix  3      [ ]         STREAM     CONNECTED     23975    
unix  3      [ ]         STREAM     CONNECTED     32222    
unix  3      [ ]         STREAM     CONNECTED     34059    @/tmp/.X11-unix/X1
unix  3      [ ]         STREAM     CONNECTED     32116    
unix  3      [ ]         STREAM     CONNECTED     23047    
unix  14     [ ]         DGRAM      CONNECTED     15417    /run/systemd/journal/dev-log
unix  3      [ ]         STREAM     CONNECTED     28488    
unix  3      [ ]         STREAM     CONNECTED     25820    /run/user/1000/bus
unix  7      [ ]         DGRAM      CONNECTED     15419    /run/systemd/journal/socket
unix  3      [ ]         STREAM     CONNECTED     294484   
unix  3      [ ]         STREAM     CONNECTED     294483   
unix  3      [ ]         STREAM     CONNECTED     23957    
unix  3      [ ]         STREAM     CONNECTED     24948    
unix  2      [ ]         DGRAM      CONNECTED     23748    
unix  3      [ ]         STREAM     CONNECTED     30930    
unix  2      [ ]         DGRAM                    26766    
unix  3      [ ]         STREAM     CONNECTED     127273   
unix  3      [ ]         STREAM     CONNECTED     23126    
unix  2      [ ]         DGRAM      CONNECTED     23125    
unix  3      [ ]         STREAM     CONNECTED     22358    
unix  3      [ ]         STREAM     CONNECTED     25941    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     26790    
unix  3      [ ]         STREAM     CONNECTED     20101    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     27659    
unix  3      [ ]         STREAM     CONNECTED     18188    
unix  3      [ ]         STREAM     CONNECTED     34818    
unix  3      [ ]         STREAM     CONNECTED     27663    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     18409    /tmp/sddm-authfc9f8dcf-c02e-4013-830c-9ec5ba9b6cdd
unix  3      [ ]         STREAM     CONNECTED     23740    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     116446   
unix  3      [ ]         STREAM     CONNECTED     31462    
unix  3      [ ]         STREAM     CONNECTED     34834    
unix  3      [ ]         STREAM     CONNECTED     26726    
unix  3      [ ]         STREAM     CONNECTED     23751    
unix  3      [ ]         STREAM     CONNECTED     21403    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     28512    
unix  3      [ ]         DGRAM      CONNECTED     122643   
unix  3      [ ]         STREAM     CONNECTED     26566    
unix  2      [ ]         DGRAM      CONNECTED     18025    
unix  3      [ ]         STREAM     CONNECTED     21233    /run/user/1000/at-spi/bus_1
unix  3      [ ]         STREAM     CONNECTED     25759    
unix  3      [ ]         STREAM     CONNECTED     26727    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     118314   
unix  3      [ ]         STREAM     CONNECTED     29652    
unix  3      [ ]         STREAM     CONNECTED     23755    
unix  3      [ ]         STREAM     CONNECTED     21407    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25053    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     18189    
unix  3      [ ]         STREAM     CONNECTED     28928    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25138    
unix  3      [ ]         STREAM     CONNECTED     28104    
unix  3      [ ]         STREAM     CONNECTED     26692    
unix  3      [ ]         STREAM     CONNECTED     20053    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     31147    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23503    /run/user/1000/gvfsd/socket-RlkCcdrk
unix  3      [ ]         STREAM     CONNECTED     21161    
unix  3      [ ]         STREAM     CONNECTED     118999   /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     21243    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     125248   /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     34826    
unix  3      [ ]         STREAM     CONNECTED     29647    
unix  3      [ ]         STREAM     CONNECTED     26729    
unix  3      [ ]         STREAM     CONNECTED     23745    
unix  3      [ ]         STREAM     CONNECTED     118312   
unix  3      [ ]         STREAM     CONNECTED     23979    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     22773    
unix  3      [ ]         STREAM     CONNECTED     28129    
unix  2      [ ]         DGRAM      CONNECTED     18413    
unix  3      [ ]         STREAM     CONNECTED     22872    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     294490   
unix  3      [ ]         STREAM     CONNECTED     21066    
unix  3      [ ]         STREAM     CONNECTED     113655   /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     27695    /run/user/1000/bus
unix  2      [ ]         DGRAM                    16263    
unix  3      [ ]         STREAM     CONNECTED     22776    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     21171    
unix  3      [ ]         STREAM     CONNECTED     119236   
unix  3      [ ]         STREAM     CONNECTED     26879    
unix  3      [ ]         STREAM     CONNECTED     20098    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     30298    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     30801    
unix  3      [ ]         STREAM     CONNECTED     21150    /run/user/1000/bus
unix  2      [ ]         DGRAM                    24000    
unix  2      [ ]         DGRAM      CONNECTED     18829    
unix  3      [ ]         STREAM     CONNECTED     29648    
unix  3      [ ]         STREAM     CONNECTED     21105    
unix  3      [ ]         STREAM     CONNECTED     23825    
unix  3      [ ]         STREAM     CONNECTED     118464   
unix  3      [ ]         STREAM     CONNECTED     120041   /run/user/1000/sway-ipc.1000.956.sock
unix  3      [ ]         STREAM     CONNECTED     116447   
unix  3      [ ]         STREAM     CONNECTED     24982    
unix  3      [ ]         STREAM     CONNECTED     20153    
unix  3      [ ]         SEQPACKET  CONNECTED     27618    
unix  3      [ ]         SEQPACKET  CONNECTED     27612    
unix  3      [ ]         STREAM     CONNECTED     27340    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     28528    
unix  3      [ ]         STREAM     CONNECTED     20042    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     22419    
unix  3      [ ]         STREAM     CONNECTED     29312    /run/user/1000/gvfsd/socket-E3mNGVL1
unix  3      [ ]         STREAM     CONNECTED     25153    
unix  3      [ ]         STREAM     CONNECTED     25104    
unix  3      [ ]         STREAM     CONNECTED     20104    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     29663    
unix  3      [ ]         STREAM     CONNECTED     23737    
unix  3      [ ]         DGRAM      CONNECTED     21265    
unix  3      [ ]         STREAM     CONNECTED     31466    
unix  3      [ ]         STREAM     CONNECTED     21249    
unix  3      [ ]         STREAM     CONNECTED     21223    /run/user/1000/at-spi/bus_1
unix  3      [ ]         STREAM     CONNECTED     21404    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25955    /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     20054    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23980    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     22499    
unix  3      [ ]         STREAM     CONNECTED     19745    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     29314    
unix  3      [ ]         STREAM     CONNECTED     16244    
unix  3      [ ]         STREAM     CONNECTED     22775    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     267152   
unix  3      [ ]         STREAM     CONNECTED     25795    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM      CONNECTED     20797    
unix  3      [ ]         STREAM     CONNECTED     23100    
unix  3      [ ]         STREAM     CONNECTED     25958    /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     26748    
unix  3      [ ]         STREAM     CONNECTED     395991   
unix  3      [ ]         STREAM     CONNECTED     21065    
unix  3      [ ]         STREAM     CONNECTED     19754    
unix  3      [ ]         STREAM     CONNECTED     34052    @/tmp/.X11-unix/X1
unix  3      [ ]         STREAM     CONNECTED     31513    
unix  3      [ ]         STREAM     CONNECTED     22806    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     117552   
unix  2      [ ]         DGRAM                    119012   /run/wpa_supplicant/wlan0
unix  3      [ ]         STREAM     CONNECTED     28156    
unix  3      [ ]         STREAM     CONNECTED     193775   
unix  2      [ ]         DGRAM                    117495   /run/wpa_supplicant/p2p-dev-wlan0
unix  3      [ ]         STREAM     CONNECTED     26567    
unix  3      [ ]         STREAM     CONNECTED     30310    
unix  3      [ ]         STREAM     CONNECTED     21176    
unix  3      [ ]         STREAM     CONNECTED     24018    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25940    
unix  3      [ ]         STREAM     CONNECTED     25871    
unix  3      [ ]         STREAM     CONNECTED     24977    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     119157   
unix  3      [ ]         STREAM     CONNECTED     23971    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     26743    
unix  3      [ ]         STREAM     CONNECTED     20982    /run/dbus/system_bus_socket
unix  2      [ ]         DGRAM                    21172    
unix  3      [ ]         STREAM     CONNECTED     26693    
unix  3      [ ]         STREAM     CONNECTED     193776   
unix  3      [ ]         DGRAM      CONNECTED     122644   
unix  3      [ ]         STREAM     CONNECTED     26562    
unix  3      [ ]         STREAM     CONNECTED     26559    
unix  3      [ ]         SEQPACKET  CONNECTED     27616    
unix  3      [ ]         STREAM     CONNECTED     23370    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20148    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     23127    /run/user/1000/bus
unix  2      [ ]         DGRAM                    18184    
unix  2      [ ]         DGRAM      CONNECTED     18139    
unix  3      [ ]         STREAM     CONNECTED     123444   
unix  3      [ ]         STREAM     CONNECTED     267151   
unix  3      [ ]         STREAM     CONNECTED     124396   /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     120045   /run/user/1000/wayland-1
unix  2      [ ]         DGRAM      CONNECTED     15714    
unix  3      [ ]         STREAM     CONNECTED     29660    
unix  3      [ ]         STREAM     CONNECTED     21071    
unix  3      [ ]         STREAM     CONNECTED     20152    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     26774    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     21226    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     28091    
unix  3      [ ]         STREAM     CONNECTED     23076    
unix  3      [ ]         STREAM     CONNECTED     28157    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25864    
unix  3      [ ]         STREAM     CONNECTED     34066    
unix  3      [ ]         STREAM     CONNECTED     33825    
unix  3      [ ]         STREAM     CONNECTED     21165    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     27662    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     24973    
unix  3      [ ]         SEQPACKET  CONNECTED     117554   
unix  3      [ ]         STREAM     CONNECTED     29651    
unix  3      [ ]         STREAM     CONNECTED     23905    
unix  3      [ ]         STREAM     CONNECTED     23829    
unix  3      [ ]         STREAM     CONNECTED     26681    
unix  3      [ ]         STREAM     CONNECTED     26746    
unix  3      [ ]         STREAM     CONNECTED     26745    
unix  3      [ ]         STREAM     CONNECTED     27668    
unix  3      [ ]         STREAM     CONNECTED     27664    
unix  3      [ ]         STREAM     CONNECTED     24907    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20130    
unix  3      [ ]         STREAM     CONNECTED     23939    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23367    
unix  3      [ ]         STREAM     CONNECTED     20131    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     34827    
unix  3      [ ]         STREAM     CONNECTED     24965    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     29659    
unix  3      [ ]         STREAM     CONNECTED     21089    
unix  3      [ ]         STREAM     CONNECTED     119234   /run/user/1000/pulse/native
unix  3      [ ]         STREAM     CONNECTED     22931    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     25755    
unix  3      [ ]         STREAM     CONNECTED     32221    
unix  3      [ ]         STREAM     CONNECTED     32208    
unix  3      [ ]         STREAM     CONNECTED     28513    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23075    
unix  3      [ ]         STREAM     CONNECTED     28515    
unix  3      [ ]         STREAM     CONNECTED     23463    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     120779   /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25111    
unix  3      [ ]         STREAM     CONNECTED     25110    
unix  3      [ ]         STREAM     CONNECTED     266119   /run/user/1000/wayland-1
unix  2      [ ]         DGRAM      CONNECTED     23763    
unix  3      [ ]         STREAM     CONNECTED     294488   
unix  3      [ ]         STREAM     CONNECTED     189363   
unix  3      [ ]         STREAM     CONNECTED     189362   
unix  3      [ ]         STREAM     CONNECTED     22450    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     127309   
unix  3      [ ]         STREAM     CONNECTED     33246    
unix  3      [ ]         SEQPACKET  CONNECTED     27613    
unix  3      [ ]         STREAM     CONNECTED     23119    
unix  3      [ ]         STREAM     CONNECTED     21149    
unix  2      [ ]         DGRAM      CONNECTED     22498    
unix  3      [ ]         STREAM     CONNECTED     31463    
unix  2      [ ]         DGRAM                    18412    
unix  3      [ ]         STREAM     CONNECTED     401816   
unix  3      [ ]         STREAM     CONNECTED     118996   
unix  3      [ ]         STREAM     CONNECTED     25934    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25875    
unix  3      [ ]         STREAM     CONNECTED     22414    
unix  3      [ ]         STREAM     CONNECTED     120042   /run/user/1000/pulse/native
unix  3      [ ]         STREAM     CONNECTED     27696    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     24916    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     29658    
unix  3      [ ]         STREAM     CONNECTED     19813    
unix  3      [ ]         STREAM     CONNECTED     120110   /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     24401    
unix  3      [ ]         STREAM     CONNECTED     31153    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     21224    
unix  3      [ ]         STREAM     CONNECTED     28516    
unix  3      [ ]         STREAM     CONNECTED     21192    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25956    /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     25821    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21318    
unix  3      [ ]         DGRAM      CONNECTED     21266    
unix  3      [ ]         STREAM     CONNECTED     125581   
unix  3      [ ]         STREAM     CONNECTED     25960    
unix  3      [ ]         STREAM     CONNECTED     27658    
unix  2      [ ]         DGRAM                    252199   
unix  3      [ ]         STREAM     CONNECTED     118401   
unix  3      [ ]         STREAM     CONNECTED     20081    
unix  3      [ ]         STREAM     CONNECTED     20067    
unix  3      [ ]         STREAM     CONNECTED     21067    
unix  3      [ ]         STREAM     CONNECTED     267145   
unix  3      [ ]         STREAM     CONNECTED     19746    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     26776    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     23990    
unix  3      [ ]         STREAM     CONNECTED     32120    
unix  3      [ ]         STREAM     CONNECTED     21211    /run/user/1000/at-spi/bus_1
unix  3      [ ]         STREAM     CONNECTED     25822    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     22927    
unix  3      [ ]         STREAM     CONNECTED     26777    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21230    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21162    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     294487   
unix  3      [ ]         STREAM     CONNECTED     34831    
unix  3      [ ]         STREAM     CONNECTED     121709   
unix  3      [ ]         STREAM     CONNECTED     24765    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     24967    
unix  3      [ ]         STREAM     CONNECTED     20020    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     34060    @/tmp/.X11-unix/X1
unix  3      [ ]         STREAM     CONNECTED     20966    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     401818   /run/user/1000/wayland-1
unix  3      [ ]         DGRAM      CONNECTED     15402    
unix  3      [ ]         STREAM     CONNECTED     26773    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20119    
unix  3      [ ]         STREAM     CONNECTED     21068    
unix  3      [ ]         STREAM     CONNECTED     26810    
unix  3      [ ]         STREAM     CONNECTED     28494    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     25881    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     26671    
unix  3      [ ]         STREAM     CONNECTED     24979    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     24036    
unix  3      [ ]         STREAM     CONNECTED     21225    /run/user/1000/bus
unix  3      [ ]         DGRAM      CONNECTED     18029    
unix  3      [ ]         STREAM     CONNECTED     120038   /run/user/1000/sway-ipc.1000.956.sock
unix  3      [ ]         STREAM     CONNECTED     21044    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     116448   
unix  2      [ ]         DGRAM      CONNECTED     25747    
unix  3      [ ]         STREAM     CONNECTED     294482   
unix  3      [ ]         STREAM     CONNECTED     118316   
unix  3      [ ]         STREAM     CONNECTED     34835    
unix  3      [ ]         STREAM     CONNECTED     23830    
unix  3      [ ]         STREAM     CONNECTED     123729   /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     18428    
unix  3      [ ]         STREAM     CONNECTED     32209    
unix  3      [ ]         STREAM     CONNECTED     28531    /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     34065    
unix  3      [ ]         STREAM     CONNECTED     20149    
unix  3      [ ]         STREAM     CONNECTED     34055    @/tmp/.X11-unix/X1
unix  3      [ ]         STREAM     CONNECTED     16243    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     118309   
unix  3      [ ]         STREAM     CONNECTED     19979    
unix  3      [ ]         DGRAM      CONNECTED     25756    
unix  3      [ ]         STREAM     CONNECTED     23831    
unix  3      [ ]         STREAM     CONNECTED     120043   /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     28489    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     26732    /run/user/1000/at-spi/bus_1
unix  3      [ ]         STREAM     CONNECTED     22973    
unix  3      [ ]         STREAM     CONNECTED     120203   
unix  3      [ ]         STREAM     CONNECTED     26233    /run/systemd/journal/stdout
unix  3      [ ]         DGRAM      CONNECTED     18032    
unix  3      [ ]         STREAM     CONNECTED     120046   
unix  3      [ ]         STREAM     CONNECTED     34056    
unix  3      [ ]         STREAM     CONNECTED     21164    
unix  3      [ ]         STREAM     CONNECTED     400925   
unix  3      [ ]         STREAM     CONNECTED     118463   
unix  3      [ ]         STREAM     CONNECTED     34817    
unix  3      [ ]         STREAM     CONNECTED     23901    
unix  3      [ ]         STREAM     CONNECTED     29655    
unix  3      [ ]         STREAM     CONNECTED     23538    /run/user/1000/gvfsd/socket-LunNYvbu
unix  3      [ ]         STREAM     CONNECTED     32210    
unix  3      [ ]         STREAM     CONNECTED     20029    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     28530    
unix  3      [ ]         STREAM     CONNECTED     20122    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     24985    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     28539    /run/user/1000/pipewire-0
unix  3      [ ]         STREAM     CONNECTED     119011   /run/user/1000/bus
unix  3      [ ]         SEQPACKET  CONNECTED     117553   
unix  3      [ ]         STREAM     CONNECTED     29657    
unix  3      [ ]         STREAM     CONNECTED     19989    
unix  3      [ ]         STREAM     CONNECTED     25799    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     23885    
unix  3      [ ]         STREAM     CONNECTED     127308   
unix  3      [ ]         STREAM     CONNECTED     23118    
unix  3      [ ]         STREAM     CONNECTED     21210    
unix  3      [ ]         DGRAM      CONNECTED     18834    
unix  3      [ ]         STREAM     CONNECTED     28532    /run/user/1000/bus
unix  2      [ ]         DGRAM                    26784    
unix  2      [ ]         DGRAM                    27690    
unix  3      [ ]         STREAM     CONNECTED     401817   
unix  3      [ ]         STREAM     CONNECTED     25144    
unix  3      [ ]         STREAM     CONNECTED     25880    
unix  3      [ ]         STREAM     CONNECTED     22762    
unix  3      [ ]         STREAM     CONNECTED     26741    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     294480   
unix  3      [ ]         STREAM     CONNECTED     125222   /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     27647    
unix  3      [ ]         STREAM     CONNECTED     23750    
unix  3      [ ]         STREAM     CONNECTED     116449   
unix  3      [ ]         STREAM     CONNECTED     25727    
unix  3      [ ]         STREAM     CONNECTED     19988    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     24923    
unix  3      [ ]         STREAM     CONNECTED     34175    
unix  3      [ ]         STREAM     CONNECTED     26775    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     26740    /run/user/1000/bus
unix  3      [ ]         STREAM     CONNECTED     26561    
unix  3      [ ]         STREAM     CONNECTED     18002    
unix  3      [ ]         STREAM     CONNECTED     125580   
unix  3      [ ]         STREAM     CONNECTED     23074    
unix  3      [ ]         STREAM     CONNECTED     22380    
unix  3      [ ]         STREAM     CONNECTED     392146   /run/user/1000/wayland-1
unix  3      [ ]         SEQPACKET  CONNECTED     117557   
unix  3      [ ]         STREAM     CONNECTED     20123    
unix  3      [ ]         STREAM     CONNECTED     21070    
unix  3      [ ]         STREAM     CONNECTED     120976   /run/user/1000/at-spi/bus_1
unix  3      [ ]         STREAM     CONNECTED     31512    
unix  3      [ ]         STREAM     CONNECTED     25061    
unix  3      [ ]         STREAM     CONNECTED     123433   
unix  3      [ ]         STREAM     CONNECTED     22901    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     21251    /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     32115    
unix  3      [ ]         STREAM     CONNECTED     33821    
unix  3      [ ]         STREAM     CONNECTED     23128    
unix  3      [ ]         STREAM     CONNECTED     21216    
unix  3      [ ]         STREAM     CONNECTED     116525   /run/dbus/system_bus_socket
unix  3      [ ]         STREAM     CONNECTED     25951    
unix  3      [ ]         STREAM     CONNECTED     34061    @/tmp/.X11-unix/X1
unix  3      [ ]         STREAM     CONNECTED     29897    
unix  3      [ ]         STREAM     CONNECTED     20100    /run/user/1000/wayland-1
unix  3      [ ]         STREAM     CONNECTED     20483    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     294489   
unix  3      [ ]         STREAM     CONNECTED     34832    
unix  2      [ ]         DGRAM      CONNECTED     25733    
unix  3      [ ]         STREAM     CONNECTED     24924    /run/systemd/journal/stdout
unix  3      [ ]         STREAM     CONNECTED     20809    
unix  3      [ ]         STREAM     CONNECTED     33249    
unix  2      [ ]         DGRAM                    27109    
unix  3      [ ]         DGRAM      CONNECTED     18031    
unix  2      [ ]         DGRAM      CONNECTED     22369    
unix  3      [ ]         STREAM     CONNECTED     28282    /run/dbus/system_bus_socket
unix  3      [ ]         SEQPACKET  CONNECTED     27615    @abfa6
unix  3      [ ]         SEQPACKET  CONNECTED     27617    @2b1b7
unix  3      [ ]         SEQPACKET  CONNECTED     117558   @be48f
unix  2      [ ]         STREAM                   25879    @printer-applet-lock-user-ryanc
unix  3      [ ]         SEQPACKET  CONNECTED     117556   @93030
```
# Lab 3 - Python

Running the Original Files - I've copied the original files directly from the IOT repo as of 04/13/2023
```auto
Calendar Date: 2023-04-13
Julian Date: 2459988.5
Modified Julian Date: 59988.0
Date: 2023-04-13
Date: 04-13-23
Day of Week: Thursday
Month: April
Year: 2023
26 days after the first day of classes
80 days before the last day of classes
2023-04-13 17:44:46.265485
2023-04-13 17:44:46.265535
2023-04-13 22:44:46.265545
1676328286.2655518
Thu Apr 13 17:44:46 2023
2023-04-13 17:44:46.265616
2023-04-13 22:44:46.265626
Information for New York/USA

Timezone: US/Eastern
Latitude: 40.72; Longitude: -74.00

Dawn:    2023-02-13 06:24:16.679789-05:00
Sunrise: 2023-02-13 06:52:59.652406-05:00
Noon:    2023-02-13 12:10:13-05:00
Sunset:  2023-02-13 17:27:57.563584-05:00
Dusk:    2023-02-13 17:56:41.814544-05:00
2023-04-13 Moon Phase: 20
2023-04-14 Moon Phase: 21
2023-04-15 Moon Phase: 22
2023-04-16 Moon Phase: 23
2023-04-17 Moon Phase: 24
2023-04-18 Moon Phase: 25
2023-04-19 Moon Phase: 27
2023-04-20 Moon Phase: 0
2023-04-21 Moon Phase: 1
2023-04-22 Moon Phase: 2
2023-04-23 Moon Phase: 3
2023-04-24 Moon Phase: 4
2023-04-25 Moon Phase: 5
2023-04-26 Moon Phase: 6
2023-04-27 Moon Phase: 7
2023-04-28 Moon Phase: 8
2023-05-01 Moon Phase: 8
2023-05-02 Moon Phase: 9
2023-05-03 Moon Phase: 10
2023-05-04 Moon Phase: 11
2023-05-05 Moon Phase: 12
2023-05-06 Moon Phase: 13
2023-05-07 Moon Phase: 13
2023-05-08 Moon Phase: 14
2023-05-09 Moon Phase: 15
2023-05-10 Moon Phase: 16
2023-05-11 Moon Phase: 17
2023-05-12 Moon Phase: 18
2023-05-13 Moon Phase: 19
2023-05-14 Moon Phase: 20
Library Parking, Williams Lake, Cariboo Regional District, British Columbia, Canada
(52.130143399999994, -122.14187089155848)
Stevens Institute of Technology, Field House Road, Hoboken, Hudson County, New Jersey, 07030, United States
(40.744809599999996, -74.0252392276461)
sbattery(percent=40.565493364108484, secsleft=17575, power_plugged=False)
Word Count: 1343
Top Ten Words: [('our', 26), ('their', 20), ('has', 20), ('he', 19), ('them', 15), ('these', 13), ('have', 11), ('we', 11), ('us', 11), ('people', 10)]
The number of physical cores =  4
The number of logical CPUs =  8
The utilization per second as a percentage for each CPU
[5.1, 3.1, 1.0, 3.1, 6.0, 7.1, 3.1, 6.3]
[3.0, 7.1, 5.2, 1.0, 6.1, 3.0, 2.0, 7.1]
[0.0, 0.0, 2.9, 4.0, 1.0, 2.0, 0.0, 0.0]
[2.0, 0.0, 1.0, 0.0, 1.0, 1.0, 1.0, 1.0]
[0.0, 4.2, 2.1, 5.1, 2.0, 0.0, 0.0, 2.0]
[1.0, 2.1, 5.1, 2.0, 0.0, 0.0, 0.0, 4.0]
[0.0, 2.1, 6.1, 4.0, 3.0, 1.0, 1.0, 3.0]
[0.0, 1.1, 1.0, 1.0, 0.0, 0.0, 1.0, 2.0]
[1.0, 0.0, 1.0, 0.0, 0.0, 1.0, 1.0, 2.0]
[1.0, 1.1, 1.0, 6.0, 0.0, 1.0, 1.0, 1.0]
Thu Apr 13 17:44:59 2023
Thu Apr 13 17:45:09 2023
```

Running Modified Files
```auto
Calendar Date: 2023-04-13
Julian Date: 2459988.5
Modified Julian Date: 59988.0
Date: 2023-04-13
Date: 04-13-23
Day of Week: Thursday
Month: April
Year: 2023
26 days after the first day of classes
80 days before the last day of classes
2023-04-13 17:43:55.200199
2023-04-13 17:43:55.200248
2023-04-13 22:43:55.200258
1676328235.200265
Thu Apr 13 17:43:55 2023
2023-04-13 17:43:55.200328
2023-04-13 22:43:55.200336
Information for New York/USA

Timezone: US/Eastern
Latitude: 40.72; Longitude: -74.00

Dawn:    2023-04-13 06:24:16.679789-05:00
Sunrise: 2023-04-13 06:52:59.652406-05:00
Noon:    2023-04-13 12:10:13-05:00
Sunset:  2023-04-13 17:27:57.563584-05:00
Dusk:    2023-04-13 17:56:41.814544-05:00
2023-04-13 Moon Phase: 20
2023-04-14 Moon Phase: 21
2023-04-15 Moon Phase: 22
2023-04-16 Moon Phase: 23
2023-04-17 Moon Phase: 24
2023-04-18 Moon Phase: 25
2023-04-19 Moon Phase: 27
2023-04-20 Moon Phase: 0
2023-04-21 Moon Phase: 1
2023-04-22 Moon Phase: 2
2023-04-23 Moon Phase: 3
2023-04-24 Moon Phase: 4
2023-04-25 Moon Phase: 5
2023-04-26 Moon Phase: 6
2023-04-27 Moon Phase: 7
2023-04-28 Moon Phase: 8
2023-05-01 Moon Phase: 8
2023-05-02 Moon Phase: 9
2023-05-03 Moon Phase: 10
2023-05-04 Moon Phase: 11
2023-05-05 Moon Phase: 12
2023-05-06 Moon Phase: 13
2023-05-07 Moon Phase: 13
2023-05-08 Moon Phase: 14
2023-05-09 Moon Phase: 15
2023-05-10 Moon Phase: 16
2023-05-11 Moon Phase: 17
2023-05-12 Moon Phase: 18
2023-05-13 Moon Phase: 19
2023-05-14 Moon Phase: 20
Library Parking, Williams Lake, Cariboo Regional District, British Columbia, Canada
(52.130143399999994, -122.14187089155848)
Stevens Institute of Technology, Field House Road, Hoboken, Hudson County, New Jersey, 07030, United States
(40.744809599999996, -74.0252392276461)
sbattery(percent=40.75783804577804, secsleft=16659, power_plugged=False)
Word Count: 1343
Top Ten Words: [('our', 26), ('their', 20), ('has', 20), ('he', 19), ('them', 15), ('these', 13), ('have', 11), ('we', 11), ('us', 11), ('people', 10)]
The number of physical cores = 4
The number of logical CPUs = 8
The utilization per second as a percentage for each CPU
[3.9, 4.0, 3.9, 1.0, 3.0, 1.0, 5.1, 7.5]
[6.9, 3.9, 6.8, 0.0, 3.0, 4.0, 6.0, 4.0]
[6.9, 9.9, 10.9, 11.7, 10.7, 5.2, 7.0, 5.9]
[4.9, 1.0, 2.0, 6.7, 4.0, 4.9, 0.0, 3.0]
[4.0, 3.0, 2.9, 11.7, 1.0, 2.0, 0.0, 1.0]
[3.9, 3.0, 4.0, 7.6, 1.0, 4.0, 3.1, 1.0]
[2.0, 1.0, 8.0, 5.0, 2.0, 5.9, 5.1, 4.9]
[4.0, 3.0, 9.8, 9.0, 2.0, 6.9, 5.9, 7.9]
[2.9, 1.0, 7.8, 2.0, 0.0, 1.0, 2.0, 13.2]
[0.0, 3.0, 4.0, 5.8, 3.0, 0.0, 0.0, 11.3]
Thu Apr 13 17:44:08 2023
Thu Apr 13 17:44:18 2023
Thu Apr 13 17:44:28 2023
Thu Apr 13 17:44:38 2023
```
