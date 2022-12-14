# sofle-keymap
Built myself a gorgeous Sofle v1.1 split ergo mech keyboard - now time to customise the keymap!

The JSON file in this repo is direct from the VIA software (webapp or desktop, I've found desktop works better for me but YMMV).

You will need to have the VIA firmware loaded first before you can load a VIA keymap.

> I've adjusted the TAPPING_TERM time to 250ms within ```qmk_firmware/keyboards/sofle/rev1/config.h``` to suit my personal typing habits.

> This was done to counter all sorts of false triggers for "holding" when trying mod-taps on the thumbs. For whatever reason the default on the Sofle is 100ms instead of the QMK default of 200ms.

From the default QMK environment, use the following command to flash the most recent VIA firmware version for the Sofle:

```
qmk flash -kb sofle -km via
```

## Current To Do List - Feel free to make a Pull Request to solve any of these
- [ ] Number pad on layer 2 right hand.
- [ ] Move control to outside column, remap other keys elsewhere.
- [x] Consider using the hold mod option on space and enter

Done, implemented for testing and enjoying so far. There's a standard mod-tap for SPACE, however for ENTER I've used the ANY assignment option under the Special keys section within the VIA keymap tool with the following code:
```LT(3,KC_ENT)``` 

> You have to use LT (for Layer Toggle) as a workaround based on my research as MT in this section won't save. For example, this one will toggle layer 3 while held but return ENTER when tapped.
- [ ] Dedicated cut/copy/paste/excel "paste special" macros
- [x] Macro for Task Manager to maintain muscle memory for standard keyboards.

Done, implemented for testing on Layer 2. Have it mapped to both the original Layer 2 mod for Layer 0 (just inside of the left thumb) as well as Layer 0 TAB (3rd down outside left column left hand).


## LAYOUT DESCRIPTION

**Layer 0:**

Default layer, QWERTY, with minor basic changes to locations on ctl/alt/win/space/enter/bkspc/esc to suit my preferences.

Changes to layer mods in testing

**Layer 1:**

Colemak layout, with minor basic changes to locations on ctl/alt/win/space/enter to suit my preferences.

**Layer 2:**

Not happy with this layer currently, will leave function keys on here but want to move all sorts of things around (see to do list)

**Layer 3:**

TBC - currently arrow keys is all that will stay here. Possibly will move different brackets to this layer? 
