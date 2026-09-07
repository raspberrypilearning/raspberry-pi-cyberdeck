## Knitdeck

Knitdeck is a small cyberdeck built for reading knitting patterns. It shows a pattern on an e-ink screen, and you can turn the pages and hold your place while you knit with mechanical buttons.

![The finished Knitdeck, shown closed and then open with a pattern on its e-ink screen.](images/knitdeck-final1.jpg){:width="450px"}

![The finished Knitdeck from another angle.](images/knitdeck-final2.jpg){:width="450px"}

### Inspiration

Knitdeck grew out of a love of making and crafts. The aim was to make a cyberdeck that felt like it belonged in the craft world rather than the tech one.

Collecting inspiration is a good start. This is a figma mood board, of references for the look and feel of it.

![A Figma mood board of knitting and craft references, used to set the look and feel.](images/knitdeck-inspo.png){:width="450px"}

### The enclosure

Knitdeck started with an early 2000s sewing box, that was bought second-hand. This kind of box often turns up in charity shops and thrift stores. It already carried the craft feel the project was reaching for.

![The second-hand 1990s sewing box used as the enclosure.](images/knitdeck-case.png){:width="450px"}

### Making everything fit

Before starting, it is helpful to map out how the screen, keys and Raspberry Pi would sit inside. In the end the parts needed more room than expected, so the design changed through the making process.

![The first plan for where the battery and Raspberry Pi would go.](images/knitdeck-design.png){:width="450px"}


### Adding buttons

Before adding the mechanical buttons it is helpful to test how they will work. This can be done by connecting a breadboard with buttons to the Raspberry Pi.

![Add.](images/knitdeck-inital-test.jpg){:width="450px"}

A lot of the structure is made from adding the components to cardboard. The best way to do this is to draw where the parts go first, then cut.

![Arranging the buttons for the bottom part.](images/knitdeck-arrangebuttons.gif){:width="450px"}

The buttons sit on a soft board, stuffed with wadding.

![Adding wadding to the bottom button part.](images/knitdeck-wadding.gif){:width="450px"}

Cardboard can be glued with PVA glue or held together with tape.

![Gluing the bottom button part together.](images/knitdeck-glue.gif){:width="450px"}

### Soldering

Soldering is fiddly, and a cyberdeck with a regular keyboard is far simpler — even a few buttons adds a tangle of wires to manage.



The buttons are soldered then glued into the cardboard.

![The buttons working after soldering.](images/knitdeck-keys.gif){:width="450px"}

![The soldering set-up for the button wires.](images/knitdeck-solderingset-up.jpg){:width="450px"}

Finally buttons and all GPIO parts are soldered to the board. 

To keep track, use diagrams and draw out the circuit first.

![add - image of circuit diagram](images/add.jpg){:width="450px"}

This cycberdeck uses a circuit board to solder all the wires to, then headers to connect to the Raspberry Pi GPIO pins.

![Soldering the button wires.](images/knitdeck-soldering-parts.jpg){:width="450px"}

Only solder after testing, and being certain where all the wires go.

![Soldering the button wires.](images/knitdeck-soldering.gif){:width="450px"}

There a 6 buttons, and multiple wires for the e-ink screen, so once soldered into place, the wiring can look like a tangle. 

![Soldering the button wires.](images/knitdeck-tangle.jpg){:width="450px"}


### Placing the screen

![Cutting the card for the top part that holds the screen.](images/knitdeck-cutout-card.gif){:width="450px"}

### The software

The software came together bit by bit over SSH, going back and forth with the code. It shows the pattern pages on the screen and moves through them with the buttons, each one mapped to a page turn or the stitch count. Everything was tested before the deck was assembled.

![Connecting to the Raspberry Pi over SSH to work on it.](images/knitdeck-softwared-ssh.png){:width="450px"}

![The config that maps each button.](images/knitdeck-software-config.png){:width="450px"}

![Testing everything before the deck was assembled.](images/knitdeck-test.jpg){:width="450px"}

### Powering

![Drilling a hole for the power cable.](images/knitdeck-drill.gif){:width="450px"}

### Making it yours

One of the best parts was decorating it and making it personal.

![The decorated Knitdeck, with a close-up of the details.](images/knitdeck-deco.gif){:width="450px"}

![A close-up detail of the finished Knitdeck.](images/knitdeck-detail1.jpg){:width="450px"}
