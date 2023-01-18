# Music bot
Credit to [Pawel Bes](https://github.com/pawel02)
Code Edited By [Riyadh Alzahrani](https://github.com/RiyadhAlzahrani)

Since a lot of discord music bots are being blocked by youtube nowadays I've decided to write up a quick project that will allow anyone to host their own discord bot. This bot includes the following commands:

* `/help` - displays all the available commands
* `/p "keywords"` - finds the song on youtube and plays it in your current channel. Will resume playing the current song if it was paused
* `/q` - displays the current music queue
* `/skip` - skips the current song being played
* `/clear` - Stops the music and clears the queue
* `/leave` - Disconnected the bot from the voice channel
* `/pause` - pauses the current song being played or resumes if already paused
* `/resume` - resumes playing the current song


# Installation
To run the discord bot all you need is `python 3.4` or above.\
install dependencies of the python that are needed for the bot.\
  \
youtube_dl:
  ```md
  pip install youtube_dl
  ```

ffmpeg:
  ```md
  pip install ffmpeg
  ```

PyNaCl:
  ```md
  pip install PyNaCl
  ```
>Please note that you will need to have [ffmpeg](https://ffmpeg.org/download.html) installed and make sure that the path to the bin folder is in your environment variables. 

# Token
Add your Bot Token by going to the [DEVELOPER PORTAL](https://discord.com/developers/applications/) then...
  1. Login by using your discord account.
  2. Create New Application .
  3. Go to Bot then Add Bot .
  4. Reset Token then Copy the new Token the Paste it in the File Token in the Bot folder .
  5. Go to Privileged Gateway Intents and Enable `PRESENCE INTENT` , `SERVER MEMBERS INTENT` , `MESSAGE CONTENT INTENT` .
  6. You are done installion .

# Invite to Discord Server
  1. To invite the Bot to ur server go to `OAuth2` -> `URL Generator`.
  2. Set the `SCOPES" to "Bot`.
  3. Set the `BOT PERMISSIONS` what ever the Bot Needs or just set it to `Administrator`.
  4. Copy the `GENERATED URL` the Paset it in the Browser then Invite your Bot like any other Bot.

# Creating a bot
To create a bot follow Pawel Bes [tutorial](https://www.youtube.com/watch?v=PJDuI9n7rWE&t=325s&ab_channel=Computeshorts). 
  >This will guide on how to create a bot.

# Deploying your bot
Lastly you'll need to deploy your bot. 
Navgate to the Bot Folder in the `CMD` then...
  ```md
python main.py
  ```

or just open the folder in Visual Studio Code Then `Run` the main.py file or `Run and Debug` the `main.py` file

>You can follow Pawel Bes other [tutorial](https://www.youtube.com/watch?v=z58g7_dHeMA) on deploying with docker 
  >the gist is to have a server setup with all the dependencies and then run `python main.py`.
