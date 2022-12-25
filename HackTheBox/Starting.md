
A good place to start in [HackTheBox](https://www.hackthebox.com/) is in the Labs > Starting Point folder.  This will walk you through with questions on how to solve problems and build up your knowledge of different tools.

1. To run any of the Starting Point exercises on HTB, navigate to the Starting Point tab and select the `Connect to HTB` button in the top right of your screen.

![](../Images/HTB_navbar.png)

2. Select Starting Point

![[../Images/StartingPoint.png|500]]

3. Select OpenVPN

![[../Images/OpenVPN.png|500]]

4. Leave the default values, and select Download [VPN](../Jargon.md).  (If you find that when working on these examples, your connection is slow, you can select a different VPN server )

![[../Images/DownloadVPN.png|500]]

5. Open your terminal and go to Downloads.  You should find a file called `starting\_point\_\<username\>.ovpn`  Run the command `sudo openvpn starting\_point\_\<username\>.ovpn`  You'll be prompted for a password (since you are running sudo) - type in the administrative password.  Then a bunch of stuff will be spit out to the terminal.  You can ignore that.  You will need to keep this terminal running the entire tme you are working.  Simply open another terminal for any other work you'd like to do.

![[../Images/RunVPN.png|700]]

6. Navigate back to the HTB exercise you were going to work on.  Select `Spawn Machine`

![](../Images/SpawnMachine.png)

7. You should now be able to attack the IP address!  Happy [pwning](../Jargon.md)!