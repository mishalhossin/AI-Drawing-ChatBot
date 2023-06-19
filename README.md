# Stable Diffusion Bot

![](https://img.shields.io/github/license/mak448a/Stable-Diffusion-Bot)
![](https://img.shields.io/github/contributors/mak448a/Stable-Diffusion-Bot)
![](https://img.shields.io/github/repo-size/mak448a/Stable-Diffusion-Bot)

This is an AI image generator Discord bot written in Python. It has a chatbot that uses ChatGPT!

This project uses lots of APIs. As a result, you will not need a powerful computer!

**DISCLAIMER:** ChatGPT uses your Poe account.
I am not responsible if your Poe account gets banned, since using Poe in programs is against their TOS.

![](demo.png)


## Table of Contents
1. [Features](#Features)
2. [Notes](#Notes)
3. [Prerequisites](#Prerequisites)
4. [Setup](#Setup)
5. [Configuration](#Configuration)
6. [Generate images faster with Stable Horde](#Generate-images-faster-with-Stable-Horde)


## Features
- ChatGPT chatbot that is integrated with Imaginepy
- 3 slash commands for generating images
- Stable Diffusion
- Anything Diffusion
- Pollinations


## Notes

- ChatGPT is the fastest model that you can use.
- Integrated drawing is not available for GPT4All.
- Please do not enter any personal information in the Chatbot or in the image generators,
because your prompts are sent to various providers.
- When you use Stable Horde to generate images, your prompts are sent to Stable Horde, as listed in their [privacy policy](https://stablehorde.net/privacy). 
- The chatbot may not work as expected if multiple users are chatting with it at once. 
- When using Replit, GPT4All cannot be used.
- When using Replit, you must input your .env variables in the `Secrets` button on Replit.


## Prerequisites
This project assumes that:
- Python 3.8+ is installed and is on your PATH
- Pip is installed
- Python-venv is installed (only for Debian based distros)
- Git is installed
- You know how to create a Discord Bot account
- You know JSON syntax (It's basically a Python Dictionary)


## Setup
1. Create a Discord Bot and grab the token. Make sure to switch on Message Content Intent in the `Bot` tab of the [Developer Portal](https://discord.com/developers/applications).
2. Grab an API key from Stable Horde [at their register page](https://stablehorde.net/register).
3. Rename `example.env` to `.env` and place your bot token and your API key in under `API_KEY`.
4. [Register](https://poe.com) for Poe and open inspect tool. [Find your token](https://github.com/ading2210/poe-api#finding-your-token) and place it under `POE_TOKEN` in your `.env` file.
5. Place your Discord bot token under `BOT_TOKEN`.
6. Clone the Stable Horde module:
```shell
git clone 'https://github.com/mak448a/horde_module' --depth=1
```
7. Create venv and install dependencies:

Linux or MacOS
```shell
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
Windows
```shell
python -m venv venv
venv\Scripts\activate.bat
pip install -r requirements.txt
```
8. Rename `example_config.json` to `config.json`. Edit this file however you like. See [Configuration](#Configuration).
9. Run the bot and invite it with the link it provides.
10. Type / in the message box and start messing around with the commands!


## Configuration
<details><summary>Configuring chat model</summary>
Go to <code>config.json</code> and set the key <code>"model"</code> to the model you want.

**Available Models**
- ChatGPT
- GPT4All
- text-davinci-003

You must write the model exactly as it is written here.
When using ChatGPT, you must sign up for a Poe account.

When you are done, the edited line should look like this:

<code>"model": "ChatGPT",</code>
</details>
<details><summary>Disable chatbot</summary>
Go to <code>config.json</code> and set the key <code>"chatbot"</code> to false.

It should look like this:

<code>"chatbot": false,</code>
</details>
<details><summary>Change loading GIF</summary>
Go to <code>config.json</code> and set the key <code>"loading_gif"</code> to any GIF on Tenor you want!

It should look like this:

<code>"loading_gif": "https://tenor.com/your/favorite/loading/gif"
</code>
</details>



## Generate images faster with Stable Horde
Stable Horde uses Kudos to rank users on a queue. The more Kudos you have, the higher you are on the generation queue.
You get Kudos by rating images and/or generating images for Stable Horde
on your local hardware.
To get more Kudos, first stick your api key [here](https://tinybots.net/artbot/settings).
Then, rate some images generated by other users [here](https://tinybots.net/artbot/rate).
After rating for a few minutes, you will have more Kudos!
**IMPORTANT: When an image says, "This rating must be x," you must rate it that. This picture is used as a Captcha to avoid spam.**
