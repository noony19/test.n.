**If you don't have a bot application created, please reference [[Getting a Bot Token]] for how to set one up!**

1. Navigate to the [Applications page](https://discordapp.com/developers/applications/me) and select one of your bot applications.<br> ![App Page](http://i.imgur.com/YxZWndU.png)
2. In the **App Details** section, find the Client ID.<br> ![Client ID](http://i.imgur.com/tsI8nwD.png)
3. Replace the CLIENTID in the following link with your bot's client ID:
```
https://discordapp.com/oauth2/authorize?client_id=CLIENTID&scope=bot
```
For example, if you bot's Client ID is `168682538028630017`, your link would be `https://discordapp.com/oauth2/authorize?client_id=168682538028630017&scope=bot`

4. Go to the link you generated, and select a server from the drop-down menu. **You must have the Manage Server permission to add a bot to a server!** If no servers appear, you may need to [log in](https://discordapp.com/login).

### Troubleshooting
* If you get a "Requires Code Grant" error, make sure that this box is **unchecked** on your application: <br>![Code Grant](http://i.imgur.com/5uOq0Ad.png)