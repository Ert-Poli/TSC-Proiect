Prezentare Generală
OpenBook ESP32-C6 este o platformă hardware portabilă și eficientă energetic, concepută pentru aplicații embedded. Aceasta are la bază microcontrollerul ESP32-C6-WROOM-1-N8, ce oferă suport pentru Wi-Fi 6 și Bluetooth 5.0 Low Energy, precum și o varietate de interfețe pentru conectarea senzorilor și a altor module externe. Sistemul integrează un ecran e-paper, senzor de mediu BME688, ceas în timp real DS3231SN, memorie NOR Flash de 64MB, cititor pentru card microSD și un sistem de alimentare pe bază de baterie LiPo, cu încărcare integrată și monitorizare a nivelului de energie.

Componente Hardware
ESP32-C6
Microcontrollerul ESP32-C6 gestionează întreaga funcționare a sistemului, inclusiv comunicarea cu perifericele, procesarea datelor și optimizarea consumului energetic.

Arhitectură RISC-V pe 32 de biți

Frecvență: până la 160 MHz

Conectivitate: Wi-Fi 6, Bluetooth 5.0

GPIO-uri versatile pentru interfețe I2C, SPI și UART

Modul RTC – DS3231SN
Ceas în timp real cu precizie ridicată și compensare termică

Funcționează independent de sistem, chiar și în mod oprit

I2C partajat cu senzorul de mediu

Senzor BME688
Măsoară temperatura, umiditatea, presiunea și compuși volatili (VOC)

Conectat pe magistrala I2C comună cu RTC

Ideal pentru analiza condițiilor ambientale și optimizarea afișajului

Ecran E-Paper
Tehnologie de afișaj pasivă, cu consum extrem de redus

Controlat prin SPI și pini RST, DC, BUSY

Dimensiune: 7.5"

Rezoluție: 800x480 px

Memorie NOR Flash – 64MB
Model W25Q512JVEIQ

Stocare SPI pentru loguri și grafice e-paper

Slot microSD
Alternativă de stocare pentru volume mari de date

Comunică prin SPI, cu chip select dedicat

Sistem de Alimentare
Intrare USB-C cu protecție ESD

Suportă baterii LiPo de 3.7V, minim 1500mAh

Încărcător: MCP73831

Monitorizare nivel baterie: MAX17048 (I2C)

Stabilizare tensiune: LDO 3.3V

Protecție și Conectivitate
USB-C cu protecție ESD și diodă Schottky pentru polaritate inversă

Asigură atât alimentare cât și transfer de date

Interfață cu Utilizatorul
Butoane tactile pentru controlul funcțiilor

Conector Qwiic pentru extinderea cu senzori I2C

GPIO-uri disponibile pentru alte extensii

Interfețe de Comunicație
SPI – utilizat pentru e-paper, card SD și memoria NOR Flash

I2C – folosit pentru BME688, DS3231SN și MAX17048

UART – debug și programare

GPIO – pentru control general și butoane

Wireless – conectivitate prin Wi-Fi 6 și BLE 5.0

Supraveghere Tensiune și Reset
Circuit de monitorizare pentru tensiunea de alimentare

Reset automat în caz de instabilitate

Afișare nivel încărcare baterie

Dimensiuni și Design Fizic
Dimensiunea plăcii PCB: aprox. 92 x 54 mm

Design compact, ideal pentru integrarea într-o carcasă personalizată

Specificații Cheie
Consum minim datorită ecranului e-paper și optimizării energetice

Suport extins pentru conectivitate wireless

Măsurători de mediu în timp real

Arhitectură modulară pentru personalizare și extindere facilă

Suport stocare externă pe card microSD

Autonomie ridicată pe baterie

Funcționalitate Software
Compatibilitate cu diverse formate de e-book-uri

Interfață intuitivă pentru citire și navigare

Sincronizare wireless cu dispozitive și servicii externe

Posibilități avansate de personalizare a experienței de utilizare

Logare și analiză a datelor de mediu

Considerații de Design
PCB optimizat pentru reducerea zgomotului electric și creșterea eficienței

Componente cu consum redus alese atent pentru fiabilitate maximă

Sisteme de protecție integrate pentru siguranță

Dimensiuni mici pentru portabilitate crescută

Conectivitate ESP32-C6

Pin ESP32-C6	Funcție	Legat la
IO0	SPI MOSI	E-paper, SD Card, Flash
IO1	SPI MISO	SD Card, Flash
IO2	SPI CLK	Toate dispozitivele SPI
IO3	SPI CS	E-paper
IO4	SPI CS	NOR Flash
IO5	SPI CS	SD Card
IO6	I2C SDA	BME688, RTC, Fuel Gauge
IO7	I2C SCL	BME688, RTC, Fuel Gauge
IO8	Buton Boot	GND prin rezistor
IO10, IO11	UART0	Programare / Debug
EN	Enable MCU	Pull-up la 3.3V
