Forked by numindast from ldirko - my first fork and attempt at actual for real work on sketches in Arduino.

TODO (wishlist):
 a) Investigate ways to wire up small display to show the names of the patterns/palettes ldirko chose as they rotate
   a1) using i2c?
 b) possible to use jcoon's fastled webserver for wifi control?
 c) possible to use rotary encoder, a la wled? maybe even RoenDi?

~~~~~~~~~~~~~~

This is firmware for Fibonacci 256 by Jason Coon with new and colorful effects.

Video how it looks in real life: https://twitter.com/jasoncoon_/status/1449162673346781187?s=20 

This sketch use button, but work without it in Automode by default

This sketch use one button to control patterns and bright. And esp32 M5 Atom lite with builtin button is ideal for this sketch (yes, i use Atom lite).
Attach button to pin what you want and gnd and chande default button pin to your pin.

Controls: 

Firm start with Automode ON and if button not press patterns change in loop. 

If one click button Automode is OFF and you can cnange next pattern by click button.

if button is double clicked bright is change in loop from 0 to max bright with 7 steps (i think this is best method to control bright). Double click not affect to Automode state.

If button is longpressed Automode id ON and patterns patterns change in loop because button not press.


Sketch used two libraries: FastLED https://github.com/FastLED/FastLED and OneButton https://github.com/mathertel/OneButton

And some words about what Fibonacci 256 is:

https://twitter.com/jasoncoon_/ autor

https://www.tindie.com/stores/jasoncoon/ buy it here


