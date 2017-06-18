---
title:  "AngleTools.js"
---
I made a thing called AngleTools.js.

It is used to calculate angles and movements with x,y coordinates

{% highlight javascript %}
const at = {
	angle: (a,b)=>Math.atan2(b.y-a.y,b.x-a.x)/Math.PI*180,
	dist:  (a,b)=>Math.sqrt((a.x-b.x)*(a.x-b.x)+(a.y-b.y)*(a.y-b.y)),
	step:  (a,s)=>({x:s*Math.cos(a*Math.PI/180),y:s*Math.sin(a*Math.PI/180)})
}
{% endhighlight %}

### angle

Calculate the angle between two objects in degrees. Both objects need to have x and y properties.

Eg.
{% highlight javascript %}
var obj1 = { x: 100, y: 100 }
var obj2 = { x: 200, y: 200 }

var angle = at.angle(obj1, obj2) // 45
{% endhighlight %}


### distance

Calculate the distance between two objects in a straight line in pixels. Both objects need to have x and y properties.

Eg.
{% highlight javascript %}
var obj1 = { x: 100, y: 100 }
var obj2 = { x: 200, y: 200 }

var distance = at.dist(obj1, obj2) // 141.4213562373095
{% endhighlight %}


### step

Calculate the x and y changes needed to move an object a certain distance along a certain angle.

Eg.
{% highlight javascript %}
//              angle, distance
var step = at.step(45, 200)

obj1.x += step.x
obj1.y += step.y
{% endhighlight %}