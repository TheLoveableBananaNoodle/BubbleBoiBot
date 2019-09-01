# BubbleBoiBot
This bot is a remake of a bot created by alekxeyuk that adds an easier command line interfact, the ability to easily run eighteen bots at the same time and adds an easier spam configuration.
# How to install the bot:
1. Download Python 3.7.4 here: https://www.python.org/ftp/python/3.7.4/python-3.7.4.exe

2. When installing Python 3.7.4, check the, "Install to PATH", checkbox then click, "Custom installation". Check every box and leave the default save location as default (Do not click browse!)

3. On this GitHub page, click the green, "Clone or download." Buton and then click, "Download as ZIP." Then, extract the ZIP file somewhere on your computer. You will need to come to this file to run the bot, so save it somewhere rememerable.

4. Install GIT here: https://git-scm.com/download/win                                                                                      When installing GIT, just click, "Next" until you reach the, "Install" button and click it.
5. Do `windows + s` and type in the search, "Windows power shell". Right click it and then click, "Run as administrator."
6. In the windows shell, enter the following command:
```
pip install websockets aiohttp python-socketio requests git+https://www.github.com/hbldh/hitherdither Pillow google_images_download numpy
```
7. To run the bot, head to the BubblyBoiBot folder (not the ZIP, the folder you extracted) and click the `loopAll.bat` file.
# How to customize the bot (loopAll.config):
In the `loopAll.config` file (Inside the exec folder), you will find the following options: `hidden`, `delay`, `devSkip` and `startTimes`. `hidden` is set to false by default. Setting it to true will cause the bot windows to become hidden to the user outside of the task manager. Leaving it as false will set the bot windows to open minimized. `delay` sets how long the delay is between each bot starting. The default value is 1. `devSkip` simply stops any bots from running when using the `loopAll.bat` file. It is set to false by default and is only really used when testing the simple interface of the `loopAll.bat` program. Finally, `startTimes` sets how many bots will open on each of the three Skribbl.io ports (port5001, port5002, port5003) when running `loopAll.bat`. The default is 6. From testing, it appears the maximum is also six bots per port (Meaning at optimal time and without any errors, you can run up to eighteen bots on one computer).

# How to customize the bot (BubblyBoiBot.py):
Line 16: `SETTINGS = {'port': '5001', 'join': '', 'language': 'English', 'x': 3, 'y': 4, 'shuffle': True}`                                 `'port': 'x'` This can be used to determine whether the bot runs on port5001, 5002 or 5003 when not being ran from any of the .bat files. `'join': ''` Put a private game key (the string of characters after the `?` in the game link) to join a private game. Test each port!
`'language': 'x'` You can set which language servers the bot will join here (i.e English will join the English servers).
`'x': 'num', 'y': 'num'` I have no idea what this does. Don't touch it unless you know what you're doing.
`shuffle: x` I'd suggest leaving this to True.

Line 56: `arguments = {"keywords": "dick", "limit":10, "print_urls":False, 'no_download':True, 'safe_search':True, 'exact_size':'355,294', 'type': 'photo', 'format': 'jpg'}`                                                                               `"keywords": "dick"` Dick is the default value. This is what word(|s) the bot will search for in google images to draw.                 `"limit:10"` You can leave this as 10.
`"print_urls"` You can leage this as False.
`"no_download": x` Set to True by default, determines whether your image will be downloaded to a folder within the project.
`'safe_search': x` Will safe search by on when the bot searches for keyword specified in `"keywords": "x"`.
`'exact_size': 'w','h'` What exact size of image will the bot search for on Google Images using the keyword in `"keywords: "x"`.
`'type': 'x'` What type of picture will the bot search for on Google Images. I'd reccomend `'type': 'clipart'`. Default is photo.
`'format': 'x'` I'd suggest leaving this as jpg.

Line
