## Sideband

Sideband starts with familiar parts — a Raspberry Pi, a screen and a keyboard — and folds
them into a sealed hard case about the size of a large briefcase. It is portable, although
not quite in the laptop sense: everything travels as one piece, then runs from mains power
when it arrives.

Sideband is also a modern, deliberately jokey take on the cyberspace decks imagined by
William Gibson. His 1984 novel *Neuromancer* follows Case, a hacker who uses a specialised
cyberspace deck to enter the matrix: a shared, computer-generated world built from
networks and data. The book helped define the cyberpunk genre.

Sideband turns that Gibsonesque idea into something much more physical — a rugged, ready-to-go cyberpunk rig, part field terminal and part spacecraft
console. Its screens, switches and network activity are deliberately on show, because it's built for learning cybersecurity techniques.

It is not the smallest, lightest or most practical way to package a Raspberry Pi. That is
the point. It is not a prop, either. Everything works and has a specific function: the Raspberry Pi, tablets and connected test devices
form a working private LAN, tied together by services running on Sideband.

Most of that network works offline. When an authorised hacking task needs access to the
wider internet, Sideband can use a controlled route designed to keep its private nodes off
the public network, and away from attackers who might use it to gain access to its systems.

![TODO::Sideband set up in its open hard case, with the main display, silver acrylic deck, controls and two tablet displays visible.](images/sideband-open.jpg){:width="450px"}

At the centre is a Raspberry Pi 5 with 8GB of memory and a cooling system, running Raspberry Pi OS. It sits
below the deck surface; the screen, controls and network services are built around that
reliable core.

### The case and display

The case is more than packaging; it is the frame. A moulded lip around the inside supports
a 5mm cast acrylic panel, painted silver on the back and cut to 440mm by 296mm, without needing
a separate frame. Openings for the controls, sockets and storage slots were all laser-cut
into that one panel.

The display follows the same reuse-first approach. It came from a pi-topCEED, an older
Raspberry Pi desktop kit scavenged from a dusty store cupboard, and is mounted on an
acrylic panel in the lid. Its power-management board sits behind it.

The display has its own power supply and button, separate from the Raspberry Pi power
system. That separation is a happy by-product of the recycled monitor: the screen can be switched off without stopping the computer or its background services.

### Making room for input

The keyboard projector is another cupboard rescue. It came from a Kickstarter project
years ago, then sat unused until Sideband gave it a job: projecting a keyboard onto the
acrylic in red laser light. An infrared sensor detects each key press; the projector then
sends the keystroke to the Raspberry Pi over Bluetooth. When the case is packed, the
projector slips into its own storage slot.

Think about what a conventional mouse needs: a clear surface, room to move and somewhere
to be stowed. A trackball needs none of that. It also looks at home on a spaceship or an
arcade machine, which feels about right for this machine.

The two illuminated arcade buttons above the ball provide its left and right mouse clicks.
The trackball supplies power to their lights, controlled by the lamp switch, and the whole
assembly reaches the Raspberry Pi as one USB device through a PS/2-to-USB adapter.

![TODO::The red laser keyboard projected onto Sideband's silver acrylic deck beside the trackball and two illuminated arcade mouse buttons.](images/sideband-input.jpg){:width="450px"}

### Controls and switches

Eight physical controls divide the work between lighting, pointer input, mode selection
and safe shutdown. Four handle the lights, two are mouse buttons, the key-lock switch
chooses Sideband's role, and the shutdown button requests a safe shutdown. Nothing is
there simply to look busy.

The key-lock switch gives Sideband two distinct roles. In one position, it is a normal
Raspberry Pi OS workstation. Turned to game mode, it becomes the console for a
beginner-friendly penetration-testing game on a private LAN, with both tablets joining the
game display. The game itself is still in development.

Shutdown is deliberately harder to trigger. A tap does nothing; only a sustained press
asks Raspberry Pi OS to shut down cleanly. The button never cuts power directly, reducing
the risk of corrupting data on the microSD card.

+ **Key-lock switch** — changes between the Raspberry Pi OS desktop and game mode
+ **Shutdown button** — asks Raspberry Pi OS to shut down after a long press
+ **Mode button** — moves the lighting to its next pattern
+ **Brightness dial** — changes the brightness of the lighting
+ **Blackout switch** — turns off the main decorative lighting without cutting power to the
  Raspberry Pi
+ **Lamp switch** — turns on the lights beneath the arcade buttons
+ **Two arcade buttons** — work as the trackball's left and right mouse buttons

![TODO::Close view of Sideband's labelled key-lock, shutdown button, lighting mode button, brightness dial, blackout switch and lamp switch.](images/sideband-controls.jpg){:width="450px"}

### Side displays

The two 7-inch Android tablets have already had one working life. They started out at
Raspberry Pi Foundation events, handling audience quizzes and forms; although they are now
too old for modern apps, their screens remain perfectly useful. Sideband gives them a
narrower second job as instrument panels.

The Raspberry Pi creates the small Wi-Fi network they join. Because that tablet network is
kept separate from the internet, the panels do not depend on whatever Wi-Fi may—or may
not—be available at home, at school or at an event.

In workstation mode, one tablet shows system information such as temperature, memory use
and storage use, while the other reports current network connections, Wi-Fi signal
strength and connection details. In game mode, that division disappears: both become part
of the game display, showing tasks, notes and local network information such as connected
devices.

![TODO::Sideband's two tablet displays, one showing Raspberry Pi system statistics and the other showing local network information.](images/sideband-tablets.jpg){:width="450px"}

Think of the tablets as instruments, not remote controls. Their authority is deliberately
narrow: neither can type into or control the Raspberry Pi desktop, although either can
operate the two LED grids through dedicated on-screen controls.

When Sideband is packed, both tablets slide edge-on into a slot in the deck surface, where
they also charge.

### Lighting and power

The lighting is part interface, part theatre. Two grids of colour LEDs sit below the
acrylic, shining through control labels engraved through the silver paint on the back.
Some lighting modes signal error states. Others simply look good during startup, which is
reason enough.

Either tablet provides on-screen controls for the two LED grids, but the system does not
depend on them. For quick changes, the physical mode button and brightness dial remain
close at hand; the blackout switch cuts the main decorative lighting, while the lamp
switch handles the arcade-button lights separately.

Rather than shining directly out of the lid, a small circular LED board faces the mirrored
surface behind the display, spreading reflected light across the panel without direct
glare.

Despite its internal complexity, Sideband has a single mains lead. Inside the case, a
switched extension fans the power out to four adapters: one for the Raspberry Pi, one for
the main display, one for the LED panels, and one USB charger for the tablets and smaller
boards.

![TODO::Sideband's silver acrylic deck lifted to reveal the Raspberry Pi and cooling system, two LED grids, power adapters and internal cabling.](images/sideband-internals.jpg){:width="450px"}

Portable here means self-contained, not cordless. Sideband travels as one case and, once
set up, asks only for a single mains socket.
