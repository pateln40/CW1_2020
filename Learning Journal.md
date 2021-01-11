

**9/09/2020**
There was an issue with one of the scripts when the player collected the honey, the UI wouldn’t go down to 0 instead it would stay at 1. The UI should’ve countdown from 5 to 0, which would show how many collectables they had left. This is waht the script was like before.

    public void UpdateUI() 
    {
        if (cur_coins > 0)
        {
            coinsLeft.text = "Honey    " + cur_coins.ToString ("D");
            
            
It was something I couldn’t ignore because the player wouldn’t know if they collected all  objects in the maze.
It took a couple of hours to think of why it wouldn’t work since the script looked fine, however I realised that I missed a couple of lines of code.  And this finally made the UI Countdown to 0 and trigger the door. 

  
    public void UpdateUI() 
    {
        if (cur_coins > 0)
        {
            coinsLeft.text = "Honey    " + cur_coins.ToString ("D");

        }
        else if (cur_coins <= 0) {
            coinsLeft.text = "Honey    " + cur_coins.ToString ("D");
            Door.SetActive (true);
        }

    




