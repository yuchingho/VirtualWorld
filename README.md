## Steps to set up a home server
-Source: https://chapter-and-metaverse.blogspot.com/2008/11/3-remotely-connecting-to-standalone-sim.html

1. set up a Static IP Address 
   Very easy and user friendly instructions from this website for windows 10.
   https://portforward.com/networking/static-ip-windows-10.htm
   For other platforms such as windows 8,7 etc, use this website to find what suits you.
   https://portforward.com/networking/staticip.htm
2. PortForwarding Impudence ports
   In order to that you will need to find the default gateway of your computer by typing "cmd" in the windows search and then typing        inside cmd ipconfig.
   <p align="center">
   https://github.com/yuchingho/VirtualWorld/blob/master/DefaultGateway.png
   </p>
   Type the default gateway value in your internet browserand the home page of your router will pop and look similar to this.
<p align="center">
https://github.com/yuchingho/VirtualWorld/blob/master/Page.png
</p>
   You will need to find something that is called Portforward somewhere in the settings or advanced settings or anywhere really since you have your own ISP portforward would be somewhere in there.
<p align="center">
https://github.com/yuchingho/VirtualWorld/blob/master/pORT.png
</p>
You will need to add some ports(TCP/8000-8005, TCP/8895, and UDP/TCP/9000 for a single sim, and UDP/TCP/9001 for a second sim, and so on)
<p align="center">
   
 </p>
Link for models - https://www.outworldz.com/cgi/freesculpts.plx

## Steps to set up a University Server 
1. Launch "OpenSim.32BitLaunch".
   - Wait till LaptopIsland has finished loading.
2. Launch "Imprudence".
3. Check "Login Details" section, and login.
   - Grid Manager == Local Host
   - Login URI == http://127.0.0.1:9000/
4. Server is now up and running.

## Steps to log into Server
1. Launch "Imprudence". Do not launch "OpenSim.32BitLauch".
2. Create new Grid Manager or select the one with the host's IP Address
3. Type in host's IP Address into Login URI
   - http://(IP Address):9000/
4. Login with "Login Details"

## Login Details (case-sensitive)
| First name | Last name | Password | IP address |
| :--- | :---: | :---: |:--- |
| david | sim | 123456 | http://(IP Address):9000/ |
| habtamu | sim | 123456 | http://(IP Address):9000/ |
| manuel | sim | 123456 | http://(IP Address):9000/ |
| tomis | sim | 123456 | http://(IP Address):9000/ |
| yoshi | sim | 123456 | http://(IP Address):9000/ |

<p align="center">
  <img src="https://github.com/yuchingho/VirtualWorld/blob/master/server%20in%20uni.png?raw=true" alt="server in uni"/>
</p>
