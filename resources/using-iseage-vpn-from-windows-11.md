
# Using OpenVPN From Windows 11

I have a workaround for connecting to the VPN in Windows 11. Here's the HOWTO, followed by a code gist.

## Instructions

1. If needed, install Ubuntu in WSL v2 in Windows 11. From now on, I'll refer to this as "Ubuntu."
2. Inside Ubuntu, Run `sudo apt install openvpn` to install OpenVpn v2. These instructions work only with OpenVPN v2, not v3.
  - After installing OpenVPN, you can verify the version by running `openvpn --version.` As of this writing, the answer you want is some flavor of 2.4.x (mine is 2.4.12).
3. Run  `sudo openvpn blue-vpn.ovpn` in Ubuntu to open a connection to ISEAGE, providing your ISEAGE credentials when prompted. Make sure to use `sudo` or you OpenVPN will not be able to access the network resources it needs to function.

## Using SSH

At this point, you will be able to SSH from inside Ubuntu to the competition network. You can use any SSH client as long as it is launched from Ubuntu.

## Using RDP, FTPS, and Web Clients

If you want to connect using other protocols to connect to the competition network, such as RDP, FTPS, or a Web Browser, you will need to use applications installed inside Ubuntu, because the VPN will only be visible inside Ubuntu. 

For SSH, RDP, and FTPS connections, I use Remmina. For Web connections, I use Firefox.

```bash
apt install remmina firefox
```
Once installed, you must launch them from inside an Ubuntu (WSL) prompt. You can launch them by running `remmina` or `firefox`, respectively. 

You may want to include a trailing ampersand at the end of the command so that they run in the background and you can continue using the terminal.

```bash
# code gist
# all code runs inside Ubuntu/WSL2

# to install necessary software:
apt install openvpn remmina firefox

# to connect to VPN
openvpn ./path/to/blue-vpn.ovpn

# to launch firefox and remmina (from another Ubuntu terminal
firefox &
remmina &
```
