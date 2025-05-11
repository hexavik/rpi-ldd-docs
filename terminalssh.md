At the time of installing image in Raspberry Pi using Imager tool, edit the settings and enable the SSH connection and Wi-Fi connection by providing SSID and password. Along with this it is recommended to set up username and password.

Initially you need to login to the raspberry pi 5 with display attached  to get the IP address of the Raspberry Pi 5.

Once this is done you can handle Raspberry Pi 5 using SSH from your host machine:

```bash
ssh <rp-username>@<ip address>
e.g. ssh user123@192.168.1.78
```

