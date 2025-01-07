RASPBERRYPI - INICIALIZAR


| Comando         | Descripción     | 
|-----------------|-----------------|
| ```ipconfig```  | Show ip   | 
| ```ping -4 raspberrypi```  | Check ip that using raspberry     | 
| ```ssh pi@raspberrypi or ip ```  | Conecting with the raspberry   | 
| ```sudo raspi-config nonint do_wifi_country MX```  | Setting the internet     |
| ```wpa_passphrase "<ssid>"```  | Encode the password of the internet     | 
| ```sudo nano /etc/wpa_supplicant/wpa_supplicant.conf ```  | Enter setting wifi    | 
| ```ip a  ```  | ip raspberry     | 
| ```sudo reboot  ```  | Reset raspberry     | 


1. ipconfig - ethernet
    * -IPv4 - Ip

2. ping -4 raspberrypi
    * -ip

3. ssh pi@raspberrypi
    * -ssh <username>@<host>
    * -ssh pi@169.254.129.216
    * -ssh pi@raspberrypi.local

4. sudo raspi-config nonint do_wifi_country MX
     * -configurate internet<ssid>

5. wpa_passphrase " ssid "
     * -ssid = name network

6. Network
     ```python
    network={
            ssid="name_network"
            #psk="password"
            psk=10145daf900bc96424410826a95b4cb6f6b5147389df23193e8887a6ab294509
    }
    ´´´

7. sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
    * -configurar network
    * Write 
        ```python
        network={
            ssid="<ssid>"
            scan_ssid=1
            psk=<psk>
        }
        
        ´´´

8. Save (ctrl + x, then y)
    * sudo reboot 

9. verificacion 
    * ip a - conectados

10. install pip in raspberry
    * -sudo apt-get install python3-pip

11. install librerias
    * -sudo pip3 install nombre_libreria

