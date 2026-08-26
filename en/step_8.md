## Use Raspberry Pi Connect

**Raspberry Pi Connect** puts your Raspberry Pi's desktop in a browser on another computer. Handy, because a cyberdeck with no screen of its own is much easier to build.

![The Raspberry Pi desktop shown inside a browser window on a laptop.](images/connect-in-browser.png){:width="450px"}

> [!TASK]
>
> On your Raspberry Pi, open a **terminal** with the black icon in the top bar.
>
> ```bash
> sudo apt update && sudo apt install rpi-connect
> ```

> [!INFO]
>
> Recent versions of Raspberry Pi OS already have it. "Newest version" means it is there already.

> [!TASK]
>
> Turn it on, then start signing in.
>
> ```bash
> rpi-connect on
> rpi-connect signin
> ```

> [!TASK]
>
> Open the web address it gives you, in the browser on the Raspberry Pi.
>
> Sign in with your **Raspberry Pi ID**, or make one. Name your device.

![The Connect sign-in page asking you to name your device.](images/connect-signin.png){:width="450px"}

**Test:** A Connect icon appears in the top bar.

> [!TASK]
>
> Go to another computer. Open [connect.raspberrypi.com](https://connect.raspberrypi.com) and sign in with the same Raspberry Pi ID.
>
> Click **Connect**, then screen sharing.

**Test:** The Raspberry Pi desktop appears in the browser. Moving the mouse there moves the pointer on the Raspberry Pi itself.

> [!DEBUG]
>
> Shows as offline? Check the Raspberry Pi is on and still on wi-fi. Both computers need to be online.
>
> Screen sharing greyed out? The Raspberry Pi may have started with no display attached. Plug it back in and restart.

> [!TIP]
>
> Connect works from anywhere, not only at home.
