# Valorant-Rpcanother rewrite (v3) coming after I finish my API wrapper; should be much more optimized and clean
Please read through the README in its entirety before creating issues/messaging me!

 _    _____    __    ____  ____  ___    _   ________            ____  ____  ______
| |  / /   |  / /   / __ \/ __ \/   |  / | / /_  __/           / __ \/ __ \/ ____/
| | / / /| | / /   / / / / /_/ / /| | /  |/ / / /    ______   / /_/ / /_/ / /     
| |/ / ___ |/ /___/ /_/ / _, _/ ___ |/ /|  / / /    /_____/  / _, _/ ____/ /___   
|___/_/  |_/_____/\____/_/ |_/_/  |_/_/ |_/ /_/             /_/ |_/_/    \____/   
valorant-rich-presence-client
A feature-rich Discord rich-presence extension for VALORANT.

Images
![image](https://user-images.githubusercontent.com/49095369/117168891-3e4dfa80-add1-11eb-90a9-a7c15d3b979f.png)
 ![image](https://user-images.githubusercontent.com/49095369/117168906-427a1800-add1-11eb-910a-4a63c835a229.png)
  ![image](https://user-images.githubusercontent.com/49095369/117168935-49a12600-add1-11eb-8f4a-9be9be7f8634.png)

Installation
Antivirus might mark the installer executable as malicious, you can run it anyway

For most of you, select Install for all users; you'll know if you want to select the other option.

image

If you get a Windows notification from User Account Control, choose yes

image

Take note or copy of the path to your installation, you'll need it later!

image

During installation, you have a decision to make: "do I want the program to automatically launch with VALORANT (recommended), or do I want to manually launch it every time I play?". If you chose the second option, it is recommended you create a desktop shortcut, otherwise, ignore that option.

image

It is recommended you run the program after installing; it runs a few first-time setup tasks.

Editing the configuration
Navigate to %APPDATA%\valorant-rpc and open config.json with your favorite text editor

press WIN+R, type %APPDATA%\valorant-rpc then press enter

settings
launch_timeout: time, in seconds, the program should wait for VALORANT to launch. if the time passes before the game fully loads, the program will exit
menu_refresh_interval: how often, in seconds, the program should update your Discord presence while in the menus
ingame_refresh_interval: how often, in seconds, the program should update your Discord presence while in a game
debug: set to true to show a traceback when the program crashes (useful for bug reports!)
region
change this to your client's region, can be found in settings -> about -> game shard
rpc-oauth
leave this section blank; it stores the application's Discord authentication data
rpc-client-override
leave this section unchanged UNLESS you are setting up your own Discord application to share with friends so you can use the party invites feature. Read more about it here
Restarting the application
this DOES NOT close/restart VALORANT

After editing the configuration, locate the tray icon, right click it, and select restart image

The console window will reappear for a few seconds and the program will restart

Modifying the VALORANT launch target
This section is for the "I want the program to automatically launch with VALORANT" people from earlier

Locate the VALORANT shortcut

if you typically launch from your desktop, locate the VALORANT icon
if you typically launch from the search bar, search for VALORANT and open the file location
you can also do this for every VALORANT shortcut you have
Right click on the shortcut/icon, then select Properties

![image](https://user-images.githubusercontent.com/49095369/117168841-32facf00-add1-11eb-99c2-557f05a633f8.png)


In the Target box, paste the path to valorant-rpc.exe from when you installed (ex. C:\Program Files (x86)\valorant-rpc\valorant-rpc.exe), then select Apply
image

Launch VALORANT! The program console should appear for a few seconds before the game launches.
Legal Stuff
This project is not affiliated with Riot Games or any of its employees and therefore does not reflect the views of said parties. This is purely a fan-made project to enhance VALORANT's Discord integration.

Riot Games does not endorse or sponsor this project. Riot Games, and all associated properties are trademarks or registered trademarks of Riot Games, Inc.
