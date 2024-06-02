icon: material/server-network

# :material-server-network: Host Bot 24/7

You have the Option to host your Bot on your own Home Server, on a Monthly Payed Rootserver/VPS or a special Bot Hosting.  
Here, we will go through all these ways!  

## Host on Rootserver/VPS with Root Access

1. Log into your Rootserver/VPS using a Root Account, then start by Installing Node.JS (If not installed already).  
    ```bash
    curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
    source ~/.bashrc
    nvm install v21
    ```
   
2. Create a new Folder for your Bot and navigate into it.
    It's recommend that you use a Folder like `/home` for your Bot
    ```bash
    cd /home # To get into the Home Directory
    mkdir MySpecialBot # To create a new Folder
    cd MySpecialBot # To navigate into the Folder
    ```

3. Upload your Bot Files into the Folder you just created.  
   - Use a (S)FTP Client of your choice to upload the Files, for example WinSCP or FileZilla work great.  
   - Create a New Connection with the IP/Domain of your Server, Username(root) and Password.
   - Navigate to the Folder you just created and Drag-and-Drop the Files into it.
   Here is a list of things you need to Upload, leave everything else away. NOTE: Upload the Full Blocks Folder!
   ```
    ├── blocks/
    │   ├── block1.js
    │   ├── block2.js
    │   └── etc...
    ├── data/
    │   ├── data.json
    │   ├── INTENTS.txt
    │   ├── token.txt
    │   └── workspaces.json
    ├── bot.js
    └── package.json
    ```

4. Run the Bot using the following Command:
    ```bash
    node bot.js
    ```
    - This will start the Bot and you should see the Bot Online in your Discord Server.

5. Optional to run the Bot 24/7, using Screen
    ```bash
    screen -S BotName node bot.js
    ```
    - This will start the Bot in a Screen Session, to detach from the Screen use `CTRL+A` and then `CTRL+D`. To reattach use `screen -x BotName`.