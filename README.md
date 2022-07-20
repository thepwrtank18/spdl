# spdl
yt-dlp batch file for https://southparkstudios.com

## What it does
Downloads all the South Park episodes directly from Viacom's servers.

## How to use it
### BEFORE YOU DO ANYTHING
You need to live in anywhere that lets you visit https://southparkstudios.com. If it redirects you to https://southpark.cc.com, you'll need to use a VPN to anywhere in the EU or Canada.

### Now that we're done with that...
First, you'll need to put [yt-dlp.exe](https://github.com/yt-dlp/yt-dlp) and [ffmpeg.exe](https://www.gyan.dev/ffmpeg/builds/ffmpeg-release-full.7z) in the same folder as the batch file. Then, open cmd. Type in: `yt-dlp --batch-file batch.txt --concat-playlist always`. Let it do it's thing (this will take a while).

In the meantime, any episodes that are clearly labeled (ex: "Make Love, Not Warcraft [NA].mp4") can be played with your media player of choice. Do not play episodes labeled weirdly (ex: "South Park _ The New Terrance and Phillip Movie Trailer _ E 0604 _ HDSS0604X eng _ Version - 423310 _ Comedy Central S1 [5be2e22a-03ea-4f38-886c-2e599aa1e961].mp4"). They are not finished downloading, and playing them could mess up the process when they are done.

## What it can't do
It **cannot** download:
1. Super Best Friends
2. The Biggest Douche In The Universe
3. Best Friends Forever
4. Cartoon Wars (parts 1 and 2)
5. 200 and 201
6. Insheeption
7. Bigger, Longer and Uncut
8. All Paramount+ specials

as those are not available on the Viacom servers publicly.

Subtitles are not downloaded, because that's a giant mess to deal with. If you can figure it out, you can make a pull request and i'll credit you here.
