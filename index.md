# Welcome to NaN-Bot!

This is the homepage of NaN-Bot. You will find tutorials on Mineflayer and Discord.js here.

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
```

### If you want help with your code or just want to chat with people on a Minecraft server without an account you can click [here](https://discord.gg/H8VzY7e).
