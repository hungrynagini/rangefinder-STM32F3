�������������� �������� HC-SR04 �� ������� �� Nokia 5110 (��������), �� �������� ����� ��� TRIG �� ECHO �� STM32F3 
����������, ��� ����� ��������, � ����� ������������� ���� SPI, ��'������� �� SPIx-SCK �������������� �� 
��� ������� (CLK), SPI-MOSI �������� �� ��� DIN,�� ��� ��� ��������� ������� - RST, CE, DC, ��� �������� 
���������� �� ������� ������ ��������.
��� ���� ��� �� �������� ������ ���������� �� ��������� �������, �� ������� �������� ���� ���� �������, 
�� �������� �� ����� ��� ���������:
Code 1:"Wrong state before triggering, Trig is high\n"
Code 2:Line Trig do not went high while triggering.\n
Code 3:Line Trig do not went low after triggering.\n
Code 4:Line ECHO is high too early.\n
Code 5:Line ECHO didn't go high for a long time.\n
Code 6:Line ECHO didn't go low after echoing pulse stared for a long time.\n
Code 7:\tToo far -- possibly no echo at all.