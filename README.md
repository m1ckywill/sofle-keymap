# sofle-keymap
Built myself a gorgeous Sofle v1.1 split ergo mech keyboard - now time to customise the keymap!

JSON file is direct from the VIA webapp, you need to have the VIA firmware loaded first before you can load it.
From the default QMK environment, use the following command to flash the most recent version for the Sofle:

```
qmk flash -kb sofle -km via
```

I've also adjusted the TAPPING_TERM time to 250ms within qmk_firmware/keyboards/sofle/rev1/config.h as I found I was getting all sorts of false triggers for "holding" when trying mod-taps on the thumbs.


## To Do List
- [ ] Number pad on layer 2 right hand.
- [ ] Move control to outside column, remap other keys elsewhere.
- [x] Consider using the hold mod option on space and enter

Done, implemented for testing and enjoying so far. I've used the ANY assignment option under the Special keys section within the VIA keymap section with the following code: LT(3,KC_ENT). You have to use LT as a workaround based on my research as MT in this section won't save.
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
