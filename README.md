MonoGame demo application
===========================

The program displays a png file.

Linux
------------------

Install dependencies:

	sudo apt-get install libmonogame-cil monodevelop-monogame monodevelop

Run monodevelop build tool:

	mdtool build demo.linux.csproj

Run the demo program:

	mono bin/debug/demo.linux.exe

Linux + Wine
------------------

Install dependencies:

	sudo apt-get install wine
	wget http://winetricks.org/winetricks
	chmod +x winetricks 
 
Create wine environment:

	bash winetricks -q dotnet40 corefonts
	wget http://www.monogame.net/releases/MonoGame-2.5.1.0.exe
	wine MonoGame-2.5.1.0.exe 

Run build tool:

	 wine "C:\windows\Microsoft.NET\Framework\v4.0.30319\MsBuild.exe" demo.windows.csproj /t:Build

Run the demo program:

	wine bin/debug/demo.windows.exe
	
	
Windows
----------
	
NOT TESTED!

Install dependencies:
 - Install  .NET Framework 4

Run build tool:

	 "C:\windows\Microsoft.NET\Framework\v4.0.30319\MsBuild.exe" demo.windows.csproj /t:Build

Run the demo program:

	bin\debug\demo.windows.exe

	
	
