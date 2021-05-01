<br />
    <p>
    <a href="https://dbd.js.org/invite"><img src="https://cdn.discordapp.com/attachments/804505461076131840/837194632148287509/Aoi.js_6_ver._2.png" alt="aoi.js" /></a>
  </p>

# Aoi.JS
[![NPM Downloads](https://img.shields.io/npm/dt/aoi.js.svg?maxAge=3600)](https://www.npmjs.com/package/aoi.js)
[![Discord Server](https://img.shields.io/discord/773352845738115102?color=7289da&logo=discord&logoColor=white)](https://dbd.js.org/invite)

## Table Of Contents
- [About](#about)
  - [Setup](#setup)
  - [Variables](#variables)
  - [Events / Callbacks](#callbacks)
- [Additional Support](#methods)
  - [Slash Commands](#slash-commands)
  - [Music](#music)
- [Links](#links)


## About
Aoi.JS is a package that aim to allows you to make your Discord Bots with Ease.

Aiming to be the easiest package to learn <br>
It's swift and flexible using functions </br>

## Examples

### Setup
```js
const Aoijs = require("aoi.js")

const bot = new Aoijs.Bot({
token: "TOKEN", //Discord Bot Token
prefix: "!" //Customizable
})
bot.onMessage() //Allows to run Commands

bot.command({
name: "ping", //Trigger name (command name)
code: `$ping Pong!` //Code
})
```

### Variables

What are variables?

Variables are Key-Value based data which is stored in the database, useful for Economy and Leveling system as it is allows you to save data.

```js
bot.variables({
  VariableName1: "Value", //Returns "Value"
  VariableName2: "Value2" //Returns "Value2"
})
```

### Callbacks

What are callbacks?

It's simple and easy process, it essentially allows you to trigger events, such as user joining a Guild.
This will trigger an event, causing commands with supported type for each callbacks to be executed such as.

```js
bot.joinCommand({
        channel: "Channel ID", //Enter a Channel ID
        code: `<@$authorID> just joined, welcome!` //This can be changed
})
bot.onJoined()
```

## Additional Support

### Slash Commands

With easy and simple functions, you can make Slash Commands with your Bots quick!

```js
bot.command({
    name: "slash",
    code: `$createSlashCommand[$guildID;version;Returns Aoi.js Version]`
})
bot.interactionCommand({
    name: "version", 
    code: `$interactionReply[$packageVersion]`
})
bot.onInteractionCreate()
```

More Information in our [Documentation](https://dbd.leref.ga/guide/slash-commands)

#### Music

With our powerful Package, we incorporated Music with several functions.
We allowed customization and control over what you want.


#### Music Setup Example

```js
bot.command({
name: "play", //Trigger name (command name)
code: `$playSong[song;leave vc time;defean (yes or no);leave when vc empty (yes/no);error]`
//Code
})
```

More Information in our [Documentation](https://dbd.leref.ga/guide/music)

## Links
Aoi.JS was made by [Aoi.JS Team](https://discord.gg/HMUfMXDQsV)
- [Website](https://dbd.js.org)
- [Discord Server](https://dbd.js.org/invite)
- [Documentation](https://dbd.leref.ga)

## Contributing
Please read [Contributing](https://www.github.com/aoijs/aoi.js/.github%2FCONTRIBUTING.md)
