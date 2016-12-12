# PortScan

<img alt="python-logo" width="180" src="https://raw.githubusercontent.com/Sup3r-Us3r/PortScan/master/Screenshots/python-logo.png">

### -> See more at:

* [Python](https://www.python.org/)
* [Arch Linux](https://www.archlinux.org/)


### `Screenshots of project:`

![Spyquiz.py][screenshot1]

![Url.py][screenshot2]

![Início][screenshot3]


[screenshot1]:https://raw.githubusercontent.com/Sup3r-Us3r/PortScan/master/Screenshots/1.png
[screenshot2]:https://raw.githubusercontent.com/Sup3r-Us3r/PortScan/master/Screenshots/2.png
[screenshot3]:https://raw.githubusercontent.com/Sup3r-Us3r/PortScan/master/Screenshots/3.png

### # About the project.

> PortScan.py aims to check open and closed ports quickly, It prompts you to inform a host that can be `LOCAL IP` `EXTERNAL IP` and `WEBSITE` because it converts the host informed and automatically searches its source IP address, it also asks to inform a start port and an end but if you want to check a only door you can too. it was developed in [Python 3.5](https://www.python.org/) and the System used was [Arch Linux](https://www.archlinux.org)

 * The part of the code responsible for converting from HOST to IP is:

~~~python
from socket import *

def escanear():
    menu()
    try:
        host = input("\033[31mDigite o host:\033[1;m ")
        print("")
    except:
        escanear()
    try:       
        ip = gethostbyname(host)
        print("\033[31mEndereco IP ▬▶\033[1;m %s \n" %(ip))
    except:
        print("\033[31mHost invalido.\033[1;m")   
        sleep(3)
        escanear()
~~~

* Creator [Sup3r-Us3r](https://github.com/Sup3r-Us3r)

---------

### Installation and use.

```sh
$ sudo pacman -S git // or sudo apt-get install git
$ git clone https://github.com/Sup3r-Us3r/PortScan.git
$ cd PortScan
$ sudo chmod +x portscan.py
```
To use.
```sh
$ ./portscan.py
```
> Dependency python3.5




