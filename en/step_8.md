## Use Raspberry Pi Connect

to do - test this.

**Raspberry Pi Connect** makes a version of your Raspberry Pi's desktop in a browser on another computer. This is handy for a cyberdeck, so that you can access the whole desktop without a monitor.

> [!TASK]
>
> On your Raspberry Pi, open a **terminal** with the black icon in the top bar.
>
> ![to do add image of terminal icon](images/aa.png){:width="450px"}


> [!TASK]
> 
> Copy this line of code, which update then XXX [waht does it do]
>
> ```bash
> sudo apt update && sudo apt install rpi-connect
> ```

> [!TASK]
>
> Copy this to turn Raspberry Pi Connect on. 
>
> ```bash
> rpi-connect on
> ```

> [!TASK]
>
> Then copy a line to sign in.
>
> ```bash
> rpi-connect signin
> ```

check - do we need to explaign the sign in process (i.e. propmtbed but cant see them - check this)

> [!TASK]
>
> Type the web address that is [check what this is]. You can use the browser on the Raspberry Pi or type the address into another computer.

> [!TASK]
> 
> You should see a XXX [check what happens]
>
> Sign in with your **Raspberry Pi ID**, or create one for free if you do not have an account yet.

![Raspberry Pi Connect asking you to sign in with your Raspberry Pi ID.](images/connect-id-sign-in.png){:width="450px"}

> [!TASK]
>
> Name your Raspberry Pi, then click **Create device and sign in**.

![Raspberry Pi Connect asking you to name your new device.](images/connect-name-device.png){:width="450px"}

**Test:** Check that the Connect icon in the top bar turns blue.

> [!TASK]
>
> Go to another computer. Open [connect.raspberrypi.com](https://connect.raspberrypi.com) and sign in with the same Raspberry Pi ID.

![Raspberry Pi Connect showing an online Raspberry Pi and its Connect via button.](images/connect-device-dashboard.png){:width="450px"}

> [!TASK]
>
> Find your Raspberry Pi. The example calls its device **pitowers**, but yours will show the name you chose. Select **Connect via**, then **Screen sharing**.

![to do - add image of this Raspberry Pi Connect showing an online Raspberry Pi and its Connect via button.](images/to.png){:width="450px"}

**Test:** The Raspberry Pi desktop appears in the browser. Moving the mouse there moves the pointer on the Raspberry Pi itself.

![The Raspberry Pi desktop shown inside a browser window on a laptop.](images/connect-in-browser.png){:width="450px"}

> [!DEBUG]
>
> Shows as offline? Check the Raspberry Pi is on and still on wi-fi. Both computers need to be online.
>
> Screen sharing unavailable? Run `rpi-connect doctor` in a terminal on the Raspberry Pi. It checks the service, desktop and network, and puts a cross beside anything that needs attention.

> [!TIP]
>
> Connect works from anywhere, not only at home.

to do - check what this is below
*Official sign-in, device-name and dashboard screenshots: © Raspberry Pi Ltd, from the [Raspberry Pi Connect documentation](https://www.raspberrypi.com/documentation/services/connect.html), licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Displayed at a smaller size.*
