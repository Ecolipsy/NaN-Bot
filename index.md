# NaN-Bot
Hello, and welcome to the NaN-Bot homepage! This page is not done yet so that is the reason of the lack of content.

## Here is a mineflayer example:
```js
const mfl = require('mineflayer');
const bot = mfl.createBot({
  host: "ip.hostnamecraft.net",
  port: "25565", //<-- not required if port is 25565
  username: "me@mymailprovider.mail", //<-- insert email if server is online mode
  password: "MyVeryStrongPassword125"
});

bot.on('login', () => {
  console.log('Hello, world!')
  bot.chat('Hello, world!')
});

bot.on('message', (message) => {
  if(message == '!ping'){
    bot.chat('Pong!')
  }
});
```

## And here is a discord.js example:
```js
const dc = require('discord.js');
const client = new dc.Client();

client.on('ready', () => {
  console.log('Ready!');
});

client.on('message', (message) => {
  if(message.content == '!ping'){
    msg.channel.send('Pong!')
  }
});

client.login('Token')

/*
To invite your bot you have to go to "https://discordapp.com/developers/applications".
Then when you have made an application go to the "Bot" option with a little pussle piece.
When you have created a bot you can copy the token and paste it in the client.login line.
Back to inviting your bot, go to the application and hit the "OAuth2" option with a wrench.
Then check the "Bot" box in scopes and go down to the bot permissions and check the "Administrator" box.
Then you can copy the link you will be provided with and enter it in any browser to invite your bot.
*/
```

## If you have any other questions or want help with your code, join our discord server [here](https://discord.gg/H8VzY7e)
