# NSTC MOVIE FINDER

## Added Features

<br/>
<br/>
<a target="_blank">
  <img align="right" height="400" width="400" alt="NSCTMOVIEFINDER" src="https://telegra.ph/file/9bca5220bb6be74d8abd6.jpg">
</a>

- Custom captions for your files.
- Index command to index all the files in a given channel.
- Ability to Index Public Channels without being admin.
- Support Auto-Filter (Both in PM and in Groups)
- Once files saved in Database , exists until you manually deletes.
- Added Force subscribe (Only channel subscribes can use the bot)
- Ability to restrict groups(AUTH_GROUPS)

<br/>
<br/>

## Installation

### Easy Way
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/hirendra4455/NSTC-Movie-Finder)

### Hard Way

```bash
#Cloning Source
git clone https://github.com/TharukRenuja/NSTC-Movie-Finder.git

# Create virtual environment
python3 -m venv env

# Activate virtual environment
env\Scripts\activate.bat # For Windows
source env/bin/activate # For Linux or MacOS

# Install Packages
pip3 install -r requirements.txt

# Edit info.py with variables as given below then run bot
python3 bot.py
```
Check [`info.py`](info.py) file & add your varibles.

## Variables

### Required Variables
* `BOT_TOKEN`: Create a bot using [@BotFather](https://telegram.dog/BotFather), and get the Telegram API token.
* `API_ID`: Get this value from [telegram.org](https://my.telegram.org/apps)
* `API_HASH`: Get this value from [telegram.org](https://my.telegram.org/apps)
* `CHANNELS`: Username or ID of channel or group. Separate multiple IDs by space
* `ADMINS`: Username or ID of Admin. Separate multiple Admins by space
* `DATABASE_URI`: [mongoDB](https://www.mongodb.com) URI. Get this value from [mongoDB](https://www.mongodb.com).
* `DATABASE_NAME`: Name of the database in [mongoDB](https://www.mongodb.com).

### Optional Variables
* `OMDB_API_KEY`: OMBD_API_KEY to generate imdb poster for filter results.Get it from [omdbapi.com](http://www.omdbapi.com/apikey.aspx)
* `CUSTOM_FILE_CAPTION` : A custom caption for your files. You can format it with file_name, file_size, file_caption.(supports html formating)
Example: `<b>Join [SLBotsOfficial](https://t.me/SLBotsOfficial) for more useful bots</b>\n\n<code>{file_name}</code>\nSize{file_size}\n{file_caption}.`
* `AUTH_GROUPS` : ID of groups which bot should work as autofilter, bot can only work in thease groups. If not given , bot can be used in any group.
* `COLLECTION_NAME`: Name of the collections. Defaults to Telegram_files. If you going to use same database, then use different collection name for each bot
* `CACHE_TIME`: The maximum amount of time in seconds that the result of the inline query may be cached on the server
* `USE_CAPTION_FILTER`: Whether bot should use captions to improve search results. (True/False)
* `AUTH_USERS`: Username or ID of users to give access of inline search. Separate multiple users by space. Leave it empty if you don't want to restrict bot usage.
* `AUTH_CHANNEL`: ID of channel. Without subscribing this channel users cannot use bot.
* `START_MSG`: Welcome message for start command.

## Note
* Currently [API used](http://www.omdbapi.com) here is allowing 1000 requests per day. Once a poster is fetched from OMDB , poster is saved to DB to reduce duplicate requests.

## Admin commands
```
channel - Get basic infomation about channels
total - Show total of saved files
delete - Delete file from database
index - Index all files from channel.
logger - Get log file
```

## Tips
* You can use `|` to separate query and file type while searching for specific type of file. For example: `Avengers | video`
* If you don't want to create a channel or group, use your chat ID / username as the channel ID. When you send a file to a bot, it will be saved in the database.


## Support
Contact Me On [Telegram](https://t.me/TharukRenuja)

[Bots Updates](https://t.me/SLBotsOfficial)
[Movie Updates](https://t.me/nstcentertainment)
[Movie Request Group](https://t.me/nstcentertainmentgroup)
[Movie Request New Group](https://t.me/genuinemovieclub)

## License
Code released under [The GNU General Public License](LICENSE).
```
Made with Python3
(C) @TharukRenuja
Copyright permission under GNU Public License
License -> https://github.com/TharukRenuja/NSTC-Movie-Finder/blob/main/LICENSE
```

### Credits

- [TR-TECH-GUIDE](https://github.com/TR-TECH-GUIDE)
- [SUBIN](https://github.com/subinps)
- [Mahesh](https://github.com/Mahesh0253) for Media Search Bot.
- [TrojanzHex](https://github.com/TroJanzHEX) for Auto Filter Bot.
- [Me](https://github.com/TharukRenuja) for Nothing🤣.
