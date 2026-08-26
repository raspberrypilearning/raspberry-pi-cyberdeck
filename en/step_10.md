## Add a button

On a shop-bought computer, every button does what somebody else decided. On yours, you choose.

![A button on a breadboard wired to a Raspberry Pi.](images/button-wired.png){:width="450px"}

> [!INFO]
>
> **GPIO** is short for general purpose input and output. **Input** pins listen. **Output** pins act. A button is an input.
>
> ![A GPIO pin diagram with GPIO 17 and a ground pin marked.](images/gpio-pinout-button.png){:width="450px"}

> [!TASK]
>
> Shut down before wiring anything.
>
> ```bash
> sudo shutdown -h now
> ```
>
> Wait for the light by the card slot to stop flashing, then unplug the power.

> [!TASK]
>
> Wire one leg of the button to **GPIO 17**. Wire the other leg to a **ground** pin.
>
> Either leg, either way round.

> [!TIP]
>
> A four-legged button is two pairs joined across the middle. Not working? Turn it a quarter turn.

> [!TASK]
>
> Plug the power back in.
>
> Open **Thonny**, from the raspberry menu under **Programming**.

> [!TASK]
>
> Type this and save it as `button.py`.
>
> ```python
> from gpiozero import Button
>
> button = Button(17)
> ```

> [!TASK]
>
> Add two lines, then run it and press the button.
>
> ```python
> button.wait_for_press()
> print("You pressed the button")
> ```

**Test:** The message appears in the shell at the bottom of Thonny.

> [!DEBUG]
>
> Nothing happens? Push both wires all the way on. Check one is on a ground pin, not a power pin.
>
> Message appears straight away? The wires are probably touching.

One press and it stops. Make it keep listening.

> [!TASK]
>
> Replace the last two lines with a loop.
>
> ```python
> while True:
>     button.wait_for_press()
>     print("You pressed the button")
>     button.wait_for_release()
> ```

**Test:** One message per press, as many times as you like.

> [!TASK]
>
> Now make it do something you want.
>
> This one prints the temperature of your Raspberry Pi.
>
> ```python
> from gpiozero import Button, CPUTemperature
>
> button = Button(17)
> cpu = CPUTemperature()
>
> while True:
>     button.wait_for_press()
>     print(cpu.temperature)
>     button.wait_for_release()
> ```

> [!TIP]
>
> Decide what your buttons are for before cutting holes for them.
