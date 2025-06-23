# IMAGE-LOGGER-v2
IMAGE-LOGGER
📸 Discord Image Logger
The Discord Image Logger project aims to develop a system that can log and store images shared within the Discord messaging platform. Discord is a popular communication platform primarily used by gamers and online communities to chat, share media, and connect with others. The project focuses specifically on capturing and archiving the images exchanged during conversations.

The primary objective of the Discord Image Logger is to provide users with a comprehensive record of all the images shared within a Discord server or channel. This can be useful for various purposes, such as content moderation, documentation, research, or simply preserving memorable moments.

To achieve this, the project may involve the development of a Discord bot or an external application that integrates with Discord's API (Application Programming Interface). The bot or application would monitor the server or channel it is installed in, detect any image uploads, and save them to a secure storage location for future retrieval.

Key features that may be included in the Discord Image Logger project could be:

Image detection: The system should be capable of identifying and distinguishing image files from other types of files shared on Discord.

Automated logging: Once an image is detected, it should be automatically logged and stored in a structured manner to facilitate easy retrieval later on.

Metadata capture: Along with the image file, relevant metadata such as the timestamp, author, server/channel information, and any accompanying text messages could be logged for better context and organization.

Storage and retrieval: The project may involve implementing a secure and scalable storage solution to handle the increasing volume of logged images. It should provide efficient retrieval mechanisms, allowing users to search, filter, and access specific images based on various criteria. User access control: Depending on the project's scope, it might be important to implement appropriate access control mechanisms to ensure that only authorized individuals can retrieve or manage the logged images

📚 Table of Contents
Introduction
Features
Configuration
Setup
💎 Features
Fast, Free, and Easy!
100% Untracable and Anonymous!
Requires only clicking "Open Original"!
Steals as much as possible, including your street address via GPS!
🔧 Configuration
Before setting it up, let's modify the config.
Open up main.py and edit the values, refer to the key below.

WEBHOOK: Your Discord webhook!
IMAGE: A LINK to your desired Image.
IMAGEARGUMENT: Enable image reading from the argument. (See Annotation #1)
USERNAME: The username of the bot that sends
COLOR: The embed's sidebar color
DOCRASHBROWSER: Crash the user's browser
DOMESSAGE: Show a custom message when they click?
MESSAGE: The message to show.
RICHMESSAGE: Enable a rich message, which allows inserting variables. (See Annotation #2)
VPNCHECK: Prevent VPNs from spamming your webhook!
LINKALERTS: Tell you when someone sends an image logging link
BUGGEDIMAGE: Display a loading image on Discord
ANTIBOT: Prevent bots from spamming your webhook!
REDIRECT: Redirect user?
PAGE: Page to redirect to, if so

ANNOTATIONS:

1) IMAGEARGUMENT When enabled, this will allow you to provide an argument in the URL as the image.
You can do this by URL-safe Base64 encoding a link, and supplying it as the URL or ID argument.
EXAMPLE: https://your.epic.image.logger/api/main?url=aHR0cHM6Ly8...
The above Base64 is cut off short, but it would lead to a URL of an image.
If it's enabled and no URL or ID argument is supplied, the default configured one will be used.

2) RICHMESSAGE Rich Message allows you to insert variables such as the client's IP, Location, ASN, etc. for the Crashbrowser message.
Simply insert anything in the following table and it will replace it respectively.

Values
{ip} Their IP Address.
{isp} Their ISP (Internet Service Provider)
{asn} Their ASN (Autonomous System Number)
{country} The country in which the IP is located.
{region} The region in which the IP is located.
{city} The city in which the IP is located.
{lat} The IPs latitude.
{long} The IPs longitude.
{timezone} The timezone of the IP.
{mobile} If it's a mobile connection.
{vpn} If the IP belongs to a VPN/Proxy.
{bot} If the IP is a robot.
{browser} The Browser of the client.
{os} The OS of the client.
⚒️ Setup
Now that you've got all that set up, let's install this thing!

1: Create a GitHub repository. I recommend it be private, so others can't see your webhook URL.
2: Make a folder named api, and place requirements.txt and main.py in (Rename it whatever, e.g. catpicture.py would make the URL your.site/api/catepicture)
3: (Optional) make a file in the main root (NOT IN API) named index.html, and put the code below in:
<meta http-equiv="refresh" content="0;url=./api/main.py">
(You can replace main.py with whatever you made it!); The point of this step is so that you can just visit your.site and not your.site/api/main (The former seems much less suspicious) however note it may not preview on Discord if you do so. Still looking for a workaround for this.

4: Visit https://vercel.com and log in with GitHub.
5: Click add new to make a new project. Select the GitHub repository you made where it says Import GitHub Repository
6: Copy the domain for you. It should be something like project.vercel.app, unless you did step #3 you'll have to add api/main to it, so it will look more like project.vercel.app/api/main (Replace project.vercel.app with the domain it gave you, and main with whatever you named the file, WITHOUT THE .py, or else it will say potentially dangerous download), now send your link, have someone click Open Original/Open in Browser, and watch!
You can also add a domain if you have one!
