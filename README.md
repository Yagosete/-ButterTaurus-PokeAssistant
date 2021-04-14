# PokéAssistant
A Pokétwo Hack/Assistant Bot to help you with catching Pokémons on Pokétwo.
## Information
PokéAssistant is a bot aimed to help Pokétwo players. It will tell you what Pokémon it is whenever Pokétwo spawns one (Free) and will also ping a role if rare pokemons spawn (Premium Only). As such, you no longer have to rack your brains or even search Google. Sometimes, you may just miss a rare Pokémon like this.
### Developer
TrashUwU#8019

![](https://cdn.discordapp.com/attachments/735938202782924952/831890258223956018/20210414_195332.jpg)

### How does it work?
It uses a light machine learning module, that can predict Pokémons in 5-7 seconds using only 500 MB ram!
### Issues?
Facing issues with the bot? Please create an Issue.
### Why is the source code messed up?
It's encrypted/obfuscated. I don't want Pokétwo mods to read and patch against it. But you can run it without problem!
### Why can't I invite the bot instead of hosting it?
Discord does not verify bots that work against other bot(cheat bots). Server limit for unverified bots is 100 and bots in 1K+ servers need too much ram. That means you can't invite it to your server, if it's in 100 servers already 😵. With the help of this guide, you can make your own bot and customize it without coding!
### Want to help?
Star the repository, refer your friends to this Github repository! Join the support server to request faster results, no ads and decreased rate limit! You must create a support ticket to contact the moderators.
### Bot Repl
https://replit.com/@ButterTaurus/PokeAssistant
### Server invite link
https://discord.gg/CtXvFj9yPq

## Features
- Fast and light
- Can be hosted 24/7 on cloud or on PC
- Pokemon dataset updates automatically (But if the code gets updated, you need to copy the updated code and paste it in your REPL)
- Returns 2-3 Pokemons as prediction

## Premium Features
- Faster Prediction (Reduced 4000ms waiting time)
- Decreased rate limit to 20 seconds
- No ads
- Final Prediction
- Pings a specific role when rare pokemons spawn

## Bot Installation Guide Guide
You surely want a private bot for your server, now that you have got the source code, you wonder: how do I keep the bot up 24/7?
So here the guide exists to teach you how.
### Step 1: Creating a bot account
The first step in creating a bot is to create your own Discord application. The bot will use the Discord API, which requires the creation of an account for authentication purposes. Don't worry though, it's super simple.
#### Creating the application
To create the application, head to https://discord.com/developers/applications/. Log in, and you'll reach a page that may look like this:

![](https://media.discordapp.net/attachments/660518707134595095/830720086921707540/1.png)

Click on **Create an application**. This brings you to the following page, in which you should simply enter a name for the application. After clicking **Create**, you can also add an avatar. Click **Save Changes** afterwards.

![](https://cdn.discordapp.com/attachments/660518707134595095/830720419568418857/2.png)

#### Creating the bot account
After creating the application, we need to create the Bot User. Go to the Bot section on the left, then click on **Add Bot**, then **Yes, Do it**.

![](https://cdn.discordapp.com/attachments/660518707134595095/830720692583923723/3.png)

There's a few things you can change here. 
- Username: Change your bot's username on Discord
- Icon: Change the bot's avatar
- Public bot: Toggles the ability for other users to add your bot to their server.
- Require Oauth2 Code Grant: Don't check this. Just, don't.
#### Adding to your server
To generate the invite link, click on **Oauth2** in the app page, and scroll down to **Scopes**. Check the **Bot** scope to generate a link. You can also add additional permissions for the bot.

![](https://cdn.discordapp.com/attachments/660518707134595095/830720814994161664/4.png)

Copy the link and open it, select your server and click on **Authorize**. Cheers, it has been added to your server.
#### Getting the token
Go to the **Bot** page and copy the token. Save it somewhere, you will need that later.

![](https://cdn.discordapp.com/attachments/660518707134595095/830720955277508628/5.png)

Source: https://anidiots.guide/getting-started/getting-started-long-version
### Step 2: Hosting the bot
The bot will be hosted on Replit, so you need to create a Replit account first: https://replit.com/login.
#### Getting the code
The code has already been setup, you only need to go to https://replit.com/@ButterTaurus/PokeAssistant and click `fork`. Wait 10-60 seconds after forking.

![](https://cdn.discordapp.com/attachments/678537293820330005/830756922487603220/6.png)

#### Configuration
(Mobile users will click `files` button to see all files, all files will be visible to PC users by default)
Create a `.env` file. Now open `.env` file.

![](https://i.postimg.cc/mr6hFySJ/Untitled.png)

Now open `.env` file. All options are compulsory.
- TOKEN: Your bot token
- OWNER: Your Account ID
- CHANNEL: Channel ID where Pokétwo spawns, for multiple channels separate with `,` (no spacing)


An example would be:
```
TOKEN=NTU2NjQ2MjA1MDExMDAxMzQ1.D29B7Q.LcTk_nSujMXdVyFohpJpjF50odE
CHANNEL=771967676951429150,771967676951429150,733971269527273492
OWNER=663917469523843492
```

![](https://cdn.discordapp.com/attachments/806194434117992499/831071426491449355/10.png)
(Mobile users will click on console and click green **play** button to run)
(PC users will click Green **Run** Button.)

The bot should be online now.

### Step 3: Keeping the bot online (Optional)
Replit shuts down projects that are inactive for over 5 minutes. The current code should already keep it up, but some users feedback that it doesn't. We will be using Uptime Robot to keep it up here. Create an account first: https://uptimerobot.com/signUp.

After signing up, login and go to the Dashboard, click on **Create New Monitor**, the configurations are as follows:

![](https://cdn.discordapp.com/attachments/678537293820330005/830758495824510986/8.png)

- Monitor Type: Choose HTTP(s)
- Friendly Name: Literally anything
- URL (or IP): Put `your repl`'s link. Repl links are [these](https://cdn.discordapp.com/attachments/678537293820330005/830757823549276160/7.png) and mobile users will click `web` button to get the repl link.
- Monitoring Interval: 5 minutes

Finally click **Create Monitor** and you're done! Done with everything!

### Keep in Mind
- If the bot gets updated, you will need to copy the index.js code and paste it in the index.js of your repl or the bot will stop working
- The bot will identify 1 pokemon every 60 seconds; if there are multiple spawns in 1 minute, the bot will get rate limited
- Reduce the number of channels in `.env` if the bot gets rate limited too many times
- The bot has permissions to send embeds
- Upgraded/Premium bot includes decreased rate limits(1 pokemon every 20 seconds), no ads, pings a role if a rare pokemon has spawned(Coming Soon), gives final prediction and faster response
- Make sure `.env` is not empty and information provided there is correct
- Make sure the bot can DM the owner
- The bot's accuracy is 80%
- Do not edit the code, because it will break the whole bot :/

### Get Premium
Join the support server and create a support ticket to contact the moderators. Premium can't be bought with money.

### Made by TrashUwU#8019
