icon: material/music-box

# Music Blocks

=== "Setup"
    ## Setup

    The Music Player Blocks will probably not work from the start, so we need some dependencies that we need to install.

    Run these commands to install the required packages to play Music:  

    ```
    npm i discord-player@latest  
    npm i @discord-player/extractor@latest  
    npm i mediaplex@latest  
    npm i ffmpeg-static (If on Linux, do: apt install ffmpeg)
    npm i youtube-ext@latest  
    ```

    ???+ info "Newest Patch 09/15/2023"
        The `Discord Audio Player Dependency` Block now AUTOMATICALLY Installs Updates and removes old not supported packages.

    ***

=== "Examples"
    <h3> Play Music in Voice Channel </h3>

    > Playing Music is really easy, and doesn't take a lot of Blocks... Here is a Simple Example:
    ![PlayInVC](https://i.imgur.com/inEUci8.png)

    <h3> Setup Slash Command Autocomplete </h3>

    > Below is an example of how to enable Auto Complete on a slash command: 
    ![AutoCompleteSlashCommands](https://cdn.discordapp.com/attachments/1081509800464109638/1085955745671032994/image.png)

    ***

=== "Troubleshooting"
    A quick follow-up for discord-player v6, if you are getting weird errors like `something is not a constructor` or `version.split is not a function` or something similar, please try the following:

    Remove `node_modules`, `package-lock.json` or any lockfiles you have, run `npm cache clean --force` or similar command equivalent to your package manager and then run `npm install` (or the install command of your package manager)

    ***