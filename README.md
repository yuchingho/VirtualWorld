 Link for models - https://www.outworldz.com/cgi/freesculpts.plx
 
## Login Details (case-sensitive)
| First name | Last name | Password | IP address |
| :--- | :---: | :---: |:--- |
| david | sim | 123456 | ```http://127.0.0.1:9000/``` |
| habtamu | sim | 123456 | ```http://127.0.0.1:9000/``` |
| manuel | sim | 123456 | ```http://127.0.0.1:9000/``` |
| tomis | sim | 123456 | ```neoptolemospapa.hopto.org:9000/```|
| yoshi | sim | 123456 | ```http://127.0.0.1:9000/``` |

<p align="center">
  <img src="https://github.com/yuchingho/VirtualWorld/blob/master/README%20Images/University%20IPv4.png?raw=true" alt="Univerisity IPv4"/>
</p>

## Steps to log into a Server
1. Launch ```Imprudence``` Do not launch ```OpenSim.32BitLauch```
2. Create new Grid Manager or select the one with the host's IP Address
3. Type in host's IP Address into Login URI - ```http://(IP Address):9000/```
4. Login with ```Login Details```

## Steps to set up Server in UWS
1. Launch ```OpenSim.32BitLaunch```
   - Wait till LaptopIsland has finished loading.
2. Launch ```Imprudence```
3. Check "Login Details" section, and login:
   - Grid Manager - ```Local Host```
   - Login URI - ```http://127.0.0.1:9000/```
4. Server is now up and running.

## Steps to set up Server at Home from [this website](https://chapter-and-metaverse.blogspot.com/2008/11/3-remotely-connecting-to-standalone-sim.html)
1. Set up a Static IP Address:\
Very easy and user friendly instructions from [this website](https://portforward.com/networking/static-ip-windows-10.htm) for Windows 10.\
For other platforms such as Windows 8,7 etc, use [this website](https://portforward.com/networking/staticip.htm) to find what suits you.

2. PortForwarding Impudence Ports:\
Find the default gateway:\
Type ```cmd``` in Windows Search to open up the Command Prompt.\
Type ```ipconfig```
<p align="center">
  <img src="https://github.com/yuchingho/VirtualWorld/blob/master/README%20Images/DefaultGateway.png?raw=true" alt="DefaultGateway"/>
</p>

Type the ```default gateway value``` into your browser and the home page of your router show.
<p align="center">
  <img src="https://github.com/yuchingho/VirtualWorld/blob/master/README%20Images/Home%20Page.png?raw=true" alt="Home Page"/>
</p>

You will need to find ```Port Forwarding``` in the Settings.
<p align="center">
  <img src="https://github.com/yuchingho/VirtualWorld/blob/master/README%20Images/Port%20Initialize.png?raw=true" alt="Port Initialize"/>
</p>

You will need to add some ports ```TCP/8000-8005```, ```TCP/8895```, and ```UDP/TCP/9000``` for a single sim, and ```UDP/TCP/9001``` for a second sim, and so on...
<p align="center">
  <img src="https://github.com/yuchingho/VirtualWorld/blob/master/README%20Images/Port%20Setup%20Complete.png?raw=true" alt="Port Setup Complete"/>
</p>

3. Setup a Dynamic DNS hostname Service:\
We are using ```https://www.noip.com/``` to create a host name and use their application to work as a server.\
Create an account, install the application and create a hostname through the application or their website.
 
4. Configure your OpenSim Software for an External Connection:\
The next step is to configure the OpenSim software.
    - Go to the ```Bin/Regions/default.xml``` file.
    - Right-click and Open with Notepad. 
    - Change the ```external_host_name```, which can be your DNS host name, so it will look something like this:\
    ```external_host_name="garys-sim.servegame.org"```

5. Launch the ```DUC(noip) application``` then launch ```OpenSim.32BitLaunch```.

6. The Login URI should be the hostname created with ```noip``` and it should look something like this:\
```neoptolemospapa.hopto.org:9000/```