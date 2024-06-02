icon: material/help-box-outline

# :material-help-box-outline: Troubleshooting
Issues are normal in DBB, since mostly everything is made by the community, but sometimes it's just the users fault. Try following these steps if you have issues!

---

???+ success "An Always Fix"
    If you encouter some weird issue that was not documented and happens with some block or anything just try this fix to get it working...

    Make sure your Bot is Not Running while following these Steps...
    
    Remove the `node_modules` folder and `package-lock.json` file in your Project folder,  
    then run `npm cache clean --force` in a Terminal/CMD that is navigated to the Bot Folder and then start your Bot.

---

??? failure "Error: Used Disallowed Intents"
    ## **Error: Used Disallowed Intents**
     
    ![Intents Error](https://i.imgur.com/VJ7MsbQ.png)
     
    This error occurs when the users forgets to allow the bot to use all Intents on the [Discord Developer Portal](https://discord.com/developers/applications) of your Application/Bot.
     
    ![Intents](https://i.imgur.com/nF2znDh.png)

??? failure "Big Error: While installing @discordjs/opus"
    ## **Big Error: While installing @discordjs/opus**
     
    ![opus Error MSG](https://i.imgur.com/NQFxLaz.png)
     
    **Update:** @discordjs/opus isn't being used anymore, please update your Blocks if you still encounter this issue.  

    ~~This error occurs when the wrong NodeJS Version was installed, make sure you installed **v18** and depending on your OS **64x** for **Windows**.~~

??? failure "DBB Error: Command failed: node -v"
    ## **DBB Error: Command failed: node -v**
     
    ![DBB Comand Failed Error](https://i.imgur.com/Xai6kXD.png)
     
    This error occurs when NodeJS was not detected, please make sure you installed NodeJS Correctly!
    If you already installed it and it still occurs, please restart your PC.
     
    If you, for whatever reason, can't restart your PC, there is a `Start Bot.bat` file in your Project folder that can start the bot!

??? failure "Cannot read properties of undefined (reading "...")"
    ## **Cannot read properties of undefined (reading "...")**
     
    In this case it means that you connected something to a block that was not found or was not specified, or sometimes even nothing connected at all.  
    Incase you use any "Find" Block, make sure to use IDs to find things, don't rely on using Names. If there is no way around using names, check if the name is written correctly.

---

## **Any Errors**

:   If any other Error appears always read the error fully, search for the mentioned block and look what you connected to the Block or selected in it...

---

## **Final Note**

:   If your problem was not listed here or you have issues fixing it you can always join our [Discord Server](https://discord.gg/PAzxTDw){:target="_blank"}