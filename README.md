Uses a Wiznet w5500-evb-pico board: https://docs.wiznet.io/Product/iEthernet/W5500/w5500-evb-pico

![image](https://github.com/andrewmk/IP-keyboard/assets/1872642/91c6d3b5-5c01-44a7-adeb-582798374d89)

Running CircuitPython 9.0.4: https://downloads.circuitpython.org/bin/wiznet_w5500_evb_pico/en_GB/adafruit-circuitpython-wiznet_w5500_evb_pico-en_GB-9.0.4.uf2

UK keyboard layout from here: https://github.com/Neradoc/Circuitpython_Keyboard_Layouts

Send UDP commands to the board:
```
echo 'ALT ESCAPE,DELAY 2000,ALT ESCAPE,RIGHT,RIGHT,RIGHT,RIGHT,RIGHT,ENTER' | nc -q0 -u 192.168.1.100 5000
```
```
echo 'WINDOWS R,DELAY 500,STRING notepad.exe,ENTER,DELAY 500,Hello World!' | nc -q0 -u 192.168.1.100 5000
```
