### **As of release 0.1.3, the Linux jar includes the necessary natives for Raspberry Pi. You can download the latest release [here](https://github.com/jagrosh/MusicBot/releases/latest).** You no longer need to follow these steps.


> If you plan to run this bot on a raspberry pi, there are a few additional steps you will need to take. The default build does not include some required native files for raspberry pi due to filesize concerns (it's already big enough as it is!). Therefore, it is highly recommended that you complete these steps for each release you use. (Also, if you need to install JDK 1.8, please read [[Installing-JDK1.8]]).

> 1. Download **[libconnector.so](https://cdn.discordapp.com/attachments/154460214769221632/414242970540441620/libconnector.so)**

> 2. Download the required files from the **[latest release](https://github.com/jagrosh/MusicBot/releases/latest)**

> 3. Using [WinRAR](http://www.rarlab.com/download.htm) (or some other archiving tool), open up the JMusicBot-X.Y.Z.jar. It should look similar to this:<br>
> ![jarfiles](http://i.imgur.com/aWrWv0i.png)

> 4. Navigate to `/natives/linux-arm/`. Inside should be a single `libopus.so`

> 5. Insert the `libconnector.so` file from step one into this same folder. It should appear like this:<br>
> ![newfile](http://i.imgur.com/SiNXFC3.png)

> 6. Close WinRAR (or whatever tool you used). Your `.jar` file is now ready! Simply continue following the instructions from the [[Setup]] page!