# al-game-chy
Al-Game-Chy A List of Game Dev Ingridients

⛯ Gravity ⛯

    #Staying on the Ground

    velocity.y = input_direction.y * gravity

    #Falling To The Ground

    velocity.y += input_direction.y * gravity

☍ Where to Change State ☍

    If State Change is Based On Physics Condition
        Change State on the Physics Loop
    If State Change is Based On Player Input 
        Change State on the Input Loop
    If State Change Involves Both Physics and Player Input
        Change State on the Physics Loop
        But Send the Player Input to the next state
        Allow the next State to Adopt The Player Input From the Previous State
