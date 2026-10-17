# gadgets-colorsystem

ColorSystem for the gadgets of [polpo](https://github.com/polpo-system/polpo): a panel that shows
the colours of the display palette, changes them, and loads and stores palette files (*.Pal).

```
portia.Install gadgets-colorsystem
```

## Using

    Desktops.OpenDoc ColorSystem.Panel    the panel; Load and Store read and write the palette
                                          file named in its text field

## What is here

    src/ColorSystem.Mod        the colour model and gadget
    share/ColorSystem.Panel    the panel
    tools/ColorSystem.Tool
    test/ColorSystemTest.Mod

The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to plain
text; the first commit has it unchanged. It compiles unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS).

## Tests

    ColorSystemTest.Run      3 checks: the model and the gadget made, the panel opened; it needs
                             the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
