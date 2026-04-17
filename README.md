# christmas-trees

Simple light-up Christmas tree ornaments.

This was a practice project for learning Altium Designer and practicing PCB design, board bring-up, and debugging.

## Design

The double-sided board uses the front silkscreen layer to make the LEDs appear like a strand of lights on a Christmas tree. When two CR2032 coin cell batteries are inserted on the back and the switch is turned on, the lights flash sequentially.

The design uses a simple LM555 timer circuit to increment an octal counter. Each output of the counter controls a single LED.

## Files

```
.
├── altium       original Altium Designer files
├── kicad        converted KiCad files
├── images       schematic, board view, and PCB images
└── README.md
```

## Project Images

### Schematic

<img src="images/schematic.webp" alt="Schematic" width="500px">

### Board Views

<img src="images/boardview_all.webp" alt="Board view, all" width="500px">
<img src="images/boardview_top.webp" alt="Board view, top" width="500px">
<img src="images/boardview_bottom.webp" alt="Board view, bottom" width="500px">

### Bare Board

Bare board fresh from JLCPCB. They came back looking clean.

<img src="images/bare_front.webp" alt="Bare board, front" width="500px">
<img src="images/bare_back.webp" alt="Bare board, back" width="500px">

### Modded Board

Of course the first run had some bugs. I was able to get it working after a bit of troubleshooting and some board modifications.

<img src="images/modded_front.webp" alt="Modded board, front" width="500px">
<img src="images/modded_back.webp" alt="Modded board, back" width="500px">

## Lessons Learned

- Double check trace widths before ordering. I used the default trace width, which led to the traces being thinner than expected. It didn't cause any electrical issues, but the traces could've been wider for the same cost.

## Next Steps

- Translate indentified design issues back into schematic and layout
- Order another run of boards
