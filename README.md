# spdl
yt-dlp batch file for https://southparkstudios.com

## What it does
Downloads all the South Park episodes directly from Viacom's servers.

## How to use it
### BEFORE YOU DO ANYTHING
You need to live in anywhere that lets you visit https://southparkstudios.com. If it redirects you to https://southpark.cc.com, you'll need to use a VPN to anywhere in the EU or, if you live in North America, "Canada, buddy!" (Rule of thumb: Closest to you.)

### Now that we're done with that...
First, you'll need to put [yt-dlp.exe](https://github.com/yt-dlp/yt-dlp) and [ffmpeg.exe](https://www.gyan.dev/ffmpeg/builds/ffmpeg-release-full.7z) in the same folder as the batch file. Then, open cmd. Type in: `yt-dlp --batch-file batch.txt --concat-playlist always --concurrent-fragments 20`. Let it do it's thing (this will take a while).

In the meantime, any episodes that are clearly labeled (ex: "The New Terrance and Phillip Movie Trailer [NA].mp4") can be played with your media player of choice. Do not play episodes labeled weirdly (ex: "South Park _ The New Terrance and Phillip Movie Trailer _ E 0604 _ HDSS0604X eng _ Version - 423310 _ Comedy Central S1 [5be2e22a-03ea-4f38-886c-2e599aa1e961].mp4"). They are not finished downloading, and playing them could mess up the process when they are done.

## Errors during use
### Episodes still weirdly labeled
Press Ctrl+C to stop the program (if applicable), delete all the bad files, then edit the batch.txt to remove the episodes you already downloaded. Run it again.
### `ERROR: RTMP download detected but "rtmpdump" could not be run. Please install`
(also known as `ERROR: rtmpdump exited with code 1`)
This is a server issue. Press Ctrl+C to stop the program (if applicable), delete the weirdly labeled files, edit the batch.txt to remove already downloaded episodes, then retry again in 15 minutes.
### `ERROR: The files have different streams/codecs and cannot be concatenated. Either select different formats or --recode-video them to a common format`
The files are corrupted. Press Ctrl+C to stop the program (if applicable), delete all the weirdly labeled files, then edit the batch.txt to remove already downloaded episodes. Run it again.
### 403: Forbidden errors (or similar)
Remove the `--concurrent-fragments 20` line when starting up. Note that this will make downloading the entire show take from 2 hours at most to DAYS. Only do this if you have to.

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

as those are not available on the Viacom servers publicly, for reasons I can't list on a GitHub repo (hint: politics). Most of those can be downloaded via https://southparkuncensored.com, or your local you-know site.

Subtitles are not downloaded, because that's a giant mess to deal with. If you can figure it out, you can make a pull request and i'll credit you here.

## Downloading specific episodes
You can delete lines of the batch.txt file to only download the episodes/seasons you want, then run the same command again.

## Sorting episodes after downloading
good luck

## who cares
This is for educational purposes only. All data on this repository is publicly available, directly from their sources.
