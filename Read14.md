# CSS Properties
1. Transform 
* It is a css propery that allows us to change and alter the position of elements. 
* It had two settings: **2D** and **3D**.
## 1.1 2D:
### Values:
1. rotate: it rotate elements between 0-360 degrees.
```
.box-1 {
  transform: rotate(20deg);

```
2. scale: it changes the appeared size of an element. 

```
.box-1 {
  transform: scale(.75);
```
* Notes: The `scaleX` value will scale the width of an element while the `scaleY` value will scale the height of an element. 

3. Translate: it pushes and pull an element in different directions without interrupting the normal flow of the document.

```
.box-1 {
  transform: translateX(-10px);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: translate(-10px, 25%);
}
``` 
4. skew: it distorts elements on any axis or both.

```
.box-3 {
  transform: skew(5deg, -20deg);
}
```
* Note: We can combine transforms:
```
.box-1 {
  transform: rotate(25deg) scale(.75);
}
.box-2 {
  transform: skew(10deg, 20deg) translateX(20px);
}
```
* Note:
The default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the `transform-origin` property may be used.

## 2. 3D:
* In order for three-dimensional transforms to work the elements need a perspective from which to transform.
* To chanege perspectve: Either use the *perspective value* within the transform property on *individual *elements OR use using the *perspective property* on the *parent* element. 
```
.box {
  transform: perspective(200px) rotateX(45deg);
}
```
### Values:
1. It uses the rotate value same as 2D.
2. Scale: we scale the Z axis.
```
.box-1 {
  transform: perspective(200px) scaleZ(1.75) rotateX(45deg);
}
``` 
3. translate: we translate the z axis.
4. Skew: cannot be use in 3D. 
## The transform style property
* It needs to be placed on the parent element above any nested transforms.
## Values:
1. **The preserve-3d**: it allows the transformed children elements to appear in their own three-dimensional plane.
2. **The flat value**: it forces the transformed children elements to lie flat on the two-dimensional plane.
## Backface Visibility
Some 3D elements sometimes face away from screen. We can set the backface-visibility property to *hidden*, to hide the element whenever it is facing away from the screen. otherwise, the default value is *visible*.
## CSS Transitions 
we alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
### Properties
1. transition-property: it determines exactly what properties will be altered in conjunction with the other transitional properties.
2. transition-duration: The duration in which a transition takes place. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). They may also come in fractional measurements, .2s for example.
3. transition-timing-function: it is used to set the speed in which a transition will move.
4. transition-delay: sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing.

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```
* Shorthand transition: `transition: background .2s linear, border-radius 1s ease-in 1s;`
## Animations
The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
```
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
}
```
* to repeate animations, use `animation-iteration-count` property.
* to declare the direction an animation completes, use the `animation-direction` property.
* The `animation-play-state` property allows an animation to be played or paused using the running and paused keyword values.
