## Sideband

Sideband begins with familiar parts — a Raspberry Pi, a screen and a keyboard — and packs
them into a tough, sealable case about the size of a large briefcase.

It is a playful, modern take on the cyberspace decks imagined by science-fiction
writer William Gibson. In his 1984 novel *Neuromancer*, a hacker named Case uses a special
computer called a *cyberspace deck* to enter the matrix. In the story, the matrix is a
shared virtual world made from computer networks and data. The book helped shape
cyberpunk: a kind of science fiction set in high-tech worlds where life is often difficult.

Sideband gives Gibson's idea a chunky, physical twist: a rugged, ready-to-go cyberpunk rig
that is part field computer and part spacecraft console. Instead of hiding the technology,
it celebrates it. Screens, switches and lighting make its network activity visible.

It is not the smallest, lightest or most practical way to package a computer. That is
deliberate. Sideband looks as though it has dropped out of a science-fiction future, but
every part has a real job.

The whole system works less like one giant computer and more like a team. The Raspberry
Pi, tablets and approved test devices are all *nodes* — individual devices on a private
local network. Each node has its own job.

Most of this network stays offline. If an authorised security task needs the internet,
only the main computer is given access. The tablets and test devices remain isolated from
the public internet. Here, hacking means testing only computers that the person using
Sideband owns or has permission to test.

![TODO::Sideband open inside its hard case, with the main display, silver deck, controls and two tablet displays visible.](images/sideband-open.jpg){:width="450px"}

Beneath the deck, a Raspberry Pi 5 with 8GB of memory and a cooling system runs Raspberry
Pi OS. It also runs Sideband's local websites and network tools.

### The case and display

The hard case does more than protect the parts. It also supports them. A moulded ledge
around the inside holds the deck, so no extra frame is needed.

The deck is made from a 5mm sheet of cast acrylic, a rigid, clear plastic. It measures
440mm by 296mm and is painted silver on the back. A laser cutter made the openings for the
controls, sockets and storage slots.

The main display was rescued from a pi-topCEED, an older Raspberry Pi desktop kit found in
a dusty store cupboard. It sits on an acrylic panel in the lid, with the screen's power
board mounted behind it.

The screen keeps its original power supply and button, separate from the Raspberry Pi.
This means the screen can be switched off while the Pi and its background tools continue
to run.

### Making room for input

The keyboard projector was first funded through the crowdfunding website Kickstarter,
then sat unused for years. It now projects a keyboard across the acrylic in red laser
light. An infrared sensor uses light that human eyes cannot see to detect each key press.
The projector then sends the selected key to the Raspberry Pi over Bluetooth. When
Sideband is packed away, the projector fits into its own storage slot.

An ordinary mouse needs a flat surface, room to move and somewhere to be stored. A
trackball stays in one place while its exposed ball is rolled. It also looks at home on a
spaceship or an arcade machine, which suits Sideband nicely.

Two lit-up arcade buttons above the ball act as the left and right mouse buttons. They
connect through the trackball, which also supplies power to their lights. A PS/2-to-USB
adapter then connects the complete set to the Raspberry Pi as one USB device.

![TODO::The red laser keyboard projected onto Sideband's silver deck beside the trackball and two lit-up arcade mouse buttons.](images/sideband-input.jpg){:width="450px"}

### Controls and switches

Sideband has eight physical controls: four for lighting, two mouse buttons, a key-lock
mode switch and a safe shutdown button.

The key-lock switch selects one of two modes. In workstation mode, Sideband works like a
regular Raspberry Pi OS computer. In game mode, it becomes the console for a
beginner-friendly local penetration-testing game, with the game spread across both
tablets.

Penetration testing means looking for security weaknesses in a computer or network. It
must only be carried out on systems you own or have permission to test. Sideband's game
uses its closed practice network and is still in development.

The shutdown button is deliberately difficult to trigger by accident. A quick press does
nothing. A long press asks Raspberry Pi OS to finish its work and shut down safely; the
button never cuts the power directly. This makes files on the microSD memory card less
likely to be damaged.

+ **Key-lock switch** — changes between the Raspberry Pi OS desktop and game mode
+ **Shutdown button** — asks Raspberry Pi OS to shut down after a long press
+ **Mode button** — moves the lighting to its next pattern
+ **Brightness dial** — changes the brightness of the lighting
+ **Blackout switch** — turns off the main decorative lighting without turning off the
  Raspberry Pi
+ **Lamp switch** — turns on the lights beneath the arcade buttons
+ **Arcade buttons (two)** — work as the trackball's left and right mouse buttons

![TODO::Sideband's labelled key-lock, shutdown button, lighting controls and two arcade mouse buttons.](images/sideband-controls.jpg){:width="450px"}

### Side displays

The two 7-inch Android tablets were once used at Raspberry Pi Foundation events for
audience quizzes and forms. They are now too old for many current apps, but their screens
still make useful information displays.

The Raspberry Pi creates private Wi-Fi and sends a different webpage stored on the Pi to
each tablet. The displays therefore work at home, at school or at an event without using
the venue's Wi-Fi or internet connection. Only approved devices can join.

In workstation mode, one tablet shows the Pi's temperature, memory use and storage use.
The other shows which devices are connected, the strength of the Wi-Fi signal and other
network details.

Game mode gives the tablets a different job. Both become part of the game display, showing
tasks, notes and information about devices on the local network.

![TODO::Sideband's two tablets, showing temperature, memory and storage information on one screen and local network information on the other.](images/sideband-tablets.jpg){:width="450px"}

The tablets show information and provide lighting controls, but neither can type into or
control the Raspberry Pi desktop.

When Sideband is packed away, both tablets are stored upright on their narrow edges in a
slot in the deck, where they also charge.

### Lighting and power

The lights are useful as well as dramatic. Two LED grids — rows of small, coloured lights
— sit below the acrylic deck. The control labels are engraved through the silver paint,
allowing the LEDs to shine through. A small Raspberry Pi Pico W controls both grids. Some
light patterns warn that something has gone wrong; others simply make startup look
properly futuristic.

Either tablet can control the grids through its local webpage. The physical mode button
and brightness dial provide another way to adjust them. A hardware blackout switch cuts
the main decorative lighting directly, without using either tablet. A separate lamp
switch controls the arcade-button lights.

A circular LED board in the lid provides a separate glow. It shines towards the mirrored
surface behind the display, where the light bounces back softly instead of pointing
straight out of the case.

Everything packs into one case, but Sideband still needs to be plugged into a wall socket.
A single power cable enters the case. From there, a switched extension lead shares power
between four adapters: one for the Raspberry Pi, one for the main display, one for the LED
lighting, and one USB charger for the tablets and smaller boards.

![TODO::Internal view of Sideband, showing the Raspberry Pi and cooling system, two LED grids, power adapters and the cables inside.](images/sideband-internals.jpg){:width="450px"}
