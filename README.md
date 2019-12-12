#Cypress SPI 2-byte adressed FRAM

This is the official Cypress library from their site for working with 2-byte addressed SPI FRAM. It is ready to use with Arduino IDE. If you have problems with accessing FRAM try to use

{SPI.beginTransaction(SPISettings(100000, MSBFIRST, SPI_MODE0));
<your FRAM access>
SPI.endTransaction();}

instead of regular  'SPI.begin();'