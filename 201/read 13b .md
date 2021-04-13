# ***Read: 13b - CSS Transforms, Transitions, and Animations***
- - -
## Transforms
The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

### Transform Syntax

#### 2D 

* ***Rotate*** provides the ability to rotate an element from 0 to 360 degrees , The default point of rotation is the center of the element    
example transform: rotate(20deg);   
 
* ***Scale*** change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear large   
example   transform: scale(.75);    
we can also use scale x and scale y       
example  transform: scaleY(1.15);    transform: scale(.5, 1.15);   

* ***Translate*** pushing and pulling an element in different directions without interrupting the normal flow of the document    
 example  transform: translateX(-10px);  transform: translateY(25%); transform: translate(-10px, 25%);

It is common for ***multiple transforms*** to be used at once, rotating and scaling the size of an element at the same time for example.    
example   transform: rotate(25deg) scale(.75);    

* ***Transform Origin***  To change the default origin position 
examples transform-origin: 0 0;  transform-origin: top left; transform-origin: 20px 50px;    

there are many other 2d and 3d proparites we can change .   
    
- - -
## Transitions & Animations

Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

### Transitions

There are four transition related properties
* ***transition-property*** determines exactly what properties will be altered in conjunction with the other transitional properties

* ***transition-duration*** The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms).  

* ***transition-timing-function*** used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration.       

* transition-delay

Any properties included when changing an element’s state, but not included within the transition-property value, will not receive the transition behaviors as set by the transition-duration or transition-timing-function properties.    
not all properties may be transitioned, only properties that have an identifiable halfway point.    


### Animations

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
