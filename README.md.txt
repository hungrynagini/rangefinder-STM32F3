Використовуючи далекомір HC-SR04 та дисплей від Nokia 5110 (червоний), ми отримуємо через піни TRIG та ECHO на STM32F3 
інформацію, яку зібрав далекомір, а також використовуємо один SPI, під'єднуючи пін SPIx-SCK мікроконтролера до 
піна дисплею (CLK), SPI-MOSI відповідно до піна DIN,та три піни керування дисплею - RST, CE, DC, щоб передати 
інформацію на дисплей чорним кольором.
Для того щоб не виводити багато інформації на маленький дисплей, ми вирішили виводити лише коди помилок, 
які залежать від стану пінів далекоміра:
Code 1:"Wrong state before triggering, Trig is high\n"
Code 2:Line Trig do not went high while triggering.\n
Code 3:Line Trig do not went low after triggering.\n
Code 4:Line ECHO is high too early.\n
Code 5:Line ECHO didn't go high for a long time.\n
Code 6:Line ECHO didn't go low after echoing pulse stared for a long time.\n
Code 7:\tToo far -- possibly no echo at all.