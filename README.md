# GDIM 33 In-Class Activities
## W1
### Activity 1
[Mood Board](https://docs.google.com/drawings/d/137NF1I_z6MVHimet8F8JeoYGWbEKrYcGnjdGF0K_KmU/edit?usp=sharing)
1. The patterns that are emerging from my inspiration sources are the unknown and the dark. The mechanic that I like to use in horror games is being able to move around a building and using cameras to get information. I am also really interested in low poly like PS1 graphics because they are used in one of my favorite games, Fears to Fathom.
2. We both want monsters in our game but in my game I want to avoid my monster as much as possible while my table mates want there to be full on confrontation and combat while I want to outsmart my monster.
3. The table LA Eric really likes to play shooter games and I am not too much a fan of them but I like the strategic part of those games. I do have in common that I also liked to play overwatch even though it has been awhile since I last played.


### Activity 2
<img width="960" height="720" alt="GDIM 33 Breakdown" src="https://github.com/user-attachments/assets/408ba7ca-3a06-4675-9881-1d11ba42ce33" />



## W3
### Activity 1
<img width="1275" height="743" alt="GDIM 33 Breakdown" src="https://github.com/user-attachments/assets/64cb7321-8ed8-4cfc-8e3a-69bd19a7e1a9" />

### Activity 2
1. It is advantageous to save the event name for the explorer to dialogue state transitions as the scene variable “clickNpcEventName” so that we could access it in the walrus graph to start the transition. It could also help in trying to set up future NPC’s as we can just trigger that same event throughout the scene.
2. The way that one debug.log helped me test my graphs was that it helped me notice that the transition was not transitioning because the debug.log was not activating. This allowed me to fix the way the custom event trigger was triggering because it was not triggering the transition like it was supposed to.
3. Yes the set cursor lock state is relevant to my vertical slice as I want there to be movement with the cursor locked and then be able to pull up a tablet and use your mouse to click things so it will be useful to move between those two states.
4. Yes, the concept of the “game state” is relevant to my vertical slice as it will help me control how my player moves and interacts with objects and also how my monster will move around depending on the specific game states it has.

## W4
### Activity 1
1. What is playable right now is that there is a monster that chases you and you are able to run away. You can both move and look around and there is a timer that will count down and if it reaches zero the player wins. But if the monster touches the player the player loses.
2. I am testing to make sure there are no bugs in the movement, camera controls, and monster collision.
3. The playtest went well nothing went wrong all the collision triggered correctly although the timer glitched a bit it was an easy fix. Of course with this prototype it was not that difficult but it was a playable game I think keeping the player at one speed but allowing the monster to speed up might be better in the long run.
4. Nathan H., Kai M. Marcelo TET.


### Activity 2
1. I do think that a writer could write more dialogue as long as they know their way around the game engine. This is because creating the dialogue is entirely in the game engine after the code is set up.
2. I do not think there is a limit to creating dialogue nodes but it might become very convoluted the more you have to make reply wise. But theoretically it could be done just not as efficient. This reminds me of how most of the dialogue in undertale is in one if statement, inefficient but it works.
3. It refreshes the library of nodes so that they can be refreshed and also it allows newly added nodes to be accessed in script machines and graphs.

## W5
### Activity 1
1. Create a navmesh for the monster to track the player
   a. Create and bake a navmesh that allows walking through hallways
   b. Have it track the player and follow them
   c. Have it update every frame so that it can follow the player when they move
2. Have the monster speed up when it reaches a specific radius close to the player and make it chase
3. Create monster control StateMachine with the categories of Chasing the player, breaking light, running away from light, and wandering.
4. Finish making a map for the player and monster to roam around in.

## Activity 2
Today in class I created a navmesh for my monster instead of the usual scripting graph that would just transform itself to follow the players position I now have set it up through navmesh of the terrain. This helps me in the future as it will help my monster go around walls unlike how my last one was working. I had an error in the beginning where I couldn't tell why my navmesh surface was not baking correctly but I got it working. But right now I have replaced all the code that controlled movement with navmesh and I also got my lose condition working again on the monster.

Continue adding additional headers below this one for future weeks and future activities.
