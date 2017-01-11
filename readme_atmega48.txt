AVR ZX-Spectrum Keyboard Controller for Atmega48
Version 5.5 (02.02.2016)

Features:
- NoWait version
- Additional buttons F11,F12
- Reset - PrScr
- C - Caps Lock
- E - ESC
- G - Del
- CapsShift - Shift (works really as on PC!)
- SymbolShift - Ctrl
- NumLock changes cursor keys and space to Sinclair Joystik

Removed saving indicators to EEPROM function
Extra optimized code

You may direct connect this controller to Keyboard port

/RDFE - is a signal from #FE port buffer Pin 1
(сигнал с дешифратора порта #FE, обычно приходит на певую ногу микросхемы ИР22 или ИР23 на которую идут биты данных клавиатуры)

Uploading:

	Use avrdude and USBAsp programmer

	avrdude -p atmega48 -c USBasp -U flash:w:KBD13_M48_nw_MODIFIEDv5_3_24MHz.hex -U lfuse:w:0xEE:m -U hfuse:w:0xD5:m



You may use sources to compile for different oscillators changing TIMING_COEFF value

ORIGIN: http://www.avray.ru