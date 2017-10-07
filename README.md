# Selfbot
This is a simple discord Nano selfbot, written in Java using the [JDA]

## Features
* Manage your personal to-do list!
* `me` command for showing when you are doing an action
* Make fancy embedded messages
* Do quick google searches
* Make reaction-based polls quickly and easily
* Show users' or servers' avatars/icons
* Share what time it is for you
* See larger versions of (and find the server-of-origin) of custom emotes
* Quote other users' messages (from any channel)
* Cleanup your own messages if you realize you were spamming
* Set your Discord game (Playing ...)
* Use "custom emojis"; when you type :emojiname: your preset text will automatically be edited in
* Make evaluations in Nashorn (javascript) using JDA methods
* Many more features coming soon

## Requirements
* JDK1.8

## Setup

1. **Download the latest release.

2. **Find your User Token.** In browser or desktop Discord, type `Ctrl-Shift-I`. Go to the Application section, and and go to **Storage** > **LocalStorage** > **discordapp.com**. Find the `token` row, and your token will be the value in quotes. ⚠ **Do not share this token with anyone** ⚠ This token provides complete access to your Discord account, so never share it!

3. **Create or edit config.txt.** If you didn't download the template, create a new file called `config.txt` in the same directory as `JSelfBot.jar`. On the first line, paste your user token (_without_ the quotation marks). On the second line, type the prefix you want to use (for example, if you put `self.` on this line, the help command would be `self.help`)
Example config.txt:
```
token=Mfa.sjaslkkngejfnesjkaNiCETokeNBrosdhsajshfjkjlajf
prefix=self.
timezone=GMT+4
status=IDLE
```

4. **You don't need to do anything with the emojis.json or todo.json file.** This file gets automatically loaded at start, and saved when you make edits to your emoji list with the `set` and `delete` commands. 

5. **Run the selfbot** If you're on Windows, you can just double-click `run.bat`. On Mac, double-click `run.command`. Otherwise... you'll want to do this via Command Line or Terminal. On most operating systems, you can right click in a directory (sometimes you need to hold shift) and click to open a Command Prompt or Terminal. If your operating system doesn't support this, just open a command line program of some sort and navigate to the selfbot directory (if you don't know how to do this, there are plenty of tutorials online). Once in the directoy, run with `java -jar JSelfBot.jar`
