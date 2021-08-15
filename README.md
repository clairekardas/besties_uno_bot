# Besties Uno Bot 🌈

[![forthebadge](https://raw.githubusercontent.com/clairekardas/besties_uno_bot/master/images/readme/draw-two-no-u.svg)](https://forthebadge.com/)
[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg?style=flat-square)](./LICENSE)

<img src="https://raw.githubusercontent.com/clairekardas/besties_uno_bot/master/images/readme/logo-small.png">

Telegram Bot that allows you to play UNO via inline queries. The bot runs as [@besties_uno_bot](http://telegram.me/besties_uno_bot) and is based on https://github.com/jh0ker/mau_mau_bot 😋

It's made by besties, for besties, featuring pride flag cards and slang text 🏳️‍🌈 

To run the bot yourself, you will need: 
- Python (tested with 3.4+) 🐍
- The [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot) module 💻
- [Pony ORM](https://ponyorm.com/) 🦄
- Lots of patience ⏳
- Pizza 🍕

This version of the bot is still under devlopment 👩‍💻

## Setup
- Get a bot token from [@BotFather](http://telegram.me/BotFather) and change configurations in `config.json`.
- Convert all language files from `.po` files to `.mo` by executing the bash script `compile.sh` located in the `locales` folder.
  Another option is: `find . -maxdepth 2 -type d -name 'LC_MESSAGES' -exec bash -c 'msgfmt {}/unobot.po -o {}/unobot.mo' \;`.
- Use `/setinline` and `/setinlinefeedback` with BotFather for your bot.
- Use `/setcommands` and submit the list of commands in commandlist.txt
- Install requirements (using a `virtualenv` is recommended): `pip install -r requirements.txt`

You can change some gameplay parameters like turn times, minimum amount of players and default gamemode in `config.json`.
Current gamemodes available: classic, fast and wild. Check the details with the `/modes` command.

Then run the bot with `python3 bot.py`.

Code documentation is minimal but there.
