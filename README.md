Docker image which creates a Windows Server Core environment with Visual Studio 2019 and the below workloads installed:

C++ toolset
MSBuild
Windows 10 SDK

Hello World sample taken from here - https://github.com/microsoft/Windows-classic-samples

Requirements:

Docker (ensure to switch to Windows containers once installed)

Instructions:

Build Image - Open a command line and execute the command:

docker build -t buildtools2019:latest -m 2GB . 

Run Container - Execute:

docker run -it buildtools2019

Build Application - Execute:

msbuild /t:Rebuild

Credit:

https://docs.microsoft.com/en-us/visualstudio/install/build-tools-container?view=vs-2019
https://github.com/microsoft/Windows-classic-samples

