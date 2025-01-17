<p align="center">
  <a href="https://github.com/larafe1/saturn-bot">
    <img src="https://github.com/larafe1/saturn-bot/blob/master/.github/saturn-logo.png">
  </a>
</p>

<p align="center">
  <a href="https://github.com/larafe1/saturn-bot/releases">
    <img src="https://img.shields.io/static/v1?label=version&message=4.x&color=5965E0&labelColor=121214" alt="Version">
  </a>
  <a href="https://www.typescriptlang.org/">
    <img src="https://img.shields.io/static/v1?label=built%20with&message=TypeScript&color=5965E0&labelColor=121214" alt="TypeScript">
  </a>
  <a href="https://nodejs.org/en/">
    <img src="https://img.shields.io/static/v1?label=built%20with&message=Node.js&color=5965E0&labelColor=121214" alt="Node.js">
  </a>
  <a href="https://github.com/discordjs/discord.js/">
    <img src="https://img.shields.io/static/v1?label=built%20with&message=Discord.js&color=5965E0&labelColor=121214" alt="Discord.js">
  </a>
  <a href="https://github.com/larafe1/saturn-bot/blob/master/LICENSE">
    <img src="https://img.shields.io/static/v1?label=license&message=GPL-v3.0&color=5965E0&labelColor=121214" alt="License">
  </a>
  <a href="https://github.com/larafe1/saturn-bot/actions/workflows/ci.yml">
    <img src="https://github.com/larafe1/saturn-bot/actions/workflows/ci.yml/badge.svg" alt="GitHub Actions">
  </a>
</p>

<a href="https://www.digitalocean.com/">
  <img src="https://web-platforms.sfo2.cdn.digitaloceanspaces.com/WWW/Badge%201.svg" alt="DigitalOcean Referral Badge" />
</a>

## Overview

Saturn is a modular multipurpose, user-friendly and feature-rich discord bot. Just perfect for manage your server and provide the best experience for you and your community. All of that and many more, together on the most amazing planet of our solar system!

### Bot features

- Server moderation (linked with your MongoDB database)
- Server & Members info
- Music playback (YouTube and Spotify)
- Weather report
- Reminders

### Technologies used

- [TypeScript](https://www.typescriptlang.org/)
- [Node.js](https://nodejs.org/en/)
- [Discord.js](https://github.com/discordjs/discord.js)
- [Axios](https://github.com/axios/axios)
- [Mongoose](https://github.com/Automattic/mongoose)

## How to use (MUST READ)

Saturn is a _self-hosted_ bot, this means you will need to host and maintain your own instance. For that, you can instantiate at your own machine or you can use a cloud platform to do that. A great cloud platform that I have used before and recommend is [Heroku](https://www.heroku.com/), it's a nice cloud service which offers a great compatibility for apps like this one, and also has a free plan option.

Please notice, you're **NOT** allowed to upload this bot to any service such as "discordbotlist" or "top.gg". You're only allowed to host this bot for your community.

In this step-by-step I will only cover about how you can set Saturn in your own machine. Also, notice that each topic in the next sections has a brief description in the title explaining what we're about to do. With that been said, let's move on.

### Getting started

First things first, make sure that you have `git`, `node` and `npm` installed. Then open your terminal or cmd and type the commands below.

#### Cloning this repository & Cd'ing into project's folder

```elm
git clone https://github.com/larafe1/saturn-bot.git

cd saturn-bot
```

#### Setting up everything

```elm
npm install
```

When the installation finishes, find the `.env.example` inside of the project's folder and open it with some text editor of your choice.

Now, make sure that you have your own bot token in hands — in case you don't know how to get it, go at the [Discord developers portal](https://discord.com/developers/) and create a new app.

After that, replace the `HELLO_WORLD` with your bot token and some prefix of your choice (e.g: !, +, -). When you're done, rename the `.env.example` to `.env`.

```bash
BOT_TOKEN=HELLO_WORLD
BOT_PREFIX=HELLO_WORLD
```

Now, as I mentioned before, this bot has a weather report function and also supports a MongoDB database linked to it. In case you wanna use these features, you will also need to set in the `.env` an [OpenWeather API token](https://openweathermap.org/api) and your [MongoDB database link](https://www.mongodb.com/).

To get these features working properly, your `.env` file should have this template below with your credentials settled in the `HELLO_WORLD`'s place.

```bash
BOT_TOKEN=HELLO_WORLD
DB_ACCESS=HELLO_WORLD
OPENWEATHER_TOKEN=HELLO_WORLD
BOT_PREFIX=HELLO_WORLD
```

Notice these are **EXTRA** features! If you don't wanna use them, just follow the first `.env` template introduced in this step-by-step and your bot still will work normally.

#### Running

```elm
npm run dev
```

## Final considerations

That's pretty much it, thanks for using Saturn and have fun!

Also, PRs are more than welcome, in case you wanna contribuite to this project, feel free to open a pull request with a new feature.

> **This project is licensed under a [GNU General Public License v3.0 License](https://github.com/larafe1/saturn-bot/blob/master/LICENSE)**
