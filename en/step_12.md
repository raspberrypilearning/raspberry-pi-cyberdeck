## Connect with SSH

**SSH** is short for **S**ecure **Sh**ell. You can use it to work on your Raspberry Pi from a different computer.

to do - check this, is this a safety warnign? if so make it say that
> [!INFO]
>
> For this project, keep SSH inside your private network. Both computers should be
> connected to the same router or local network.

> [!TASK]
>
> On the desktop of your Raspberry Pi computer, hover over the network icon in the top-right corner to see the local IP address. 
>
> Write both down. 

- is this needed?

![The Raspberry Pi OS network tooltip showing a Wi-Fi connection and its local IP address.](images/ssh-find-ip-address.png){:width="450px"}

> [!TIP]
>
> Your network name and numbers will differ from this example.

- as before is theis needde?

> [!TASK]
>
> Open a terminal on another computer.
>
> - **Windows** — open Terminal or PowerShell from the Start menu. 
> - **Mac** — open Terminal from Applications, then Utilities. 
> - **Linux** — open your usual terminal program.

> [!TASK]
>
> In the terminal type `ssh` and your username and hostname. For example, below the username is `alex` and the hostname is `cyberdeck`. You chose the password, username and hostname in the Imager. 
>
>
> ```bash
> ssh alex@cyberdeck.local
> ```

to do - write the following wardnifns into steps - reduce them so they are simple. 

> The first time you connect, SSH asks if you trust this computer. Check that you
> are connecting to your own Raspberry Pi, then type `yes` and press **Enter**. 

A warning will The authenticity of host 'code-club.local (2a00:23c7:510e:cc01:2ecf:67ff:fec3:140d)' can't be established.
ED25519 key fingerprint is: SHA256:LVUDIaqPYRyJiGzLD4CQKYCyDeg/A2RbuUSSTR7jLQs
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])?If prompted Are you sure you want to continue connecting (yes/no/[fingerprint])? yes


Warning: Permanently added 'code-club.local' (ED25519) to the list of known hosts.
code-club@code-club.local's password: 
> [!TASK]
>
> When prompted enter your password. 
> Type the full password, then press **Enter**. For security, nothing will appear when you type. 

> [!TIP]
>


to do - check if the next steps are needed. could let them know what to do - such as some simple tasks.

**Test:** Check that the terminal prompt [to do - check this word] changes to show the Raspberry Pi's username and hostname, such as `alex@cyberdeck:~ $`.

![to do - add image of this.](images/to.png){:width="450px"}


> [!TASK]
>
> Ask the remote computer for its hostname.
>
> ```bash
> hostname
> ```

to do - check why this is done?

**Test:** The reply matches the Raspberry Pi hostname you wrote down earlier.

> [!DEBUG]
>
> **Could not resolve hostname?** Connect with the IP address instead. Replace the
> example username and numbers with your own:
>
> ```bash
> ssh alex@192.168.1.42
> ```
>
> **Connection timed out?** Check that the Raspberry Pi is on and both computers are on
> the same local network. Check the IP address again too.
>
> **Connection refused?** SSH may be off, or the address may lead to a different device.
> Return to the first task and check both.
>
> **Permission denied?** Check the username and password you entered in Imager, and make
> sure **Caps Lock** is off.

> [!TASK]
>
> When you have finished, close the SSH connection:
>
> ```bash
> exit
> ```

> [!TIP]
>
> SSH suits commands and files. Connect suits anything with windows and buttons.

to do check this - can we jsut use the screen shots that we make ourselves? --->
*Official Control Centre and network screenshots: © Raspberry Pi Ltd, from the [Raspberry Pi remote-access documentation](https://www.raspberrypi.com/documentation/computers/remote-access.html), licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Displayed at a smaller size.*




- add this somewher
> [!TIP]
>
> If did not enable SSH in the Raspberry Pi Imager, you will need to switch it on.
>
> To check open the Raspberry Pi menu, then **Preferences** and **Control Centre**. Select **Interfaces**, switch **SSH** on and select **Close**. If you changed the switch, restart the Raspberry Pi before you continue.

to do - add iamge of the raspbey pi menu - one step before this. 

![Raspberry Pi OS Control Centre open on the Interfaces page, with SSH switched on.](images/ssh-control-centre.png){:width="450px"}