icon: material/form-textbox

<meta content="Modals - DBB Documentation" property="og:title" />
<meta content="A Modal is a box that appears after a Interaction where the user can fill infos." property="og:description" />
<meta content="https://dbb.software/" property="og:url" />
<meta content="https://raw.githubusercontent.com/XCraftTM/DBBDocs/refs/heads/main/docs/assets/favicon.png" property="og:image" />
<meta content="#292e4a" data-react-helmet="true" name="theme-color" />

# :material-form-textbox: Modals
This Section will explain how setup a Modal, and show that to the User and also fetch what the User Inputed into the Modal.

???+ danger "This Page explains using Mods!"
    :   This Page includes Content using Community Created Mods and may vary from your experience!

    :   [Go to Documentation page for Mods :fontawesome-solid-arrow-right:](mods.md){ .md-button .md-button--primary }

## Setup Modal
:   !!! warning "Important"
        * To be able to receive a Modal, a normal Prefix Command is not working, you will need some kind of Interaction. 
        
        :   This can be a Slash command, Button or Select Menu.  

    !!! danger "Modals have Changed"
        Modals have changed a LOT, they now require the usage of the Components V2 which can be a bit overwhelming but allow for more features.
        The Guide will go over each Combination that you can do for Modals to explain it as well as possible.

    ### Adding Normal Text Inputs to Modals
    :   To add Text Inputs to Modals use need to use a `Label (Component)` in combination with `Modal Text Input (Component)`,

    :   ![Image](assets/modals/text-input.png)

    ### Adding Text Displays
    :   Text Displays supports any Discord Message Formatting including Headers or other formatting, even multi lines.

    :   ![Image](assets/modals/text-displays.png)

    ### Adding Select Menus
    :   Select Menus are the one New Thing for Modals, they can be any Type of Select Menu.

    :   ![Image](assets/modals/select-menu.png)

    ### Everything Together in Discord
    :   If you combine all three Types you can get something similar to this!

    :   ![Image](assets/modals/modal-in-discord.png)

## Reacting to the Modal
:   You just use the `Interaction [Event]` again, set it to Modal, and enter CustomID of the Modal.  

    Then use the `Get Modal Argument by Name` to get both Field Inputs, and use them as you like. In this Example we will add them together using `Merge Texts (Advanced)`.  

    After that Reply to the Interaction to tell the User that we received the Input!  

    ![Image](assets/modals/handle-modal.png)

## Testing in Discord

:   ![GIF](assets/modals/testing-in-discord.gif)