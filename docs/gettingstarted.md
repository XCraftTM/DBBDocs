icon: material/information-variant-box

# :material-information-variant-box: Getting Started
This section will explain how to install NodeJS, setup a Bot Project within DBB as well as create and invite your Discord Bot!  
***

=== "1. Preparation"
    <h3>Installing Node.js</h3>

    :   In order to allow your bot to run, you will need to install Node.js:

    :   ??? info "Installing on Windows"
            - Click [here](https://nodejs.org/dist/v18.18.2/node-v18.18.2-x64.msi){:target="_blank"} to download the installer for the LTS version of Node.js.
            - Follow the installer's instructions

    :   ??? info "Installing on Ubuntu via CLI"
            - Copy these commands using the copy button in the top right hand corner of the box and paste them into your command line.
            ```
            curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
            source ~/.bashrc
            nvm install v18
            ```

    ***

=== "2. Creating a Project"
    <h3>Create Your First Project</h3>

    :   1. Start DBB. You will be greeted with this screen:

        :   ![StartupScreen](https://i.imgur.com/5tpQr9i.png)
    <br>

    :   2, Click on Create New Project. You should now have this screen:

        :   ![CreateBotScreen](https://i.imgur.com/T8gcDbn.png)
    
        :   The 'Bot Folder Name' is the name of your project and the name of the folder that will contain your bot. The Bot Folder Path is the directory on your computer where the new folder containing your bot will be created.

        :   In the example below, the bot will be saved in the folder "DBBProjects" in a new folder and with the project name 'MySpecialBot'

        :   ![CreateBotScreen](https://i.imgur.com/2h7reFa.png)<br>

    ***

=== "3. Creating a Discord Bot"
    <h3>Create a New Bot Account and Set it Up in DBB</h3>

    :   Go to the [Discord Developer Portal](https://discord.com/developers/applications){:target="_blank"} and do the following things:

        :   1. Create a New Application with the name of your Choice <br>
            2. Go to "Bot", and click "Add Bot" <br>
            3. After that you go down and enable the 3 "Privileged Gateway Intents" <br>
            4. Disable Public bot, to make the bot only inviteable via the URL <br>
            5. Copy the Bot Token and save it for later... <br>
            (**Note: MAKE SURE TO KEEP THE TOKEN SECRET AT ALL TIMES! IF SOMEBODY GETS THE BOT TOKEN, THEY CAN ACCESS AND ABUSE YOUR BOT!**) <br>

    :   ![Gif](https://i.imgur.com/8xMWmLL.gif)<br>
    <br>
    Input it into DBB. Do this by selecting the Bot menu in the toolbar at the top of the screen and selecting Set Bot Token. Then paste the token and hit Enter or click OK.

    :   ![Image](https://i.imgur.com/bANjuKK.png)<br>
    <br>

    :   Now you need to invite the bot to your server. Get an invite link by going to the Bot menu in the toolbar at the top of the screen and selecting Generate Invite.

    :   ![CreateInviteInDBB](https://i.imgur.com/UUxaWD8.gif)<br>
    <br>

    :   Then go to your web browser and paste the invite link there. Choose which server you want to invite the bot to and click Continue.

    :   ![DiscordInviteStart](https://i.imgur.com/hUFHGMO.png)<br>
    <br>

    :   On the next page, a huge list of permissions will come up. Change them as you wish. Scroll down to the bottom (there will be some information about your bot) and click Authorize.

    :   ![DiscordInviteStart](https://i.imgur.com/g6W4Qvh.png)<br>
    <br>

    :   Finally, complete the reCAPTCHA, click Verify, and this message should display.

    :   ![EndImageDiscordInvitePage](https://i.imgur.com/wubHQWG.png)
    <br>

    :   That means you're all set and the bot's now in your server.

    ***

## Other Important Stuff

:   !!! warning "Important"
        Without an event, your command will never work! Events are the only blocks that have no "Action Connection" input since they get triggered by the bot itself.

:   ??? knowledge "Variable Types"
        ![Image](https://i.imgur.com/1n2IEHy.jpeg)

:   The line types must match to connect two blocks.

:   On the Output side of the block, there can be as many connections to one point as you like (except on the action type).

:   On the Input side of the block, there can always only be one connection per point.

:   ??? knowledge "Good to know"
        Server = Guild

        User ≠ Member

        A member is a user that is relevant to the guild only. You can execute actions to do with a specific server with a member.

## Your turn!
:   Use these Examples, Tutorials and Infos to create your own Bot. Maybe you can even try to code your own Blocks and learn Javascript!
