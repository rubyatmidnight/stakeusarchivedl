# stakeusarchivedl
stake.us Game Archive Downloader Tool


This is a javascript tool for use with less tediously downloading your personal game archives from stake.us.
This tool may be usable with .com as well, if you just change the instance of '.us' with '.com' in the code, which should not be hard to do.


# Instructions

Open to your game archive: https://stake.us/transactions/archive

Open the console. It may give you a warning, and you should read it and be sure you want to run this script, do not run js scripts haphazardly through important websites.

Paste the code in to the console. (you do not need to download the js file, only paste the code from https://github.com/rubyatmidnight/stakeusarchivedl/blob/main/usarchivedl.js

![image](https://github.com/user-attachments/assets/c16afdfd-61d1-412d-82b8-d0621ad7f08f)

Click 'run'.
Clear the console, and then type: `startDownloader()`. It will start from the most recent archive, and go down, and then through each page until it reaches the end.

For active users, this may take some time. The script is designed to not be aggressive against the website and shouldn't be detected as a bot, or ddosing, or anything like that. I have tested it and it downloaded everything fine.

Each archive has a cooldown of about 1 second between requests, and each page is turned in 2 seconds, so on average, each page takes about 12 seconds- A month should take around half a minute, then. So it should be about 20 minutes for the most active user. 

However, you don't have to do anything while this is going, and can safely leave it on another window or in the background. 

If for some reason you want to stop it and don't want to close your browser, type `stopDownloader()` in the same way, and click run again.

It will download each file, and name each one its respective date, rather than the archive ID. 

It will put them into the downloads folder. 

# URL Downloader Tool

This version of the tool ONLY downloads the respective urls that the archives will come from. This is useful if you just want to mass download them later.

As long as you have the URLs, you don't need cookie authorization, so be careful who you give everything to if you don't want them to have your bet archive data. The only personal information within these files, as far as I understand, is the IP of the bet location. 

# Information about the bet archives

These come in json files and some are extremely long, and need to be parsed more easily using a json formatter or some filtering tool. 

[As an example, you could do something like this, where you find all of the dragon tower results from the file, and summarize them more elegantly.](https://github.com/rubyatmidnight/provably/blob/main/dragontowerjsonextract.py)


- rubyatmidnight

If I saved you a few minutes (time is money), consider donating, but this is never required: 

ltc: LW3s8qAXRcwWNP3DJ96kCrkm3sHBRMzpWu

disclaimer: yeah i had ai do some of it hehe
