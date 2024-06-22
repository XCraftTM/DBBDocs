icon: material/form-dropdown

# :material-form-dropdown: Select Menus

This Section will explain how to create and use Select Menus.


=== "String Select Menu"
    <h2> String Select Menu </h2>

    :   A String Select Menu, is the default Menu that can have anything selectable with Text, emojis and a Description.  
    Here is a Example for a Select Menu!  

    <h3> Creating the Select Menu </h3>

    :   This will create 3 Select Menu Options and each item gets added to a list that needs to be created extra.  
    The List then gets connected to the Create Menu Block.

    :   ![Create a Select Menu](https://i.imgur.com/eCnxLnU.png)  

    <h3> Reacting to the Select Menu </h3>

    :   The Select Menu uses the Interaction Event when used.  
    The `Options` Output returns the Selected Option Custom ID as a List, which can be gotten using the `get item from list`.  
    Then using the `Switch (Conditional)` you can make each Selected item do something else. In this Example Replying some Text!  

    :   ![React to Select Menu](https://i.imgur.com/jQM1q21.png)  

    <h3> Testing in Discord </h3>

    :   After you run your Bot you should be able to see your Menu using the Command of your choice. Once you select something, the bot should return a Message or whatever you set!

    :   ![Testing in Discord](https://i.imgur.com/wHJXAzL.gif)  

    ***

=== "User Select Menu"
    <h2> User Select Menu </h2>

    :   The User Select Menu is, again, much easier then the String Select Menu.  
    You just need one Block to create it!  

    <h3> Creating the Select Menu </h3>

    :   Use a Command, then create your Select Menu, then send that Menu. It can't get any simpler than that!  

    :   ![User Select Menu](https://i.imgur.com/2PFZ5Gg.png)  

    <h3> Reacting to the Select Menu </h3>

    :   Then use the `Interaction Event`, in Combination with `Get Item from List` to get the User.  
    Then Get the Information you need about the User and Reply back to the Interaction. 

    :   ![React to Select Menu](https://i.imgur.com/ZhiGRxV.png)

    <h3> Testing in Discord </h3>

    :   After you run your Bot, just use the Command and Interact with the Select Menu, then it should work...

    :   ![Testing...](https://i.imgur.com/5PWqPrv.gif)

    ***