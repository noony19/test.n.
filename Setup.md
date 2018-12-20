## `1.` Install Java JDK 1.8
* [Java JDK 1.8](https://www.google.com/#q=download+jdk+8) (not OpenJDK)
* Instructions on how to install JDK 8 on your system: [[Installing-JDK1.8]]

## `2️.` Download JMusicBot
* Download the latest **JMusicBot-X.Y.Z.jar** (and optionally, example **config.txt** file) from the [releases](https://github.com/jagrosh/MusicBot/releases/latest) page (or, get the URL from the releases page and then use wget or similar command-line tool to download).
* Your folder should look like this (on desktop):  
![View](http://i.imgur.com/14x9uDy.png)
* Do not put this in the 'Downloads' or 'Desktop'. Use a folder within 'Documents'

## `3.` Edit the config file
* Fill in the config file (if you downloaded it). If you didn't download it, you will be prompted when you run for the first time. An example `config.txt` is provided below (See [[Getting a Bot Token]] and [[Finding Your User ID]] if you need help with the config).  
```
token=MJHJkljflksdjfCoolTokenDudeILikeItkasdk
owner=113156185389092864
prefix="!"
```

## `4.` Run JMusicBot
* Double-click the jar file, or run `java -Dnogui=true -jar JMusicBot-X.Y.Z.jar` from the command line. (replace X, Y, and Z with the release numbers)
* Provide the requested information, if prompted.
* Wait for the "Finished Loading" message.

## `5.` Add your bot to your server
* When the bot starts, if it hasn't been added to any servers yet, it will provide you with a link in the console.
* Alternatively, follow these instructions (with images): [[Adding Your Bot To Your Server]]