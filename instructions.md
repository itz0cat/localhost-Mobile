# Step 1 - Setup
Install Termux from trusted sources like [GitHub](https://github.com/termux/termux-app/releases) or [F-Droid](https://f-droid.org/en/packages/com.termux/).
Install Anlinux From [Playstore](https://play.google.com/store/apps/details?id=exa.lnx.a&hl=en_IN&pli=1).
Open AnLinux, navigate to the Dashboard, and select Ubuntu to proceed.
Then copy the command on your screen their will be a `copy` button. Then press `launch`.
Paste the command you just copied into Termux.
It will Take a while... propably 30sec - 8min (depending on your network and device i guess)
After done, run ```./start-ubuntu.sh```
 # Step 2 - Install Required Packages
Run these commands one by one!
 
1.```apt update```

2.```apt-get clean```

3.```apt-get install -y build-essential```

4.```apt-get install software-properties-common```

5.```add-apt-repository ppa:openjdk-r/ppa```

6.```apt-get update```

7.```apt-get install openjdk-8-jre```

8.```apt-get install openjdk-21-jdk```

`wget -O minecraft_server.jar (Link of the file)`
**Do note that you can use a link to PaperMC, or Spigot, or whatever else, just replace the name and the link, for example, `wget -O paper-1.20.4-496.jar (link to paper 1.20.4)`
 
 # Step 3 - Make the file executable
```chmod +x minecraft_server.jar```
# NOTE
** if you used paper or whatever else, change `minecraft_server.jar` to whatever else you used, for example, `chmod +x paper-1.20.4-496.jar`

# Step 4 - Run the sever
```java -Xmx(MAX RAM AMOUNT) -Xms (MIN RAM AMOUNT) -jar minecraft_server.jar nogui```
# NOTE 
If you used paper or whatever else, change "minecraft_server.jar" to whatever else you used, for example, `java -Xmx(RAM AMOUNT) -Xms (RAM AMOUNT) -jar paper-1.20.4-496.jar nogui`
 
Let it run until it shows eula warining.

# Setp 5 - Install Nano and agree Eula
 Run the commands one by one. Dont be in hurry :)
```apt install nano```
```nano eula.txt```

 # Step 6 - Run the server fullly and ENJOY!

Then run
```java -Xmx(MAX RAM AMOUNT) -Xms (MIN RAM AMOUNT) -jar minecraft_server.jar nogui``` 
again

**And Done Now You are hosting server on your device! :D** 

To join just open Pojava and click Multiplayer then `Add Server` Set the name as your want and ip is ```localhost``` then click add and then join it.. 

Enjoy :D

# NOTE
It should be working now, do note that **this tutorial does not show port forwarding and how to show with friends, this is a completely local server**
#                -END-
