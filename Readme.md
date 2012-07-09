Written by Richard Goulter <richard.goulter@gmail.com>, 2012
Feel free to use, modify and/or distribute the above code as you wish.
The code is provided "as is", all implied or expressed warranties are disclaimed. I hold no responsibility for any harm or damages caused by usage of this code.

This code is to demonstrate an example of HTML5's Canvas and JavaScript, in a manner one might use them for a game.

In the demo, a small arrow-like shape acts as a player avatar, and can be controlled by the keyboard. This avatar can shoot bullets. Several asteroid objects are also in the demo. Collisions can be detected and responded to in the code.

The demo is programmed in JavaScript in an HTML page, and all rendering occurs using the HTML5 Canvas.
For convenience, the JavaScript Objects for this demo have been separated into different files.
 * Geometry.js - contains the Geometry object, which has useful methods for collisions.
 * MovingObject.js - contains an object which maintains an x, y, and a velocity of an object.
 * RenderablePolygon.js - contains an object which maintains a polygon which can be rendered. Also handles collision using this polygon.
 * GameObjects.js - contains Asteroid, Bullet, Explosion, and SpaceShip objects, which script the specifics of the game object behaviour.
 * GameEngine.js - contains the GameEngine object, which controls the game flow of the demo, and handles input, game object management, etc.
 * aster.html - contains the demo, combining the different aspects of the demo together.

For simplicity, all collisions in this game are done using polygons, and naive polygon intersection-detection algorithms. This is, at the moment, done within the RenderablePolygon object.
 
An example of the demo, or a similar version, can be found at http://rgoulter.com/aster2.html or http://rgoulter.github.com/aster/aster.html

The reader may feel free to try to extend or add features to this demo. Examples of such things include:
 * Adding more asteroids when all asteroids are gone.
 * Aesthetic features, e.g. adding a 'flame' animation when spaceships are moving, rotating asteroids.
 * AI for a Spaceship.
