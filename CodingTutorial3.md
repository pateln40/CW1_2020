# Player Movement


- For this tutorial we will be creating a player movement that is top down, this means we will be creating movement for up, down, lef and right. To start of we will need to insert one asset for the player, to do this you will need to go to **assets** followed by **import assets** this will allow you to pick your image for your player in the scene. 

-Once that is done we will drag the asset into the scene and name it **Player**. Under the **inspector** for the Player, we will add a **rigid body 2D** which will enable physics onto the object. Still under the inspector, we will adjust the **Gravity scale** to **0** so the player doesn't fall down and under **constraints** we will also freeze the rotation on the **Z** to make sure the player doesn't rotate. 

-Once that is done, we go to **add component** and create a **new script** for the player movement. Double click and this will lead you to visual studio. 

- Into visual studio we need to remove the **start method**, instead will we add some **variables**. Now we need to define for the movement speed, for that we will write our first line of code. We will create a public float, with the speed of 5 for now. 


      public class PlayerMovement : MonoBehaviour
      {

      public float moveSpeed = 5f;
