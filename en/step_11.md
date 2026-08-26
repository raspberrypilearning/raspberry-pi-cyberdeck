## Add lights

Lights are how a cyberdeck tells you what it is doing.

![An LED lit on a breadboard next to a Raspberry Pi.](images/led-wired.png){:width="450px"}

> [!INFO]
>
> An **LED** is an output, so this time the Raspberry Pi decides.
>
> An LED needs a **resistor** with it. Without one it takes more current than it can survive. 330 ohm is the usual choice.

> [!TASK]
>
> Shut down and unplug the power.
>
> ```bash
> sudo shutdown -h now
> ```

> [!TASK]
>
> Wire the **long leg** to **GPIO 18**, through the resistor. Wire the **short leg** to a **ground** pin.

![A wiring diagram showing the LED, the resistor, GPIO 18 and ground.](images/led-wiring-diagram.png){:width="450px"}

> [!TIP]
>
> An LED only works one way round. The long leg is positive. On a trimmed LED, the flat notch marks the short leg.

> [!TASK]
>
> Power back on. Open Thonny, start a new file, and save it as `lights.py`.
>
> ```python
> from gpiozero import LED
>
> light = LED(18)
> light.on()
> ```

**Test:** The LED lights up and stays on.

> [!DEBUG]
>
> Nothing? Turn the LED round. Backwards is the usual mistake, and does no harm.
>
> Still nothing? Check the resistor is in the loop, not bridging two empty rows.

> [!TASK]
>
> Make it blink.
>
> ```python
> from gpiozero import LED
> from signal import pause
>
> light = LED(18)
> light.blink(on_time=1, off_time=1)
>
> pause()
> ```

**Test:** On and off, once a second.

> [!INFO]
>
> `pause()` keeps the program running. Without it, the program ends and the blinking ends too.

> [!TASK]
>
> Put the button and the light together.
>
> ```python
> from gpiozero import LED, Button
> from signal import pause
>
> light = LED(18)
> button = Button(17)
>
> button.when_pressed = light.on
> button.when_released = light.off
>
> pause()
> ```

**Test:** The LED lights while the button is held down.

> [!TASK]
>
> Change the timings. Or add a second LED on another pin.
>
> A light for each thing your deck can be doing is more use than one that blinks.

> [!TIP]
>
> Lights look better shining through something. Frosted acrylic, thin white plastic, even tape over the hole spreads the light and hides the LED.
