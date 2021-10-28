# Troubleshooting Chrome Crashes
When using PatreonDownloader, and by extension, PatreonDownloaderZenityGUI, Chrome may crash before you can log in, preventing you from downloading content. 
This guide will assist you in working around these crashes.

*Note:* This process requires a quick reaction time. Prepare yourself. 

1. Pick your desired creator in the menu, or enter a custom URL. PatreondowloaderZenityGUI will notify you that it has started downloading. DO NOT click "OK" yet. 
2. Open 📈️ **System Monitor** (preinstalled on Mint and other GNOME-like DEs) or the equivalent task manager for your distribution. 
3. Press `ctrl+f` and search for `patreon`.
4. You should now have both System Monitor and the "Download Started" window on your screen. Click "OK". A chrome window will open. 
5. As quickly as possible, right click on `PatreonDownloader.App` in System Monitor and click "Stop".
6. In the chrome window, reload the tab that is on an error page. It will be stuck loading and the login page will not appear. 
7. Open a new tab, then close the tab that wasn't loading. *Do not close the first two tabs.* 
8. In the new tab you made, go to `patreon.com` and log into your account. If the tab crashes to an error screen while you are logging in (with Google or Facebook, for example), reload it untill you see your Patreon homepage. 
9. Close the Chrome window.
10. Return to System Monitor, right click on `PatreonDownloader.App` and click "Continue". The process will remain for a moment, crash silently, then disappear. 
11. Close System Monitor, then run PatreondowloaderZenityGUI again with your desired creator. The download will complete, and future downloads should as well. 

Your session may expire occasionally and you will be logged out of patron. In the event that this occurs, follow these steps again!

[< Repository Home](https://github.com/forever-and-a-day/PatreonDownloaderZenityGUI)