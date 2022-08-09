## install .Net6 on linux 20.04

$ wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
rm packages-microsoft-prod.deb

$ sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-6.0

## have a look a list of project we can create
dotnet new --list

## create blazor app
$ dotnet new blazorwasm -o BlazorWasmLinux

# run blazor app
$ dotnet run

https://localhost:7086/