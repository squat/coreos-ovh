# CoreOS-OVH
CoreOS Linux is awesome and OVH is pretty tight. Unfortunately, OVH does not offer the aforementioned Linux distribution on its VPS. Luckily, it's pretty easy to get CoreOS Linux running on your OVH box. coreos-ovh is a simple shell script that automates this installation process for you.

*Disclaimer*: This software comes with no guarantees and is endorsed by nobody. Use it or don't.

## Installation

1. Launch a new OVH VPS with any Linux distribution; it doesn't matter which one since it will be overwritten shortly;
2. navigate to the OVH web control panel and select your VPS;
3. select the *advanced mode* layout for the control panel;
4. boot your server into *rescue mode*;
5. you will receive an email with temporary credentials to access your VPS in rescue mode. SSH into your box with these credentials now; and
6. run coreos-ovh on your machine:

    ```sh
    $ sh <(curl -s https://raw.githubusercontent.com/squat/coreos-ovh/master/coreos-ohv)
    ```
**Congratulations!** You now have CoreOS Linux on your server!
