# Requirements
* Windows (or, install ffmpeg and ffprobe on operating system of your choice)
* [Java JDK 1.8](https://www.google.com/#q=download+jdk+8)
* [Python 2.7+](https://www.python.org/downloads/) (must be on [PATH](https://www.google.com/search?q=add+python+to+system+path))

# Downloads
Download the latest jar (and optionally, example config file) from the [releases](https://github.com/jagrosh/MusicBot/releases) page.

# Setup
1. Download the jar file (and the config, optional) from the [releases](https://github.com/jagrosh/MusicBot/releases) page.
2. Fill in the config file (if you downloaded it). If you didn't download it, you will be prompted when you run for the first time. An example config is provided below:
```
token=MJHJkljflksdjfCoolTokenDudeILikeItkasdk
owner=113156185389092864
prefix=!
```
See [[Getting a Bot Token]] and [[Finding Your User ID]] if you need help with the config.
3. Double-click the jar file, or run `java -jar JMusicBot-X.Y.Z.jar -nogui` from the command line. (replace X, Y, and Z with the release numbers)
4. Provide the requested information, if prompted.
5. Wait for the "Finished Loading" message.
6. Add the bot to your server. From the [bot application page](https://discordapp.com/developers/applications/me) (where you got the token), find the Client ID and insert it in this link, replacing APP_ID: `​https://discordapp.com/oauth2/authorize?client_id=APP_ID&scope=bot`