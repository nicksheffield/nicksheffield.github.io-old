---
layout: post
title:  "Mouse.js"
post_class: post-template
---
Easily get mouse position and movement values.

---

### Install

Download [Mouse.js](#)

```
npm install mouse-js
```

```
bower install mouse-js
```

---

### Use

#### `Mouse()`
A factory function that returns an instance of the mouse object

#### `mouse`
A global instance of the Mouse factory

#### `mouse.relativeTo(element)`
Returns a new mouse object, with offset's set to match given element

---

### Position

#### `mouse.x`
#### `mouse.pos.x`
The current X position of the mouse

#### `mouse.y`
#### `mouse.pos.y`
The current Y position of the mouse

#### `mouse.xO`
#### `mouse.old.x`
The previous X position of the mouse

#### `mouse.yO`
#### `mouse.old.y`
The previous Y position of the mouse

---

### Movement

#### `mouse.xV`
#### `mouse.vel.x`
The horizontal distance in the last movement

#### `mouse.yV`
#### `mouse.vel.y`
The vertical distance in the last movement

#### `mouse.aV`
#### `mouse.vel.angle`
The angle travelled at in the last movement

---

### Misc

#### `mouse.offset.x`
Subtracted from x values. Set when using `mouse.relativeTo()`

#### `mouse.offset.y`
Subtracted from y values. Set when using `mouse.relativeTo()`

#### `mouse.at`
An object containing angle calculation functions

#### `mouse.evt`
The most recently captured mouse event