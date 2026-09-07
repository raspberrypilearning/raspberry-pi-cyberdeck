## Knitdeck

Knitdeck is a small cyberdeck built for reading knitting patterns. It shows a pattern on an e-ink screen, and you can turn the pages and hold your place while you knit with mechanical buttons.

![The finished Knitdeck, shown closed and then open with a pattern on its e-ink screen.](images/knitdeck-final4.jpg){:width="550px"}

### Inspiration

Knitdeck grew out of a love of making and crafts. The aim was to make a cyberdeck that felt like it belonged in the craft world rather than the tech one.

Collecting inspiration is a good start. This is a [Figma](https://www.figma.com) mood board, with references for the look and feel of it.

![A Figma mood board of knitting and craft references, used to set the look and feel.](images/knitdeck-inspo.png){:width="550px"}

### Testing the software

The software was added using [SSH](https://projects.raspberrypi.org/en/projects/raspberry-pi-cyberdeck/9).

![Connecting to the Raspberry Pi over SSH to work on it.](images/knitdeck-softwared-ssh.png){:width="550px"}

The software test shows the knitting pattern on the screen and moves through pages of the pattern with the buttons.

![Showing a knitting pattern on the screen during testing.](images/knitdeck-test.jpg){:width="450px"}

Buttons can be tested by connecting a breadboard with buttons to the Raspberry Pi.

![A breadboard of buttons connected to the Raspberry Pi for testing.](images/knitdeck-intial-test.jpg){:width="550px"}

Once the parts are tested, it is helpful to draw the final circuit design out. This can be done on paper or by using a tool like [Fritzing](https://fritzing.org).

![The circuit design drawn out in Fritzing.](images/knitdeck-circuit.png){:width="550px"}

### The enclosure

Knitdeck is mounted inside a second-hand sewing box. This kind of box can be found in charity shops and thrift stores. It gives the project a crafty feel.

![The second-hand sewing box used as the enclosure.](images/knitdeck-case.png){:width="550px"}

### Making the control pad

Buttons are mounted onto cardboard. To do this, start by drawing where the parts go.

![Drawing where the buttons go on the cardboard.](images/knitdeck-draw-buttons.jpg){:width="550px"}

Then cut out the holes.

![Cutting out the holes for the buttons.](images/knitdeck-cutout.png){:width="550px"}

Wadding and fabric are added to the card to give it a soft feel.

![Adding wadding and fabric to soften the control pad.](images/knitdeck-wadding.gif){:width="550px"}

Cardboard is a great material to use because it is easy to get hold of and can be glued with PVA glue or held together with tape.

![Gluing the control pad together with PVA glue.](images/knitdeck-glue.gif){:width="550px"}

Make sure there is enough space to add the Raspberry Pi and wires under the buttons.

![Adding structure with space beneath the buttons for the Raspberry Pi and wires.](images/knitdeck-adding-structure.gif){:width="550px"}

### Wiring buttons

Soldering wires onto buttons can be fiddly, and a cyberdeck with a regular keyboard that does not need to be soldered is far simpler.

The order of soldering parts is important. First wires are soldered to the buttons.

![Soldering wires to a button.](images/knitdeck-solder-button.png){:width="550px"}

Then the wired buttons are threaded through and glued into the cardboard.

![Threading the wired buttons through the cardboard.](images/knitdeck-add-button.gif){:width="550px"}

![Gluing the buttons into the cardboard.](images/knitdeck-gluebuttons.png){:width="550px"}

![The buttons working once wired up.](images/knitdeck-keys.gif){:width="550px"}

### Placing the screen

The screen is positioned in a removable tray that fits inside the box lid.

![The screen in a removable tray that fits inside the box lid.](images/knitdeck-incase.jpg){:width="450px"}

It is attached to cardboard, so there is space for the board and wires behind it.

![Attaching the screen to cardboard with space behind for the board and wires.](images/knitdeck-card1.gif){:width="550px"}

![Cutting the cardboard for the screen tray.](images/knitdeck-cutout-card.gif){:width="550px"}

![Fitting the screen into its cardboard tray.](images/knitdeck-screen.gif){:width="550px"}

### Soldering to a board

The other end of the wires from the buttons and screen are soldered to a perf-board, which is a circuit board with lots of holes in it.

![Soldering the wires to the perf-board.](images/knitdeck-solderingset-up.jpg){:width="550px"}

Headers are soldered to the board and connected to the wires.

![Soldering the and headters.](images/knitdeck-board.png){:width="550px"}

This is then plugged into the Raspberry Pi GPIO pins.

There are 6 buttons, and multiple wires for the e-ink screen, so the wiring can look like a bit of a tangle.

![The tangle of wires from the buttons and screen.](images/knitdeck-tangle.jpg){:width="450px"}

### Making it yours

One of the best parts is decorating and making cyberdecks personal.

![Decorating the finished Knitdeck.](images/knitdeck-deco.gif){:width="550px"}

The Knitdeck is decorated with beads that were sewn into the fabric covering.

![A close-up of the beads sewn into the fabric covering.](images/knitdeck-detail1.jpg){:width="450px"}

Wires are covered using a macramé knotting technique.

![Covering the wires with a macramé knotting technique.](images/knitdeck-macrame.gif){:width="550px"}

Stitching is also used to add colour and texture.

![Stitching added for colour and texture.](images/knitdeck-stitching.jpg){:width="550px"}
