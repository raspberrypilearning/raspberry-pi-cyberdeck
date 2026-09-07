## Knitdeck

Knitdeck is a small cyberdeck built for reading knitting patterns. It shows a pattern on an e-ink screen, and you can turn the pages and hold your place while you knit with mechanical buttons.

![The finished Knitdeck, shown closed and then open with a pattern on its e-ink screen.](images/knitdeck-final1.jpg){:width="450px"}

![The finished Knitdeck from another angle.](images/knitdeck-final2.jpg){:width="450px"}

### Inspiration

Knitdeck grew out of a love of making and crafts. The aim was to make a cyberdeck that felt like it belonged in the craft world rather than the tech one.

Collecting inspiration is a good start. This is a figma mood board, of references for the look and feel of it.

![A Figma mood board of knitting and craft references, used to set the look and feel.](images/knitdeck-inspo.png){:width="450px"}

### The software

The software was added using SSH. It shows the knitting pattern on the screen and moves through pages of the pattern with the buttons.

![Connecting to the Raspberry Pi over SSH to work on it.](images/knitdeck-softwared-ssh.png){:width="450px"}

The buttons needed to be mapped in the config file.

![The config that maps each button.](images/knitdeck-software-config.png){:width="450px"}

### Testing

The software, screen and buttons were tested before the cyberdeck was assembled. 

![Testing everything before the deck was assembled.](images/knitdeck-test.jpg){:width="450px"}

Buttons can be tested by connecting a breadboard with buttons to the Raspberry Pi.

![Add.](images/knitdeck-inital-test.jpg){:width="450px"}

Once the parts are tested, it is helpful to draw the circuit out. This can be done on paper or by using a tool like Frizing (add link).

![add - image of circuit diagram](images/add.jpg){:width="450px"}

### The enclosure

Knitdeck is mounted inside a second hand sewing box. This kind of box can be found in charity shops and thrift stores. It gave the project a crafty feel.

![The second-hand 1990s sewing box used as the enclosure.](images/knitdeck-case.png){:width="450px"}

### Adding buttons

A lot of the structure is made from adding the components to cardboard. The best way to do this is to draw where the parts go first, then cut.

![Arranging the buttons for the bottom part.](images/knitdeck-arrangebuttons.gif){:width="450px"}

The wadding was added to the card to give it a soft feel.

![Adding wadding to the bottom button part.](images/knitdeck-wadding.gif){:width="450px"}

Cardboard can be glued with PVA glue or held together with tape.

![Gluing the bottom button part together.](images/knitdeck-glue.gif){:width="450px"}

### Soldering

Soldering is fiddly, and a cyberdeck with a regular keyboard is far simpler.

The order of assmebling parts is important, becasue the are soldered into to place. 

First wires are soldered to the buttons.
![ADD .](images/knitd.gif){:width="450px"}

Then buttons are a glued into the cardboard.

![The buttons working after soldering.](images/knitdeck-keys.gif){:width="450px"}

![The soldering set-up for the button wires.](images/knitdeck-solderingset-up.jpg){:width="450px"}

Finally wires from the buttons are soldered.

Wires are soldered to a circuit board, then headers used to connect to the Raspberry Pi GPIO pins.

![ADD - solder wires.](images/knit0deck-parts.jpg){:width="450px"}

![Soldering the button wires.](images/knitdeck-soldering-parts.jpg){:width="450px"}

![Soldering the button wires.](images/knitdeck-soldering.gif){:width="450px"}

There a 6 buttons, and multiple wires for the e-ink screen, so once soldered into place, the wiring can look like a tangle. 

![Soldering the button wires.](images/knitdeck-tangle.jpg){:width="450px"}


### Placing the screen

The screen is attached to a cardboard surface, so there is space for the boards and wires behind it.

![Cutting the card for the top part that holds the screen.](images/knitdeck-cutout-card.gif){:width="450px"}

### Making it yours

One of the best parts is decorating and making cyberdecks personal. The knitdeck was decorated with beads, that were sewn into the fabric covering.

![The decorated Knitdeck, with a close-up of the details.](images/knitdeck-deco.gif){:width="450px"}

![A close-up detail of the finished Knitdeck.](images/knitdeck-detail1.jpg){:width="450px"}

Wires were covered using a macrame knotting technique.

![ADD - close-up detail of the wires.](images/knitdeck-macrame.gif){:width="450px"}