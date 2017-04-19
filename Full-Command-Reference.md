This page contains the full list of commands. These commands (and descriptions) can also be seen via the `help` command.

### General Commands
These commands are just general-use commands to see information about the bot

**`about`** - shows basic information about the bot, including its library, framework, and some statistics

**`ping`** - shows the latency between the bot and Discord. In general, 80-250ms is a normal value.

**`settings`** - shows the settings for the current server. This includes Text Channel, Voice Channel, DJ Role, and Default Playlist. This command also shows the number of servers the bot is on, and how many audio connections there currently are.

### Music Commands
These commands are related to playing music, available to all users. If a TextChannel is set, these commands can only be used in that channel. 

**`nowplaying`** (or `np` or `current`) - shows information about the song that is currently playing (name, user that added it, current timestamp, and song URL)

**`play <URL>`** - plays the song or stream at the provided URL. Supported locations include (but are not limited to): YouTube (and playlists), SoundCloud, BandCamp, Vimeo, and Twitch. Local files or URLs of the following formats are also supported: MP3, FLAC, WAV, Matroska/WebM (AAC, Opus or Vorbis codecs), MP4/M4A (AAC codec), OGG streams (Opus, Vorbis and FLAC codecs), AAC streams, Stream playlists (M3U and PLS)

**`play <song name>`** - plays the top YouTube result for the specified song name

**`play playlist <playlistname>`** (or `play pl <playlistname>`) - plays all songs in the specified playlist. There must already be a playlist of the specified name in the Playlists folder

**`playlists`** - shows available playlists. These playlists must be inside the Playlists folder.

**`queue [pagenum]`** (or `list [pagenum]`) - shows songs in the queue. If no page number is provided, it defaults to the first page.

**`remove <songnum>`** (or `delete <songnum>`) - removes the song at the provided position in the queue. You can only remove songs that you added, unless you are an Admin or have the specified DJ role.

**`remove all`** (or `delete all`) - removes all songs that you have added to the queue

**`search <query>`** - shows the top YouTube results for a search and allows you to select one to add to the queue

**`scsearch <query>`** - shows the top SoundCloud results for a search and allows you to select one to add to the queue

**`shuffle`** - shuffles (changes the order, randomly) of songs that you have added to the queue

**`skip`** (or `voteskip`) - skips a song if you added it. If you didn't add it, it adds your vote to skip it. Approximately 60% of active listeners need to vote to skip a song for it to be skipped.

### DJ Commands
All Admins can automatically use DJ commands. Admins can also assign one server role to be the "DJ role," which allows anyone with that role to use these commands as well.

**`forceskip`** - forcibly skips the current song, regardless of who added it and how many votes there are to skip it

**`skipto <position>`** - skips forward in the queue to the provided song number, playing that song and removing any songs before that from the queue

**`stop`** - clears the queue, ends the current song, and leaves the voice channel

**`volume [0-150]`** (or `vol [0-150]`) - shows or sets the current volume. For best performance, it is recommended to leave this at 100 and adjust volume on an individual basis within Discord

### Admin Commands
Admin commands can be used by anyone with the Manage Server permission.

**`setdj <rolename>`** - sets the DJ role. Users with this role will be able to use DJ commands.

**`setdj none`** - clears the DJ role. Only Admins will be able to use the DJ commands.

**`settc <channel>`** - sets the text channel for music commands. Using music commands in other channels will result in them being deleted (if possible), and a warning sent via DMs to use the correct channel. Additionally, if the bot has the Manage Channel permission in the set channel, it will adjust the topic to show the current track.

**`settc none`** - clears the text channel

**`setvc <channel>`** - sets the voice channel for playing music. When set, the bot will only connect to the specified channel when users attempt to play music.

**`setvc none`** - clears the voice channel for playing music. This means that users can play music from any channel that the bot can connect to (if the bot is not already in a different channel)

### Owner Commands
These commands can only be used by the bot owner (set in the config)

**`playlist append <playlistname> <item> | [item] | [item]...`** - adds items to an existing playlist. Items must be urls. To add a YouTube search, it must be in the form "ytsearch:query". For a SoundCloud search, use "scsearch:query".

**`playlist delete <playlistname>`** - deletes the playlist file for a playlist

**`playlist make <playlistname>`** - creates a new, empty playlist

**`playlist setdefault <playlistname>`** - sets the default playlist for the server, which plays when the queue is empty and when the bot starts up

**`playlist setdefault none`** - clears the default playlist

**`setavatar <url>`** - sets the avatar of the bot

**`setgame [game]`** - sets the game the bot is playing

**`setname <name>`** - sets the username of the bot

**`shutdown`** - safely shuts down