# COMP210_2_interface_task

## Proposal and Market Research


Locomotion in VR is currently very limited. Some VR games like [Onwards](https://www.youtube.com/watch?v=f8N3aOn1iWE) simply use the Vive hand controller trackpads to move the player in the desired direction.

Other games like [Climbey](https://www.youtube.com/watch?v=Rhm_V__KUFo) and [Freedom Locomotion VR](https://store.steampowered.com/app/584170/Freedom_Locomotion_VR/)include movement options such as using a combination of arm movements and the grip buttons to simulate walking. Alot of games like [Gorn](https://www.youtube.com/watch?v=zFxfwKlforE)
include multiple movement options like these.<br/>
The main problem with these types of movement is they make fighting or using your hands in tandem with movement very difficult.<br/>
Because of this most VR games seem to have a basic instant point and click teleporting mechanic. Examples include Vanishing Realms, Arizona Sunshine, Sairento VR, The Gallery, Raw Data and many more. <br/>
These seem to be the most viable ways of implementing movement in VR currently, however immersion breaking they are.<br/>

Since teleporting is used heavily in most VR games, I wanted to design something based on the simplicity of teleportation but with something extra to make it seem more interesting.
My initial idea was to have a preview window of the view from the position you are about to teleport to. This would be really interesting in a strategic stealth based game as it would give you a window into areas before you teleport to them to survey the area.  <br/>
During my initial market research I discovered a game called [Budget Cuts](https://www.youtube.com/watch?v=n-bGfdK0k8Q) that already has this mechanic. <br/>

![Budget Cuts](https://www.cdkeyz.com/wp-content/uploads/2018/06/budget-cuts-pc-cd-key-4.jpg)

However, now I know that this mechanic can work, I am thinking of having other options attached to this idea. For example, I think an interesting idea would be having different teleports that also change the scale of the player after they teleport, perhaps shrinking or expanding the size of the player. In [Waltz of the Wizard](https://www.youtube.com/watch?v=pUvod-6VHbw) there is a spell that turns the player into a giant and in [Gorn](https://www.youtube.com/watch?v=ILw8TOGnd1U) the player can increase the height of the player in the settings. <br/>

A way this could be implemented is the use of a teleport gun with a finite number of bullets that each change the player size during teleportation based on the type of bullet in the teleport gun. The changing of bullet type could be simulated like the weapon changing in [Cosmic Trip](https://www.youtube.com/watch?v=Qv1PCbzJxWM) or like how [Space Pirate Trainer](https://www.youtube.com/watch?v=curX9Xe1kp0) changes gun type using a [radial menu](https://itroadblog.wordpress.com/2016/11/02/designing-embedded-menu-ui-for-vr-environments/) with the trackpad.
I could also include a mechanic that allows the player to pick up objects, these object when attached to the player would retain their size relative to the player. The resizing of objects could be an interesting mechanic for a puzzle game, with the player needing objects of different sizes to complete puzzles. Reminiscent of the ideas in Ant-Man. <br/>

## User Stories
As a player, I want to be able to teleport to a location I choose in the world. <br/>
As a player, I want to be able to switch realities (Blink) so I can solve puzzles. <br/>
As a player, I want to be able to see the other reality I'm about to Teleport to. <br/>
As a player, I want to be able to look around from the perspective of myself in the other reality. <br/>
As a player, I want to see how many times I have "Blinked". <br/>
As a player, I want to be able to collect items to progress the game. <br/>
As a player, I want to see how many items I have collected. <br/>
As a player, I want an obstacle to collecting the items in the rooms to add strategy to the game. <br/>
As a player, I want an alarm system that triggers when I enter the room, so I have an obstacle to overcome. <br/>


## Prototype Changes
My final prototype is somewhat different from my proposal idea. It no longer contains the player resizing and instead incorporates a reality switching mechanic. <br/>
The objective of the game is to move through a museum-like building and collect artifacts without being spotted by security cameras found in several of the rooms. In this regard it's similar to stealth games like [Thief](https://store.steampowered.com/app/211600/Thief_Gold/) and Dishonored. <br/> 
The reality switching mechanic allows the user to alternate between two different realities at will and realities also switch when the player teleports to a new location. The idea of a reality switch is something that is used in other games like [Titanfall 2](https://www.youtube.com/watch?v=luikI5DWaKg). In this case the player switches between different time periods rather than realities. In [Dishonored 2](https://www.youtube.com/watch?v=tyJ3Go4-nh8) there is an item that gives the player a view into another time period, my prototype is similar in that the player can see into another reality with the screens on the controllers. <br/>
![Dishonored 2 Timepiece](https://guides.gamepressure.com/dishonored2/gfx/word/82660717.jpg) <br/>
The idea being that the player can shoot a small sphere that acts like a [translocater](https://www.youtube.com/watch?v=KBA5EhbPxkc) beacon as in Unreal Tournament. While the sphere is in that position, the player can see (through the screen on the right hand controller) everything the player would see if they were to teleport there. This allows the player in the game to scope out the room before entering it in order to determine whether or not there is a security camera in the room and thus if the room is safe to enter. There are also doorways that are open in one reality but closed in the other, facilitating the need for reality switching in the game. There are a lot of possibilities with this mechanic, particularly in stealth/puzzle games. In the prototype, the aim of the game is to collect as many collectables as possible without trigggering any alarms and then find the Final Room of the level in as few "Blinks" as possible. <br/>
If I had more time I would have liked to add an effect to smooth out the teleport transition and pehaps make the screens on the controller better quality. Also the puzzle and gamification of the prototype, while demonstrating the core mechanics, are a bit simplistic.

## Resources Used
I used the free SteamVR 2.0 Plugin from the asset store to get the basic player gameobject and to get controller input actions working with my code and used an interactable sphere from the interactive sample scene as a base for my collectable objects. My teleportation code is my own that I made originally for my comp230 group project and repurposed for this project.

