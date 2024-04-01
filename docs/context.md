icon: material/form-select

# :material-form-select: Context Menu
This Section will explain how to create and use Context Menus!

!!! warning "Requirements"
    [Interaction Event](https://blocks.dbb.software/Blocks/interaction_event.js){:target="_blank"}  
    [Get Property from Object with Option](https://blocks.dbb.software/Blocks/get_property_from_object_option.js){:target="_blank"}  
    [Reply to Interaction](https://blocks.dbb.software/Blocks/reply_interaction.js){:target="_blank"}  

The Idea is pretty straight-forward. Just register them like normal slash commands, then catch them when used, using `Interaction Event` Blocks and then you can continue like you want:  

:   ![Image](https://i.imgur.com/qq99T1E.png)

Here is the Copyable version of the JSON Text:
:   
``` json
{
    "name": "Translate",
    "type": 3
},
{
    "name": "Say Hello",
    "type": 2
}
```