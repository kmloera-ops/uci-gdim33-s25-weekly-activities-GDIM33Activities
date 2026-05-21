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

### Activity 2
Today in class I created a navmesh for my monster instead of the usual scripting graph that would just transform itself to follow the players position I now have set it up through navmesh of the terrain. This helps me in the future as it will help my monster go around walls unlike how my last one was working. I had an error in the beginning where I couldn't tell why my navmesh surface was not baking correctly but I got it working. But right now I have replaced all the code that controlled movement with navmesh and I also got my lose condition working again on the monster.


## W6
### Activity 1
1. What is new in my build is lights repelling, monster navmesh, new map, and controlling whether lights turn on and off. I also changed how fast the player and monster move, making the monster move faster than the player. I also added a cooldown on the lights so that the player cannot spam them.
2. [Itch Playtest 2](https://kmloera-ops.itch.io/playtest-2-vertical-slice)
3. My playtesting goals are to make sure my navmesh is working correctly, see how players use the lights to avoid the monster, and test that the lights correctly repel the monster away. I need to see if there are any bugs with my light repelling the monster and if there are any improvements I can make upon it. Also it would be interesting to see what playtesters think of the current map and how it can improve. I also changed how fast the player and monster move to make the monster more menacing. I want to see if the cooldowns are good enough for the players or if its too hard or easy.
4. Playtesting Notes: During the playtests players were unsure of where the lights were and it caused some confusion of them thinking they had a flashlight. They also weren’t sure when they could turn the lights back on so it might be good to have an indicator showing that the lights can be turned back on.

### Activity 2
1. The reason that the multiply setting of the blend node makes the resulting color darker and less saturated than the input colors is because the lower the RGB values get the closer they get to just being a solid black. This usually happens when decimal values are multiplied together they get smaller.
2. I think if we were to multiply alpha values the result would be more translucent because it is going down the spectrum making it look less opaque. This is because alpha values are also stored between 0.0 and 1.0.
3. The shader gets these UV coordinates from the mesh as it has UV coordinates stored within the model.
4. I always knew that this was possible so I guess I am not surprised or more interested in it but I might enjoy making lighting have a specific effect on objects.


## W7
### Activity 1
1. I believe that the vertex color node would get its data from the original mesh.
2. The color on our shiba from step 3 is blended at the edges of different regions of colors because it uses the (x,y,z) coordinates of the mesh as surface normals for the (r,g,b) values.
3. The reason it is less detailed than the shiba is because vertex colors are less detailed than texture colors. I can imagine that vertex coloring is good for simple applications and optimization.
4. On the back of the dog there is a random green spot which I believe should not be there in the mesh’s vertex normals.
5. One other piece of vertex data that we can test with a debug shader like this is the lighting. This can be useful to see how the lighting will affect the shadows of specific models such that it looks natural according to where the light is in accordance with the model.
6. There is an error in the lighting in step 4 on the back of the shiba because that specific part of the shiba’s mesh has a normal value that is negative to the rest of the shiba’s back.
7. The reason the blend mode uses additive instead of multiplicative is because multiplicative would multiply the values and make the shader material darker while additive allows it to stay transparent and full of color.


## W8
### Activity 1
#### Playtest Goals:
1. Test the Button UI
2. See what improvements players could suggest in gameplay for using buttons
3. Test how strong/weak the lights are in helping the player
4. See about what could be made to make the game more beginner friendly
5. Test the new Exit mechanic
#### Whats New:
What is new in my build, since my last milestone, is that the map is now bigger, more lights have been added, and also a new way of winning has been added and that is to get to an exit door.
#### Feedback:
The feedback I received was a lot. First it was that there was no indication of the monster getting closer and the buttons do not show what lights they turn on so you have to kind of guess. Then also some mentioned that the mouse sensitivity was too high. Players said they didn't have enough time to get to the exit and it was better to just wait out the timer. A very big suggestion was to just work on setting up audio or visual cues to show that the monster is getting closer without the player having to look behind them. Otherwise players said that the game was fun and that they can’t wait to see what it would look like with good UI and visuals.

[Itch Link](https://kmloera-ops.itch.io/playtest-3)

## Activity 2C
1. The pass associated with the post processing effect is the FullScreenPass. Then the way we can tell is because the shader we created affects the whole screen.
2. The way that the screen looks if it is 0.5 is it has the texture but not really any of the red color. At 0 the texture completely disappears. Then at 1 it is very apparent over the screen but it is slightly see through so that you can see the tomato cat.
3. What this value decides is which one is more dominant over the other so at 0 it is the original image at 0.5 it is split between both and at 1 it shows mostly the shader but you can still see the other because it is slightly translucent.
4. The reason that we use (sin(time)+1)/2 is because we need values between 0 and 1 while regular sin(time) gives us values between -1 and 1. This way when we add 1 it keeps the range between 0 and 2 then dividing it by keeps the range between 0 and 1.


Continue adding additional headers below this one for future weeks and future activities.
