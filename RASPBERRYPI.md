RASPBERRYPI - INICIALIZAR


| Comando         | Descripción     | 
|-----------------|-----------------|
| ```ipconfig```  | Contenido 2     | 
| ```ping -4 raspberrypi```  | Contenido 5     | 
| ```ssh pi@raspberrypi```  | Contenido 8     | 
| ```sudo raspi-config nonint do_wifi_country MX```  | Contenido 8     |
| ```wpa_passphrase "<ssid>"```  | Contenido 8     | 
| ```sudo nano /etc/wpa_supplicant/wpa_supplicant.conf ```  | Contenido 8     | 
| ```ip a  ```  | Contenido 8     | 
| ```sudo reboot  ```  | Contenido 8     | 


ipconfig - ethernet
    -IPv4 - Ip

ping -4 raspberrypi
    -ip

ssh pi@raspberrypi
    -ssh <username>@<host>
    -ssh pi@169.254.129.216
    -ssh pi@raspberrypi.local

sudo raspi-config nonint do_wifi_country MX
     -configurate internet<ssid>

wpa_passphrase "<ssid>"
     -ssid = name network


network={
        ssid="kokas"
        #psk="kokaslocas"
        psk=10145daf900bc96424410826a95b4cb6f6b5147389df23193e8887a6ab294509
}

sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
      -configurar network

network={
  ssid="<ssid>"
  scan_ssid=1
  psk=<psk>
}

Save (ctrl + x, then y)
sudo reboot 

verificacion 
ip a - conectados

install pip in raspberry
   -sudo apt-get install python3-pip

install librerias
    -sudo pip3 install nombre_libreria
