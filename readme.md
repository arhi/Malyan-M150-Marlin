
To burn customized code, please reference command:
avrdude -F -V -p m2560 -P COMX -c stk500v1 -b 57600 -U flash:w:filename.hex 

To backup hex from mcu (not tested, might work):
avrdude -C avrdude.conf -v -v -v -v -p atmega1284p -c stk500 -U flash:r:"c:/arduino.hex":r -P\\.\COM2 -b57600
