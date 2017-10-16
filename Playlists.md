# Youtube Playlists
To play a youtube playlist, all you need is the `play` command. Make sure that the link you're using is a playlist link and not a video link. For example, https://www.youtube.com/watch?v=bd2B6SjMh_w&list=PLUib4KwT0DMJaPgg_nr1ia8FY5JcXksvb&index=4 is a video link (notice the `watch?v=`) and will just play the selected video. To play the whole list, either use the playlist link (**play https://www.youtube.com/playlist?list=PLUib4KwT0DMJaPgg_nr1ia8FY5JcXksvb**) or just the playlist ID (**play PLUib4KwT0DMJaPgg_nr1ia8FY5JcXksvb**)

# Local Playlists
Local playlists are .txt files found in the `Playlists` folder in the same folder as you are running the bot from. Each line of the file is a new entry, and entries can be:
* links to youtube videos, soundcloud tracks, or online files
* full or relative path to local files
* links to youtube or soundcloud playlists
* links to online streams or radio
* searches, prefixed by `ytsearch:` for a youtube search and `scsearch:` for a soundcloud search

Lines starting with `#` or `//` are ignored. To make a playlist automatically shuffle when loaded, add `#shuffle` or `//shuffle` on its own line somewhere in the playlist.

# Soundcloud Playlists
Just use the `play` command followed by the playlist link.