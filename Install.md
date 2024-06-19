# Installing WINE

# Ubuntu/Debian
```sh
sudo dpkg --add-architecture i386
wget -nc https://dl.winehq.org/wine-builds/winehq.key
sudo apt-key add winehq.key
sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ focal main' # For Ubuntu 20.04
sudo apt-get update
```
```sh
sudo apt-get install --install-recommends winehq-stable

```

# Arch Linux
```sh
sudo pacman -Syu wine
```

# Installing the official Jagex Launcher with Wine
```sh
wine setup_file.exe
```

# Installing the C# dependencies on Ubuntu/Debian
```sh
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
sudo apt-get update
sudo apt-get install -y apt-transport-https
sudo apt-get update
sudo apt-get install -y dotnet-sdk-7.0
```
# Installing the C# depencies on Arch Linux
```sh
dotnet new -i Avalonia.Templates
```



