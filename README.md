# All The Fishes
Things that are happening:

## four floating fish
There are four fish that are facing in different directions, which was done by multiplying their scale in the x-direction by -1. They are animated in a way that makes them look like they are floating and bobbing in the water. Each are bobbing at different speeds and directions. I made slight variations to this formula to create different "wobbles".
```javascript
let wobble = Math.sin(time / 1000) * 10;
let wobble2 = Math.sin(time / 500) * 5;
let wobble3 = Math.sin(time / 200);
```
## school of fish
I made a school of fish by making 7 fish sprites and putting them all in one container. I have the fish in random positions, but all within a 100 x 100 px area. 
```javascript
fish.position.set(Math.random() * 100 + 100, Math.random() * 100 + 100);
```
In the animation loop I have the school move across the canvas by increasing the container's x position every frame. In addition, I added a wobble to the school's y position so they squiggle across the canvas rather than just move in a straight line.

Finally, I have an if statement that checks to see if the school of fish reached the end of the canvas. If so, I reset the x position to 0 and randomly choose a y position for the school to enter the canvas at. In addition, the individual fish are in new, random positions in the 100 x 100 box. 

## bubbles
I did a similar thing with the bubbles. I have them scaled at random sizes and starting at random x and y positions. Every frame they float up the canvas, and when they reach the end, the bubble's y position is set to 0 and it's x position and scale is randomly generated. So, it looks like new bubbles are forming and floating up.

## swimming fish
For the lone swimmer, I have the fish move across the canvas and once it reaches one of the edges it will turn around and swim back. To do this, I made a boolean variable called forwards so that when it is true, the fish moves one way, if it is false, it moves the other way. I change the variable when the fish reaches one of the edges, as well as flip the fish by negating the scale in the x direction (like I did with the floating fish). 


## img attributes:

- Four big fish image

undersea animal PNG Designed By 588ku from https://pngtree.com/freepng/fish-cartoon-fish-colored-fish-animal_3855774.html?sol=downref&id=be

- background coral reef image

https://www.pngwing.com/en/free-png-buzjv

- bubble image

<a href="https://www.freeiconspng.com/img/44336">water bubble png</a>

- lone swimming fish
<a href='https://pngtree.com/so/hand'>hand png from pngtree.com/</a>

- star
Husein Aziz, CC BY 3.0 US <https://creativecommons.org/licenses/by/3.0/us/deed.en>, via Wikimedia Commons