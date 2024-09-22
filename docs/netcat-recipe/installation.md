# Installation

## Windows

```pwsh
scoop install netcat
```

or you can download the .exe file from [https://eternallybored.org/misc/netcat/](https://eternallybored.org/misc/netcat/)

## Debian/Ubuntu

```sh
# Traditional
sudo apt install netcat-traditional

sudo apt install netcat

# OpenBSD
sudo apt install netcat-openbsd

# Ncat
sudo apt install nmap
```

## CentOS

```sh
yum install nc
```

## MacOS

```zsh
brew install netcat
```

## Arch

```sh
sudo pacman -Syu netcat
```

## Make from source

### Traditional

visit the project [homepage](https://nc110.sourceforge.io/)

```sh
./configure
make
sudo make install
```

### GNU

visit the project [homepage](http://netcat.sourceforge.net)

```sh
cd netcat-0.7.1/
./configure
make
sudo make install
```
