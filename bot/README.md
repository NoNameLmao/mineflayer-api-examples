# Bot

The bot object. Created from calling the `createBot()` function.
```js
const mineflayer = require('mineflayer');
const bot = mineflayer.createBot({
    username: "technoblade_never_dies", // default: "Player"
    password: "thereisnopassword",      // if omitted (not specified, skipped) - tries to connect in offline mode
    version: "1.12.2",                  // defaults to server's minecraft version, best recommended to specify it yourself
    host: "mc.hypixel.net",             // default: "localhost" (127.0.0.1)
    port: 25565,                        // default: 25565
    auth: "microsoft",                  // default: "mojang". use "microsoft" if the bot account was migrated to Microsoft
    clientToken,                        // generated if a password is given
    accessToken,                        // generated if a password is given
    logErrors: false,                   // default: true. catch errors and log them
    hideErrors: true,                   // default: false. do not log errors (⚠️ overrides logErrors ⚠️)
    keepAlive: false,                   // default: true. send keep alive packets to the server
    checkTimeoutInterval: 1000 * 60,    // default: 1000 * 30 (30 seconds). if the client does not recieve a keep alive packet from the server within that time, disconnect
    loadInternalPlugins: false,         // default: true
    storageBuilder,                     // "an optional function, takes as argument version and worldName and return an instance of something with the same API as prismarine-provider-anvil. Will be used to save the world."
    client,                             // an instance of "node-minecraft-protocol". if ommited, a new one is created
    plugins: {                          // default: {} (empty)
        pluginName: false,              // don't load that internal plugin
        pluginName: true,               // load an internal plugin (⚠️ overrides loadInternalPlugins ⚠️)
        pluginName: () => {}            // external plugin inject (⚠️ overrides original plugin ⚠️)
    },
    physicsEnabled: false              // default: true. should the bot be affected by physics? can be changed later with bot.physicsEnabled
});
```