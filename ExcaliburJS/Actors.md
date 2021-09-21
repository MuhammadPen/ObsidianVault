### Actors
Actors must be added to a [[scene]] to be drawn or updated! `game.add(actor)` Will add an actor to the current scene.

Actors can be given a position, width, and height.

```ts
// Create an actor with x position of 150px,
// y position of 40px from the bottom of the screen,
// width of 200px, height and a height of 20px
const paddle = new Actor({
  x: 150,
  y: game.drawHeight - 40,
  width: 200,
  height: 20,
});

// Let's give it some color with one of the predefined
// color constants
paddle.color = Color.Chartreuse;

// Make sure the paddle can partipate in collisions, by default excalibur actors do not collide with each other
// CollisionType.Fixed is like an object with infinite mass, and cannot be moved, but does participate in collision.
paddle.body.collider.type = CollisionType.Fixed;

// `game.add` is the same as calling
// `game.currentScene.add`
game.add(paddle);
```

*Actors have a default anchor of (0.5, 0.5) which means their graphics are positioned in their center (not top-left) by default.*