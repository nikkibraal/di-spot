# Di-Spot 🎼

A Music Discord Bot, that plays *Youtube*, *Spotify*, *Deezer* links or raw queries. Di-Spot is currently a verified by Discord app, Wanna make your own? 
Just follow the instructions and use it in your own way, executing it in your own machine or hosting in others machines to work 24/7.

Di-Spot uses multiprocessing and asynchronous Python modules to maximize Music Player response time, so the player. 
So it isn't suppose to lag when many commands are being processed.
Able to play in multiples discord serves at the same time without affecting the response time.

<img width="447" alt="Di-Spot - Official App" src="https://github.com/user-attachments/assets/1842c3f7-aa8f-4090-840e-46201efa2f21" />

# Music 🎧

- Play musics from Youtube, Spotify and Deezer links (Albums, Artists, Playlists and Tracks).
- Play musics in multiple discord server at the same time.
- The player contains buttons to shortcut some commands. 
- Support for the new Discord Slash commands.
- Search for all musics in Queue using buttons.
- Shortcut the playing of one song using dropdown menu.
- Manage the volume of the songs.
- Manage the loop of one or all playing musics.
- Manage the order and remove musics from the queue.
- Shuffle the musics queue order.
- Automatically clean the sended messages so it doesn't fill up your server.


Setting up for yourself?

Requirements

For our newest release place follow the text below:

Installation of ``Python 3.12`` and the dependencies in the requirements.txt file, creation of your own Bot in Discord and Spotify Keys. <br>
To install the dependencies type this command in the terminal, in the project root folder.

```
pip install -r requirements.txt

```

🔑 API Keys

You have to create your own discord Bot and store your Bot Token 
* Your Discord Application - [Discord](https://discord.com/developers)
* You own Spotify Keys - [Spotify](https://developer.spotify.com/dashboard/applications)

   - This information must be stored in an .env file, explained further.


Installation of FFMPEG

FFMPEG is a module that will be used to play music, you must have this configured in your machine
*FFMPEG must be configured in the PATH for Windows users. Check this [YoutubeVideo](https://www.youtube.com/watch?v=r1AtmY-RMyQ&t=114s&ab_channel=TroubleChute).* <br><br>
You can download the executables in this link `https://www.ffmpeg.org/download.html` and then put the .exe files inside a ffmpeg\bin folder in your C:\ folder. Do not forget to add 'ffmpeg\bin' to your PATH.


.Env File Example

This is an example of how your .env file (located in root) should look like.

```env
BOT_TOKEN=Your_Own_Bot_Token
SPOTIFY_ID=Your_Own_Spotify_ID
SPOTIFY_SECRET=Your_Own_Spotify_Secret
BOT_PREFIX=Your_Wanted_Prefix_For_Di-Spot
SHOULD_AUTO_DISCONNECT_WHEN_ALONE=True #all settings can be set like this
#etc... All settings can be set this way
```

⚙️ Configs

The bot's configuration is stored in the [.env](.env) file, you can change the prefix and the bot token there, as well as all the other configurations.
Take a look in the [Settings page](.github/Docs/SETTINGS.md) to personalize the Bot for you.


Initialization

- Go to [Discord](https://discord.com/developers) and invite your Bot to your own server
- Run ```python main.py``` in console to start
- Give this project a nice 🌟


🐳 Docker

You can also run this project in a Docker container. You can find the instructions to run this project in a Docker container in the [Docker Instructions](.github/Docs/DOCKER.md) page.


🚀 Sparked Host

> Sparked Host is one of the best hosts out there, we use it ourselves for multiple projects. If you wish to run your Discord Bot 24/7, I recommend checking out their Discord Bot Hosting plans* <br>

They also have a variety of other hosting services. Also, offer custom domain names + for your server, dedicated IP addresses.  

Check them out at the following website: https://sparkedhost.com/

🧪 Tests

The tests were written manually with no package due to problems with async function in other packages, to execute them type in root: <br>
`python run_tests.py`<br>
