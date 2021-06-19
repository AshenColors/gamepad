This branch adds configurable SOCD cleaning that is stored in EEPROM.
The default is the usual hitbox L+R=N, U+D=U.

The default configuration button is START+SELECT+L3+R3. You can also short pin 7 to ground or wire it up to a dedicated button.

Configuration is performed by pressing the config button/combination, holding down input directions, and then releasing the configuration button. Left and right are evaluated as the "X" axis, and up and down as "Y", and each is configurable separately.

- If no buttons are held down, simultaneous inputs output neutral. This is the default L+R behavior for hitbox-style controllers.
- If one button is held down, that button will take priority when simultaneous inputs are made. This is the default U+D behavior for hitbox-style controllers (up takes priority).
- If both buttons are held down, the last input will take priority. (Also known as second input priority)

More about these modes can be found here: https://www.hitboxarcade.com/blogs/faq/what-is-an-socd

There's a basic wear leveling algorithm in use, so I think it's safe to say that this design will last the lifetime of the board.

---

# Arduino PC/PS3 compatible gamepad

This is Arduino code for making a gamepad using an ATmega32U4-based board.

Tested with an Arduino Pro Micro, works out of the box with at least PC and PS3.

[See here](https://www.thingiverse.com/thing:4838081) for an example of a controller made using this code.
