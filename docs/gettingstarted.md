icon: material/information-variant-box

# :material-information-variant-box: Getting Started
This section will explain how to install NodeJS, setup a Bot Project within DBB as well as create and invite your Discord Bot!  
***

=== "1. Preparation"
    <h3>Installing Node.js</h3>

    :   In order to allow your bot to run, you will need to install Node.js:

    :   ??? info "Installing on Windows"
            - Click [here](https://nodejs.org/dist/v22.12.0/node-v22.12.0-x64.msi){:target="_blank"} to download the installer for the LTS version of Node.js.
            - Follow the installer's instructions

    :   ??? info "Installing on Ubuntu via CLI"
            - Copy these commands using the copy button in the top right hand corner of the box and paste them into your command line.
            ```
            curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
            source ~/.bashrc
            nvm install v22
            ```

    ***

=== "2. Creating a Project"
    <h3>Create Your First Project</h3>

    :   1. Start DBB. You will be greeted with this screen:

        :   ![StartupScreen](assets/getting-started/2-creating-project/first.png)
    <br>

    :   2, Click on Create New Project. You should now have this screen:

        :   ![CreateBotScreen](assets/getting-started/2-creating-project/second.png)
    
        :   After these Steps, you now have a Temporary Project opened in which you can start creating your Bot.

        :   To Make sure that you progress is not lost after a restart, you can save your Project by clicking on the `Save` Button in the Top Left Corner in the `Project` Menu.

        :   ![CreateBotScreen](assets/getting-started/2-creating-project/third.png)<br>

        :   Then, a Window Pops up in which you can go into the Folder you want to the Save the Project in and then also set a Project Folder name. After that you can click on `Save`.

        :   ![SaveWindow](assets/getting-started/2-creating-project/fourth.png)<br>

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

    :   ![Gif](assets/getting-started/3-creating-bot/discord-dev-portal-creation.gif)<br>
    <br>
    Input it into DBB. Do this by selecting the Bot menu in the toolbar at the top of the screen and selecting Set Bot Token. Then paste the token and hit Enter or click OK.

    :   ![Image](assets/getting-started/3-creating-bot/input-token-in-dbb.png)<br>
    <br>

    :   Now you need to invite the bot to your server. You can get a Link by Going into the Discord Developer Portal, selecting your Application, going to OAuth2, and then selecting the `bot` and `application.commands`(Slash Commands) scope. After that you can select the permissions you want to give the bot and then copy the link.

    :   ![CreateInviteInDiscordDevPortal](assets/getting-started/3-creating-bot/invite-bot.gif)<br>
    <br>

    :   Then go to your web browser and paste the invite link there. Choose which server you want to invite the bot to and click Continue.

    :   ![DiscordInviteStart](assets/getting-started/3-creating-bot/click-on-invite-link.png)<br>
    <br>

    :   On the next page, a huge list of permissions will come up. Change them as you wish. Scroll down to the bottom (there will be some information about your bot) and click Authorize.

    :   ![DiscordInviteStart](assets/getting-started/3-creating-bot/check-permissions.png)<br>
    <br>

    :   Finally, complete the reCAPTCHA, click Verify, and this message should display.

    :   ![EndImageDiscordInvitePage](assets/getting-started/3-creating-bot/success-inviting.png)
    <br>

    :   That means you're all set and the bot's now in your server.

    ***

## Other Important Stuff

:   !!! warning "Important"
        Without an event, your command will never work! Events are the only blocks that have no "Action Connection" input since they get triggered by the bot itself.

:   ??? knowledge "Variable Types"
        ![Image](assets/getting-started/useful-variable-types.jpg)

:   The line types must match to connect two blocks.

:   On the Output side of the block, there can be as many connections to one point as you like (except on the action type).

:   On the Input side of the block, there can always only be one connection per point.

:   ??? knowledge "Good to know"
        Server = Guild

        User ≠ Member

        A member is a user that is relevant to the guild only. You can execute actions to do with a specific server with a member.

## Your turn!
:   Use these Examples, Tutorials and Infos to create your own Bot. Maybe you can even try to code your own Blocks and learn Javascript!
