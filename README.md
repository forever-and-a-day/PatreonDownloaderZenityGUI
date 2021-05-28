# PatreonDownloaderZenityGUI
A kinda bad bash script that uses Zenity to make a GUI for patreondownloader. WIP.
Designed to be a quick and dirty frontend for [PatreonDownloader](https://github.com/AlexCSDev/PatreonDownloader) (linux ver ofc) 
Thought I could do it in an hour, that was a lie given my small knowledge of bash scripting haha
It's my first real script I've made that actually does something I want (kinda) and I'm proud of it, plz don't laugh

![Screenshot](https://files.catbox.moe/it4pyc.png)

## Features 
* Downloads content from 2 hardcoded preset creators that I like
* Currently set to download absolutely everything, nice™
* Is supposed to accept custom creator URLS, does not fully work (downloads but reports invalid URL every time)
* Gives you a nice lil notification when it's done (only works for presets atm, tested on Cinnamon DE but should work with anything gnome-like)
* Prints "Done" in the terminal when it's done, like a good boy
* Archiving patreon posts not user-friendly or fast enough? Don't copy and paste commands with included urls from a text file and watch the script run in the terminal like a caveman - just double click, hit run, you're done (not quite but it rhymes) 
* I spent 5 hours automating a task that usually takes 8 min at most, and it's still broken
* I love you and you have worth <3
* This bash script loves you too <3

## Supported URL Format
`https://www.patreon.com/creatornamehere/posts`

## How to install
0. Install google chrome if not already installed
1. Download and unzip patreondownloader linux version from [here](https://github.com/AlexCSDev/PatreonDownloader/releases)
2. Extract zip to a folder just for it
3. Download downloadergui script from this repo
4. Fix it for me and submit pull request - haha, just kidding, unless... 👀
5. drop script into the same folder as PatreonDownloader.App
6. Make sure both PatreonDownloader.App and downloadergui are executable (use `chmod +x filename` or in Nemo right click, Properties, "Permissions" Tab, then check "Allow executing file as program") 
7. Run, choose preset or Other, sign in real quick before PatreonDownloader times out, and enjoy

## Troubleshooting / faq
**"How to change save location?"**
Change hardcoded download commands to specify location (idk how too lazy) or create a symlink in Nemo (Mint) or Nautilus (Ubuntu/other gnome) by creating a folder with your creator's name in lowercase in destination (or moving existing), then holding ctrl+shift and dragging the "link folder" into the "download" folder in PatreonDownloader's root directory. You know you've succeeded when you see some sort of arrow icon on the creator's folder in "download". 

**"The weird Chrome window closed before I could sign in! What do?"**
Re-run and try again. PatreonDownloader is wonky and will snap its jaws shut on the sign in browser real quick, but once you're real quick-er than it and manage to sign in, you won't have to do that again unless you change your password, in which case I recommend backing up your downloads elsewhere, deleting the patreondownloader install folder, and getting a new one from it's github repo. Also try deleting any strange new profiles that appear in chrome profile switcher before running a fresh install. 

**"The downloader GUI gives me errors when I try to use the custom url download feature. Help!"**
I'm working on this one - don't fret though, it still downloads, the script just can't read the console output properly to determine if it works and gives you a scary error instead of a friendly notification :( As a temporary workaround, consider adding your desired creator's url to an additional preset by modifying or copying my hardcoded presets. 
