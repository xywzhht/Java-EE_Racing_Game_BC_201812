# Racing games based on Java EE -- speed revolution

This is a racing shooting game, you have a luxury sports car, you can shoot bullets, defeat the enemy, different levels have different scenes, your car will be different.

Basic requirements of the game:

1. The main character's car attack √

2. Mobile attack of enemy racing car √

3. Mobile attack of boss √

4. Move and switch the background picture √

Requirements for the game:

1. Multiple enemy roles, multiple NPCs √

2. Multiple items dropped √

3. Set multiple levels √

### Environmental configuration

Operating system: Microsoft Windows

Program language: Java

Development package: Java JDK 1.8.0 development kit

Development tool: Eclipse



### Rules of the game
![Image](https://github.com/xywzhht/xywzhht.github.io/blob/master/KillerCar/img/01.png)

### Frame design
![Image](https://github.com/xywzhht/xywzhht.github.io/blob/master/KillerCar/img/02.jpg)


### Innovation point: background rolling
The reason why a car becomes a car is that the car is moving. In this game, in order to achieve the effect of racing, the effect of rolling from the background is reflected. 
In order to achieve a better effect of background rotation and rolling, in order to truly move the car in the actual game process, the project innovatively modified the method, defined two img objects with the same background map, staggered moving with the refresh of the thread, truly realize the seamless connection of the background map, and create a good game experience for the players.

### collision detection
A very important place in the game is collision detection, which is mainly the collision judgment between the protagonist's car and the enemy, and between the protagonist and other characters in the game.

In this game, because the driving is based on the track, the car and driving will not collide with the scenery beside the track, so the collision detection between the player's car and driving is mainly considered here.

We know that when two vehicles run in parallel, the horizontal distance between them is small to a certain extent, they can be considered to have collided. When the longitudinal distance between them is small to a certain extent, they can be considered to have collided.

This game checks the X, y coordinates of two cars to determine whether the two rectangles intersect to determine whether the collision occurs. After the collision, different collision effects will be set according to the role identities of the collision parties.

### Game interface
Game launch interface
![Image](https://github.com/xywzhht/xywzhht.github.io/blob/master/KillerCar/img/03.png)
Game ending interface
![Image](https://github.com/xywzhht/xywzhht.github.io/blob/master/KillerCar/img/04.png)
Game allowed interface
![Image](https://github.com/xywzhht/xywzhht.github.io/blob/master/KillerCar/img/05.png)
