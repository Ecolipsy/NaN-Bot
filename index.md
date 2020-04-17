# Welcome to NaN-Bot!

This is the homepage of NaN-Bot. You will find tutorials on Mineflayer and Discord.js here, and also, this page is not finished yet, so that is the reason for the lack of content.

## Mineflayer tutorial:
```js
const mineflayer = require('mineflayer');
const bot = mineflayer.createBot({
  host: "your.server.ip"
  port: "25565" //Not required if port is 25565
  username: /*If server is not cracked use email*/ "TestMineflayerBot"
  password: "MyStrongPassword123" //Not required if server is cracked
});

bot.on('login', () => {
  bot.chat('I am ready!')
  console.log('I am ready!')
});

bot.on('message', (user, msg) => {
  if(msg == '!hi'){
    bot.chat('Hello, ' + user + '.')
  }
});
```

## Discord.js tutorial:
```js
const discord = require('discord.js');
const client = new dc.Client();

client.on('ready', () => {
  console.log('I am ready!')
});

client.on('message', (msg) => {
  if(msg.content == '!hi'){
    msg.channel.send('Hello, **' + msg.author.username + '**. :slight_smile:')
  }
});

client.login('Token') //You can get a bot token from "https://discordapp.com/developers/applications".

/*
To invite your bot you have to go to "https://discordapp.com/developers/applications".
Then when you have made an application go to the "Bot" option with a little pussle piece.
When you have created a bot you can copy the token and paste it in the client.login line.
Back to inviting your bot, go to the application and hit the "OAuth2" option with a wrench.
Then check the "Bot" box in scopes and go down to the bot permissions and check the "Administrator" box.
Then you can copy the link you will be provided with and enter it in any browser to invite your bot.
*/
```

### If you want help with your code or just want to chat with people on a Minecraft server without an account you can click [here](https://discord.gg/H8VzY7e).
