Uses a Wiznet w5500-evb-pico board: https://docs.wiznet.io/Product/iEthernet/W5500/w5500-evb-pico
Running CircuitPython 9.0.4: https://downloads.circuitpython.org/bin/wiznet_w5500_evb_pico/en_GB/adafruit-circuitpython-wiznet_w5500_evb_pico-en_GB-9.0.4.uf2

Send UDP commands to the board:
```echo 'WINDOWS R,DELAY 500,STRING notepad.exe,ENTER,DELAY 500,Hello World!' | nc -q0 -u 192.168.1.100 5000
