
# **Hosting a Minecraft Server on Termux & AnLinux**  

## **Step 1 - Setup**  
1. Install **Termux** from trusted sources like [GitHub](https://github.com/termux/termux-app/releases) or [F-Droid](https://f-droid.org/en/packages/com.termux/).  
2. Install **AnLinux** from the [Google Play Store](https://play.google.com/store/apps/details?id=exa.lnx.a&hl=en_IN&pli=1).  
3. Open **AnLinux**, navigate to the **Dashboard**, and select **Ubuntu**.  
4. Copy the provided command and press **Launch**.  
5. Open **Termux**, paste the command, and wait for installation to complete (30 sec - 8 min).  
6. Once done, run:  
   ```bash
   ./start-ubuntu.sh
   ```  

## **Step 2 - Install Required Packages**  
Run the following commands **one by one**:  
```bash
apt update && apt install -y nano openjdk-17-jre
```

## **Step 3 - Download the Minecraft Server**  
Replace `<file_link>` with the download link for your server file.  
```bash
wget -O minecraft_server.jar <file_link>
```
Get `<file_link>` from [PaperMC.md](https://github.com/itz0cat/localhost-Mobile/blob/main/PaperMC.md)

Example for **PaperMC 1.20.4 (Build 499)**:  
```bash
wget -O minecraft_server.jar https://api.papermc.io/v2/projects/paper/versions/1.20.4/builds/499/downloads/paper-1.20.4-499.jar
```

## **Step 4 - Make the File Executable**  
```bash
chmod +x minecraft_server.jar
```

## **Step 5 - Run the Server**  
Replace `(RAM)` with your desired RAM allocation in GB.  
Example (using **2GB RAM**):  
```bash
java -Xmx2G -Xms2G -jar minecraft_server.jar nogui
```
Wait until you see the **EULA warning**.

## **Step 6 - Agree to the EULA**  
1. Open the EULA file with Nano:  
   ```bash
   nano eula.txt
   ```
2. Locate `eula=false` and change it to `eula=true`.  
3. Press `CTRL + X`, then `Y`, and hit `Enter` to save.  

## **Step 7 - Run the Server Again**  
```bash
java -Xmx2G -Xms2G -jar minecraft_server.jar nogui
```

## **Step 8 - Join the Server**  
1. Open **PojavLauncher**.  
2. Click **Multiplayer** → **Add Server**.  
3. Set the **Server Name** as you like and the **IP Address** as `localhost`.  
4. Click **Add** and **Join**! 🎮  

---

### **⚠️ Note**  
This setup is for **local servers only**. It **does not** include port forwarding or online access for friends.  

Enjoy your Minecraft server! 🚀
