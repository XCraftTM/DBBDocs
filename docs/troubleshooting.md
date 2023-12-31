icon: material/help-box-outline

# Troubleshooting
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
     
    ![Intents Error](https://media.discordapp.net/attachments/1113796723664498708/1113821079333503057/image_2023-06-01_142602019.png)
     
    This error occurs when the users forgets to allow the bot to use all Intents on the [Discord Developer Portal](https://discord.com/developers/applications) of your Application/Bot.
     
    ![Intents](https://media.discordapp.net/attachments/1021814101778899025/1021827845674246256/unknown.png)

??? failure "Big Error: While installing @discordjs/opus"
    ## **Big Error: While installing @discordjs/opus**
     
    ![opus Error MSG](https://media.discordapp.net/attachments/1110207783212687492/1110207783388840090/image.png)
     
    **Update:** @discordjs/opus isn't being used anymore, please update your Blocks if you still encounter this issue.  

    ~~This error occurs when the wrong NodeJS Version was installed, make sure you installed **v18** and depending on your OS **64x** for **Windows**.~~

??? failure "DBB Error: Command failed: node -v"
    ## **DBB Error: Command failed: node -v**
     
    ![DBB Comand Failed Error](https://cdn.discordapp.com/attachments/1135865936231010426/1135865936444936222/image.png)
     
    This error occurs when NodeJS was not detected, please make sure you installed NodeJS Correctly!
    If you already installed it and it still occurs, please restart your PC.
     
    If you, for whatever reason, can't restart your PC, there is a `Start Bot.bat` file in your Project folder that can start the bot!

??? failure "Cannot read properties of undefined (reading "...")"
    ## **Cannot read properties of undefined (reading "...")**
     
    In this case it means that you connected something to a block that was not found or was not specified, or sometimes even nothing connected at all.  
    Incase you use any "Find" Block, make sure to use IDs to find things, don't rely on using Names. If there is no way around using names, check if the name is written correctly.

---

## **Any Errors**

If any other Error appears always read the error fully, search for the mentioned block and look what you connected to the Block or selected in it...

---

## **Final Note**

If your problem was not listed here or you have issues fixing it you can always join our [Discord Server](https://discord.gg/PAzxTDw){:target="_blank"}

<iframe src="https://discord.com/widget?id=582167093139734544&theme=dark" width="350" height="500" allowtransparency="true" frameborder="0" sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"></iframe>