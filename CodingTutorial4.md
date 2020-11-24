# Health/Heart System

- In this tutorial we will be making a health system in Unity, we will need a empty heart and a full heart sprites. Create a UI canvas and make sure the scale mode is set to **scale with screen size** so the UI will scale to the aspect ratio.

- Create a UI image and drag the heart sprite into the empty sprite slot, once that is done duplicate as many hearts as you like into the scene.

- Insert a new Script called **health** and insert a **public int health and int hearts** at the top of the script, so when this is equal to one we should only have one heart container visible in the scene. Make sure to type in **Unity Engine UI at the very top of the script.**

- Insert the variables called **full heart**, it should look like this. 

      public Image [] hearts;
      public Sprite fullheart;
      public emptyHeart;
      
 - Back into Unity, we will create a empty object and name it **player** and drag our **health script** into it. Insert a default value for health qand drag and drop the empty heart images in the empty slots in the inspector.
 
 - under the void update insert the following.
 
        for ( int i = 0; i hearts.Length; i++) {
         if (if < numOfHearts){
           hearts [i].enabled = true;
         } else {
            hearts [i].enabled = false;
