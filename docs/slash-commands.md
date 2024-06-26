icon: material/slash-forward-box

# :material-slash-forward-box: Slash Commands
This Section will explain how to Create, Setup and Use Slash Commands.

!!! warning "Requirements"
    [Slash Commands Builder](/slash-command-builder/){:target="_blank"}  
    [Register Slash Commands Block](https://blocks.dbb.software/Blocks/register_slash_commands.js){:target="_blank"}  
    [Interaction Event](https://blocks.dbb.software/Blocks/interaction_event.js){:target="_blank"}  
    [Get Interaction Argument by Name](https://blocks.dbb.software/Blocks/get_interaction_argument_by_name.js){:target="_blank"}  
    [Reply to Interaction](https://blocks.dbb.software/Blocks/reply_interaction.js){:target="_blank"}  

## Create Commands

:   First go to the [Slash Commands Builder](/slash-command-builder/){target=_blank} and Create a command of your Choice.  
    In this example we will create a Kick and Timeout Command:  
    ![Image](https://i.imgur.com/aIjdRWc.png)

## Copy Command Code

After you built your Command, you click `View Code`
![CMD1](https://i.imgur.com/GBwAuTX.png)  

Import that Command into your Workspace using [Register Slash Commands Block](https://blocks.dbb.software/Blocks/register_slash_commands.js){:target="_blank"}.

## Add Command to DBB

!!! danger "READ THIS!"
    - You can add multiple Commands by using `,` to split the commands

![Image](https://i.imgur.com/CdSCeMc.png)

## Handle The Command Interaction

### Kick Command

First we Build the Kick Command Handler. For that we use the [Interaction Event](https://blocks.dbb.software/Blocks/interaction_event.js){:target="_blank"} Block. Next we use the [Get Interaction Argument by Name](https://blocks.dbb.software/Blocks/get_interaction_argument_by_name.js){:target="_blank"} to get the Member and Reason. Next we use the `Kick Member` Block and connect everything. Optionally you can use the `Merge Texts [Advanced]` Block to add the Mention of the Mmeber to a Message, you can reply to the Interaction using `Reply to Interaction`.
![Command1Handler](https://i.imgur.com/Ft4mOVm.png)

### Timeout Command

Next we will build the Timeout Command Handler. For that we again use the [Interaction Event](https://blocks.dbb.software/Blocks/interaction_event.js){:target="_blank"} Block. Next again use the [Get Interaction Argument by Name](https://blocks.dbb.software/Blocks/get_interaction_argument_by_name.js){:target="_blank"} Block to get the Member and the Time Number in Minutes. After that we use the `Timeout Member` Block and add the Rest of the Optional Stuff if needed.
![Command2Handler](https://i.imgur.com/OjpLbvN.png)

## Testing the Finished Product

After you start your Bot the Command(s) should be available in Discord!
![StartImage](https://i.imgur.com/9SnSXOc.png)
  
***
  
## Subcommands

Subcommands are not much different from natural Slash Commands and even work the same way...  
There are just some changes to the normal way.  

### Building a Slash Subcommand

On the [Slash Commands Builder](/slash-command-builder/){:target="_blank"} you can first setup a main command Name and then for the Argument Type there are two options... Either you select `Subcommand Group`, which allows to setup multiple **Subcommands** within that group. Or you select `Subcommand` and you can have just a **simple subcommand** or multiple subcommands for that one command...  
In this example we are going to create a **Subcommand Group** with 2 Subcommands and a **Subcommand**.

![SubcommandImg1](https://i.imgur.com/9MCqFp5.png)  
![SubcommandImg2](https://i.imgur.com/W50wmkz.png)  

This Example includes a **Echo Command**(Which Repeats the Users Specified Text) and a `messages` Subcommand Group, with a **delete_amount** Subcommand and **del_msg** Subcommand.  
Both Commands will have different functions within one main Command called `tools`.  

After you are done building the Command, you can click `View Code` and Copy the JSON like above.
??? question "The Command Code"

    ``` json
    {
        "name": "tools",
        "description": "Manage Bot Tools",
        "options": [
            {
                "type": 2,
                "name": "messages",
                "description": "Manage the Messages",
                "options": [
                    {
                        "type": 1,
                        "name": "delete_amount",
                        "description": "Delete a Amount of Messages",
                        "options": [
                            {
                                "type": 10,
                                "name": "amount",
                                "description": "The Amount of Messages to Delete",
                                "required": true
                            }
                        ]
                    },
                    {
                        "type": 1,
                        "name": "del_msg",
                        "description": "Delete a Specifc Message by ID",
                        "options": [
                            {
                                "type": 3,
                                "name": "msgid",
                                "description": "The Messages ID you want to delete",
                                "required": true
                            }
                        ]
                    }
                ]
            },
            {
                "type": 1,
                "name": "echo",
                "description": "Let the bot repeat a Message",
                "options": [
                    {
                        "type": 3,
                        "name": "msg",
                        "description": "The Message you want the bot to say",
                        "required": true
                    }
                ]
            }
        ]
    }
    ```

After that you paste it into your `Register Slash Commands` Block and then we continue with...

### Managing Subcommands in DBB

Subcommands are quite similar like Normal Slashcommands but need some special treatments.

![Special Subcommand Treatment](https://i.imgur.com/6sxObfV.png)

As you can see it looks really complicated at first glance, but if you ignore all connections it's pretty understandable. First we start with a `Interaction [Event]` Block and then use `Check if Value Exists` to detect if a **Subcommand Group** was used or not(This is not required if not using `Subcommand Groups`)... 

**If True**, we check the Subcommand using `Switch (conditional)`(As the Input you set `Subcommand Name` from the `Interaction Event`), the rest after that can be customized to your liking.

**If False**, we make the same check, in this case there is only one subcommand in the Main command, so we Just use the same stuff we would use in a normal Slash Command.

I hope this explained Subcommands a bit, it may be hard at first but you'll get into it... Ask around for help on the DBB Discord if you encounter issues.