AVR ZX-Spectrum Keyboard Controller for Atmega8 (Atmega8A)
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
(������ � ����������� ����� #FE, ������ �������� �� ����� ���� ���������� ��22 ��� ��23 �� ������� ���� ���� ������ ����������)

Uploading:

	Use avrdude and USBAsp programmer

	avrdude -p atmega8 -c USBasp -U flash:w:KBD13_M8_nw_MODIFIEDv5.hex -U lfuse:w:0xCF:m -U hfuse:w:0xC7:m



You may use sources to compile for different oscillators changing TIMING_COEFF value

ORIGIN: http://www.avray.ru