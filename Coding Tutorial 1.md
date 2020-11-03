# Timer Tutorial 


For this tutorial we will need two assets for this project, one for the player and one for the enemy. To insert your assets you will need to click on Assets and click on **ImportNewAssets**. 

This will let you access your **folders** , from there you will need to select the assets you will need for this Tutorial. 

Once the assets are inserted into the UnityProject, drag the assets into the **Hierarchy**. You will need to label one Enemy and one Player. Just right click on the asset in the Hierarchy and this will allow you to change the name of the asset. 

Once that is done, we will need to create a Script for the Enemy. Click on the Enemy, under the Inspector you will need to click on **Add Component**. Search Up New Script, which will enable you to add a script for the Enemy. Name the Script Enemy.

The first thing we want to do is calculate the **direction** our player is compared to our enemy object in order to do that we need to create a reference for our player object in the script. 

So for the top write public **Transform player**. Then in the update function which is executed every frame, we need to calculate the direction by writing **Vector3 direction = player.position - transform.position;**

Make sure you add a **Rigidbody** to the Enemy, to do this you need to select the Enemy and under the Inspector, add a **Rigidbody 2D** component since this is 2D. 
Back to the script, you will need to create a reference to the RigidBody 2D up at the top by writing **Private RigidBoody 2D rb.**

In the start function, you will need to define the rb, this will allow you to manipulate the movement and rotation of our object.
