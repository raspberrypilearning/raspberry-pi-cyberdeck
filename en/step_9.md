## Connect with SSH

**SSH** gives you a terminal on your Raspberry Pi from another computer. Text only, no desktop, and much faster than screen sharing.

![A terminal window on a laptop showing a connection to a Raspberry Pi.](images/ssh-terminal.png){:width="450px"}

> [!TASK]
>
> Check SSH is on. Switching it on in Imager already did this.
>
> Not sure? In a terminal on the Raspberry Pi:
>
> ```bash
> sudo raspi-config
> ```
>
> Choose **Interface Options**, then **SSH**, then **Yes**. Arrow keys to move, **Enter** to choose.

> [!TASK]
>
> Find the name of your Raspberry Pi.
>
> ```bash
> hostname
> ```

> [!TASK]
>
> Open a terminal on the other computer.
>
> **Windows** — Terminal or PowerShell, from the Start menu. **Mac** — Terminal, in Applications then Utilities. **Linux** — your usual terminal.

> [!TASK]
>
> Connect, swapping in your own username and hostname.
>
> ```bash
> ssh pi@cyberdeck.local
> ```
>
> Type `yes` the first time. Then your password.

> [!INFO]
>
> Nothing appears while you type a password, not even dots. Keep typing and press **Enter**.

**Test:** The start of the line changes to your username and hostname, like `pi@cyberdeck`.

> [!TASK]
>
> Try a command.
>
> ```bash
> uname -a
> ```

**Test:** The reply names your Raspberry Pi, not the computer in front of you.

> [!DEBUG]
>
> "Could not resolve hostname"? Use the IP address instead, like `ssh pi@192.168.1.42`.
>
> "Connection refused"? SSH is off. Go back to the first task.
>
> Password refused? Use the username from Imager, not your name on the other computer.

> [!TASK]
>
> To leave:
>
> ```bash
> exit
> ```

> [!TIP]
>
> SSH suits commands and files. Connect suits anything with windows and buttons.
