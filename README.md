# Phaser Gamepad +
This project is a plugin for [Phaser](https://phaser.io) that attempts to make easier for handling different forms of input in a uniform way. Given the desired mapping of input might differ on a per project basis, configuration is needed upon startup.

---

## Reason for this project
With all different devices that are capable of running games, there is a whole plethora of input methods. This includes, but is not limited to: 
- multi-touch, possibly with gestures
- mouse movement, clicks, and scrolling
- keyboard button presses
- sticks and buttons on a gamepad / joystick

There are hardly any devices (if at all) that support all methods. Most of them however have a method that can be easily mapped to a single point on the screen. [Phaser](https://phaser.io/) already does this with the mouse cursor and single-touch. While practically any application can be made workable with this kind of input, it might not be preferable. 

Choosing any single other type of input makes it so less devices are supported out of the box. Making the application (partially) unusable on them, unless another input method common among those devices gets supported as well. This either requires that all different tests based on the input are performed everywhere, in which case it is easy to accidentally skip one place. Or create a mapping on which all tests are performed, where certain types of input might work less convenient than if they were handled separately. It means more work for the developer either way. 
