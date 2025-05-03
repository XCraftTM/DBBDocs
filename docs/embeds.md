icon: material/message-text

# :material-message-text: Embeds
This Section will Explain how to Create a Message embed, and also send that Embed.

???+ danger "This Page explains using Mods!"
    :   This Page includes Content using Community Created Mods and may vary from your experience!

    :   [Go to Documentation page for Mods :fontawesome-solid-arrow-right:](/mods){ .md-button .md-button--primary }

## Setup the Workspace
:   First of all you will need to use the `Create Message Embed` Block, to create the Embed with the Text that you want to send.  
After that you will need to use a block that sends a Message, that may be a Interaction Reply, or just a Message in a Channel.  
(Note: If you send a Embed, Text Input is not Needed)  

:   ![Image](assets/embeds/setup-workspace.png)

## Running in Discord
:   After you Start your Bot, just run the command you setup and your Embed should appear.  

:   ![Image](assets/embeds/running-in-discord.png)

## Adding Text from the Command
:   If you want to get Text from the Command, or combine text from another place, it's really easy.  
For that we use the `Merge Texts (Advanced)` Block.  

:   ![Image](assets/embeds/embed-with-custom-text-from-command.png)

:   ![Image](assets/embeds/embed-with-custom-text-example.png)

## Editing Embeds
:   Editing Embeds is a kinda hard Task if you don't know which Blocks you need to use.
Here is a still simple example how to do it, safely.

:   At the Top it shows the Command Example from above and at the end of it, is now added a `Control Data` Block.
This Blocks Saves the Message ID for editing the Embed later.

:   The Bottom Part shows a `!editembed` Command where first it gets the Message ID we saved earlier using `Get Data`, then finds the Message using `Find Message`(Make sure to connect a Channel), then gets the Embeds and then gets the first one using `Get Item from List`.
You can then edit the Embed using `Edit Message Embed`(For this Tutorial there was a fixed version, use the best one for you) and then edit the Message using `Edit Message`(Make sure to connect the Message from the Find Message Block, and not from the Command).

:   ![image](assets/embeds/sending-and-editing-after-embed.png)

:   In Discord it looks like this!

    :   ![GIF](assets/embeds/send-edit-embed-testing.gif)