# Play list Generator
Generates Playlists for your iPod or Jellyfin server.


These locally run HTML pages generate playlist files from your music archive.

To generate the files you first need to generate an extract of the metadata of your music. Your music metadata needs to be as complete as possible before you generate the extract.

To generate the extract you will need ExifTool (https://exiftool.org/) installed on your system.

Once you have ExifTool you can run the command line: exiftool -r -ext mp3 -ext flac -ext m4a -ext wav -csv "Path\to\your\MusicFiles" > "path\for\the\export\music_inventory_allMetadata.csv"

If you are in linux or MacOS replace the \ with /. 

Once you have the extract you will then need to go download the Billboard Hot 100 Archive from https://raw.githubusercontent.com/utdata/rwd-billboard-data/main/data-out/hot-100-current.csv

The playlist generator will give you a screen where you can download the entire archive of the playlist you generated or you can download individual ones as you see fit.

If you are doing this in Windows, be aware that the export uses the / character in the path and windows needs it to be \. You will need to load the playlist files in something like Notepad++ and have it replace all the / for \ in every playlist.

Once you have the files ready, you can import them into iTunes or JellyFin and your music will be ready to play.

<img src="https://github.com/LifeAtTerminalVelocity/PlaylistGenerator/blob/main/Screenshot%202026-07-30%20at%2021.07.52.png"
