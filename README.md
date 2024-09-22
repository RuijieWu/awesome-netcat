# awesome-netcat

```plaintext
 ██████\  ██\      ██\ ████████\  ██████\   ██████\  ██\      ██\ ████████\      ██\   ██\ ████████\ ████████\  ██████\   ██████\ ████████\ 
██  __██\ ██ | █\  ██ |██  _____|██  __██\ ██  __██\ ███\    ███ |██  _____|     ███\  ██ |██  _____|\__██  __|██  __██\ ██  __██\\__██  __|
██ /  ██ |██ |███\ ██ |██ |      ██ /  \__|██ /  ██ |████\  ████ |██ |           ████\ ██ |██ |         ██ |   ██ /  \__|██ /  ██ |  ██ |   
████████ |██ ██ ██\██ |█████\    \██████\  ██ |  ██ |██\██\██ ██ |█████\ ██████\ ██ ██\██ |█████\       ██ |   ██ |      ████████ |  ██ |   
██  __██ |████  _████ |██  __|    \____██\ ██ |  ██ |██ \███  ██ |██  __|\______|██ \████ |██  __|      ██ |   ██ |      ██  __██ |  ██ |   
██ |  ██ |███  / \███ |██ |      ██\   ██ |██ |  ██ |██ |\█  /██ |██ |           ██ |\███ |██ |         ██ |   ██ |  ██\ ██ |  ██ |  ██ |   
██ |  ██ |██  /   \██ |████████\ \██████  | ██████  |██ | \_/ ██ |████████\      ██ | \██ |████████\    ██ |   \██████  |██ |  ██ |  ██ |   
\__|  \__|\__/     \__|\________| \______/  \______/ \__|     \__|\________|     \__|  \__|\________|   \__|    \______/ \__|  \__|  \__|   
```

A curated collection of usage tips, common scenarios, FAQ, implementation and more for netcat

## Contents

- [About](#about)
- [Netcats](#netcats)
  - [Original](#original)
  - [Enhanced](#enhanced)
  - [Netcat-like Tools](#netcat-like-tools)
- [Recipes](#recipes)

## About

[Netcat](https://en.wikipedia.org/wiki/Netcat) which has been always considered as the TCP/IP swiss army knife offers powerful and flexible functions to help in Dev&Ops, Pentest and so on.
There are some differences between the elder and the latest netcat. Mostly we care about two of the latest variety , netcat-openbsd and ncat when netcat is concerned.

## Netcats

### Original

Version | Link | Description
--------|------|------------
netcat-traditional | [Project Home Page](https://nc110.sourceforge.io/) | Netcat Traditional is the original implementation, written by a guy named Hobbit. This is usually not pre-installed unless using a distro like Kali Linux. It is no longer maintained and is version 1.10.
GNU Netcat | [Project Home Page](http://netcat.sourceforge.net) | GNU Netcat is a rewrite of the original netcat to make it new and fully compliant with GNU portability. This means that it can be easily installed on almost all Linux distributions. This version is not available through the Package Manager. It also doesn't seem to be maintained anymore, as its latest version is 0.7.1 from 2004.
netcat-openbsd | [Free Software Wiki Page](https://directory.fsf.org/wiki/Netcat-openbsd) | The Netcat OpenBSD release is a rewrite of the original netcat, including support for IPv6, proxies, and unix sockets. In addition to these enhancements, it was also compiled to remove a feature that was considered a huge security vulnerability in the application.

The OpenBSD netcat is the most common, and you'll find it installed by default in Ubuntu distributions (desktop and server). For other Linux distributions, you may need to install it yourself. About how to install, see [Installation](./docs/netcat-recipe/installation.md)

### Enhanced

  Name  | Link | Description
--------|------|------------
NCat | [Project Home Page](https://nmap.org/ncat/) / [Github Repo](https://github.com/nmap/nmap/tree/master/ncat) | Ncat is a feature-packed networking utility which reads and writes data across networks from the command line. Ncat was written for the Nmap Project as a much-improved reimplementation of the venerable Netcat. It uses both TCP and UDP for communication and is designed to be a reliable back-end tool to instantly provide network connectivity to other applications and users. Ncat will not only work with IPv4 and IPv6 but provides the user with a virtually limitless number of potential uses.
socat | [Project Home Page](http://www.dest-unreach.org/socat/) / [Github Repo](https://github.com/3ndG4me/socat) | socat is a relay for bidirectional data transfer between two independent data channels. Each of these data channels may be a file, pipe, device (serial line etc. or a pseudo terminal), a socket (UNIX, IP4, IP6 - raw, UDP, TCP), an SSL socket, proxy CONNECT connection, a file descriptor (stdin etc.), the GNU line editor (readline), a program, or a combination of two of these.  These modes include generation of "listening" sockets, named pipes, and pseudo terminals.
rustcat | [Github Repo](https://github.com/robiot/rustcat) / [Official Website](https://git.io/rustcat) | an easy to use port listener and reverse shell for Linux, MacOS, and Windows aimed to be easy to use and accessible.
netcat(nodejs) | [Github Repo](https://github.com/roccomuso/netcat) | 💻 Netcat client and server modules written in pure Javascript for Node.js which has been fully tested modules that implements all the basic netcat's features. To use as standalone tool install the nc package.
nclib | [Github Repo](https://github.com/rhelmot/nclib) | nclib is a python socket library that wants to be your friend. It provides Easy-to-use interfaces for connecting to and listening on TCP and UDP sockets, The ability to handle any python stream-like object with a single interface, A better socket class, the Netcat object, and so on.
NetCat for Windows | [Github Repo](https://github.com/diegocr/netcat) | This NetCat for Windows was originally created by Rodney Beede, it's a version compiled without the GAPING_SECURITY_HOLE option (-e switch) which can trigger false positives in anti-virus programs.
netcat-windows | [Download Page](https://eternallybored.org/misc/netcat/) | This is another common netcat download upstream for Windows which is compiled for both 32 and 64-bit Windows.

### Netcat-like Tools

  Name  | Link | Description
--------|------|------------
pwncat | [Github Repo](https://github.com/cytopia/pwncat) / [Official Website](https://pwncat.org/) | a specialized netcat for cyber security on steroids with Firewall, IDS/IPS evasion, bind and reverse shell, self-injecting shell and port forwarding magic - and its fully scriptable with Python (PSE).
websocat | [Github Repo](https://github.com/vi/websocat) | websocat is a tool that allows you to connect to and serve WebSockets from the command line, with features like text and binary modes, proxying, SOCKS5, and more.
pcopy | [Github Repo](https://github.com/binwiederhier/pcopy) / [Official Website](https://nopaste.net/) | a temporary file host, nopaste and clipboard across machines. It can be used from the Web UI, via a CLI or without a client by using curl.
bondcat | [Github Repo](https://github.com/benjojo/bondcat) | A netcat like system utility that has the ability to combine multiple TCP connections for better transfer speeds, but also better reliability (Assuming the connections take different network paths).
streamhut | [Github Repo](https://github.com/miguelmota/streamhut) | Streamhut allows you to stream (pipe) realtime data from your terminal stdout/stderr to a web xterm UI or even to another terminal. It also allow you to quickly share data and files between devices.
wssh | [Github Repo](https://github.com/progrium/wssh) | a command-line utility/shell for WebSocket inspired by netcat.

## Recipes

 Recipe | URL | Description
--------|-----|------------
Netcat Manuals | [Netcat: the TCP/IP swiss army](https://nc110.sourceforge.io/) | A brief introduction on the features, examples of netcat.
Ncat User's Guide | [Ncat User's Guide](https://nmap.org/ncat/guide/index.html) | Nmap.org provided a very detailed and practical user guide for ncat and it's helpful for every netcat-like tool.
Netcat Manual | [Arch Wiki Page](https://man.archlinux.org/man/nc.1.en) | Arch Wiki explain how netcat can be used in Arch Linux in this page, including the exact usage of every option, practical examples and son on.
GNU Netcat Manual | [Arch Wiki Page](https://man.archlinux.org/man/netcat.1.en) | Almost the same as the former one but GNU netcat.
Bash-web-server | [Github Repo](https://github.com/dzove855/Bash-web-server) | A fantastic script which implement a web server with basic bash commands especially netcat.
piu-piu-SH | [Github Repo](https://github.com/vaniacer/piu-piu-SH) | An Old School horizontal scroller 'Shoot Them All' game in pure bash. With multiplayer modes team and duel. You have to defeat 100 aliens to fight with Boss. Netcat serves as the client-server exchange in multiplayer mode.
Reverse Shell Cheat Sheet | [Github Repo](https://github.com/security-cheatsheet/reverse-shell-cheatsheet) | Netcat plays an important role in pentest. Hackers usually create a reverse shell for remote control. This is an example.
shellver | [Github Repo](https://github.com/0xR0/shellver) | Similar to Reverse Shell Cheat Sheet
