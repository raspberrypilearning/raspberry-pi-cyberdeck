## Knitdeck

Knitdeck is a small cyberdeck built for reading knitting patterns. It shows a pattern on an e-ink screen, and a few buttons turn the pages and hold your place while you knit.

![The finished Knitdeck, shown closed and then open with a pattern on its e-ink screen.](images/knitdeck-final1.jpg){:width="450px"}

![The finished Knitdeck from another angle.](images/knitdeck-final2.jpg){:width="450px"}

### Inspiration

Knitdeck grew out of a love of making and crafts, and a big pile of knitting patterns. The aim was something simple that felt like it belonged in the craft world rather than the tech one.

This is a figma mood board, of inspiration for the look and feel of it.

![A Figma mood board of knitting and craft references, used to set the look and feel.](images/knitdeck-inspo.png){:width="450px"}

### The enclosure

Knitdeck started from an old 1990s sewing box, bought second-hand — the kind that often turns up in charity shops and thrift stores. It already carried the craft feel the project was reaching for.

![The second-hand 1990s sewing box used as the enclosure.](images/knitdeck-case.png){:width="450px"}

### Making everything fit

The first plan for how everything would sit inside was optimistic.

![The first plan for where the battery and Raspberry Pi would go.](images/knitdeck-design.png){:width="450px"}

The real parts needed more room than expected, so the design kept changing through the making.

### Building it

The inside structure is cardboard. It took a lot of making and adjusting — cutting, gluing and trimming pieces until everything sat right.

![Cutting the card for the top part that holds the screen.](images/knitdeck-cutout-card.gif){:width="450px"}

![Arranging the buttons for the bottom part.](images/knitdeck-arrangebuttons.gif){:width="450px"}

![Adding wadding to the bottom button part.](images/knitdeck-wadding.gif){:width="450px"}

![Gluing the bottom button part together.](images/knitdeck-glue.gif){:width="450px"}

![Drilling a hole for the power cable.](images/knitdeck-drill.gif){:width="450px"}

### Soldering

Soldering was the fiddliest part, and the one that felt most permanent. A build with no buttons is far simpler — even a few buttons adds a tangle of wires to manage.

![The soldering set-up for the button wires.](images/knitdeck-solderingset-up.jpg){:width="450px"}

![Soldering the button wires.](images/knitdeck-soldering.gif){:width="450px"}

![The buttons working after soldering.](images/knitdeck-keys.gif){:width="450px"}

### The software

The software came together bit by bit over SSH, going back and forth with the code. It shows the pattern pages on the screen and moves through them with the buttons, each one mapped to a page turn or the stitch count. Everything was tested before the deck was assembled.

![Connecting to the Raspberry Pi over SSH to work on it.](images/knitdeck-softwared-ssh.png){:width="450px"}

![The config that maps each button.](images/knitdeck-software-config.png){:width="450px"}

![Testing everything before the deck was assembled.](images/knitdeck-test.jpg){:width="450px"}

### Making it yours

One of the best parts was decorating it and making it personal.

![The decorated Knitdeck, with a close-up of the details.](images/knitdeck-deco.gif){:width="450px"}

![A close-up detail of the finished Knitdeck.](images/knitdeck-detail1.jpg){:width="450px"}
