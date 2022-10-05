# Parallaxer

A parallax system created to speed up parallax effects implementation in Unity projects.

## How this works?

The main tool in this asset is the ParallaxExpansibleElement, which will move copies of itself around
while following the camera at a relative speed set by the player.

In this case, the first step taken is to create copies of the element:

<img alt="GIF" src="https://github.com/SoftBoiledGames/Parallaxer/blob/main/Documentation/copies_spawning.gif" width= 600/>

Those copies will be then moved around if the camera attempts to exit the area covered with the copies:

<img alt="GIF" src="https://github.com/SoftBoiledGames/Parallaxer/blob/main/Documentation/copies_moving.gif" width= 600/>

There's also a moving element, the ParallaxMovingElement, which moves to direction with a speed, while also following the camera movement.

This element is also able to respawn itself at the opposite side of the screen as soon as its movement takes it outside the screen:

<img alt="GIF" src="https://github.com/SoftBoiledGames/Parallaxer/blob/main/Documentation/moving_element.gif" width= 600/>

The last element of this list is the static element, the ParallaxStaticElement, which will keep following the target camera with no offset:

<img alt="GIF" src="https://github.com/SoftBoiledGames/Parallaxer/blob/main/Documentation/static_element.gif" width= 600/>

## Cool! How do I use it?

- First, create an object which will parent the parallax elements. Add to it a ParallaxManager component
- Then, add your parallax elements as children os the ParallaxManager object, setting the sprites sorting orders accordingly
- Set the speed of each parallax element as you wish
- That's it! No additional coding needed!

Graphic assets made by Kenney:
- https://kenney.nl/assets/background-elements
- https://kenney.nl/assets/simplified-platformer-pack
