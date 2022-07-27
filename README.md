const {
    Client,
    Intents
} = require('discord.js');

const bot = new Client({
    intents: [Intents.FLAGS.GUILDS, Intents.FLAGS.GUILD_MEMBERS, Intents.FLAGS.GUILD_MESSAGES]
});

bot.on('ready', () => {
    console.log(`Bot ${bot.user.tag} is logged in!`);
});

bot.login('YOUR_BOT_TOKEN'); // Replace
