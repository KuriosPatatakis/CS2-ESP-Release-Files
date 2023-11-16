Loading the driver in windows 11 poses a challenge
required actions :

1.Turn off Driver signing enforcement (google it)
2.Create a txt file (name it whatever you want).
3.Copy ,paste and modify this code :

start C:\..\CS2-ESP-Release-Files\OnlyForWindows11\dsefix.exe
timeout /t 2
sc create tutDriverr binpath=C:\..\CS2-ESP-Release-Files\OnlyForWindows11\YeeterDriver.sys type=kernel
sc start tutDriverr
timeout /t 5
start C:\..\CS2-ESP-Release-Files\OnlyForWindows11\dsefix.exe -e
timeout /t 2

4.Replace \..\ with your file destinasion and save
5.Rename the file from .txt to .bat
6.Run the file AS ADMINISTRATOR

From now on games that use an anti-cheat like battleye or easy anticheat will not work. Before trying to play games that use these
anticheat programs be sure to turn on Driver signing enforcement (from step 1) and reboot (obviously).