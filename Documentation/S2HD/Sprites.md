# S2HD Internal - Sprites

* This is me documenting how sprites work in Sonic 2 HD!

So apparently theres 2 png files, BODY.png and SKIN.png.

The BODY.png contains well... the body of whatever object, and the SKIN.png contains the skin.
If we use Sonic for instance, his BODY.png contains his body, eyes, ears, and shoes. It also contains the little effect around his hands when he's balancing. While his SKIN.png contains the blue-ness and his spindash.

There's also another file called ANIGROUP.anim, .anim files are just xml files.

The xml contains tags for the texture, animations.

Inside of the animations theres comments for each animation (thank the lord.). 
Anyways theres delay and y(?)offset for the animation:

```xml
<animation delay="4"  offset_y="-4"> <!-- Taken from the wait animation -->
```

In some animations, for instance, the lookUp animation, it has an extra tag called "loop":

```xml
<animation delay="3" loop="2" offset_y="-4">
```

Which I'm assuming just loops the first two frames?? (I am most likely wrong.).

Inside of the animation tag it has the frame tag, which is for the frames.

The frame tag has the x (axis??), y (axis??), width, and height of the animtion.

I plan to making a tool to be able to view them better and to make your own!