# Vaja8-I2C-ADS1115--STM32F0

Cilj naloge: S pomočjo STM32CubeIDE in HAL knjižnicami sprogramirajte mikroprocesor tako, da bo preko I
2C protokola prebral in prikazal analogne vrednosti iz 4-kanalnega ADC pretvornika ADS1115. Potrebujete 
tudi 4 trimerje/potenciometre, upore in kondenzator. Za prikaz spremenljivk potrebujete STM Studio (ali 
STM32CubeIDE v Debug načinu).

 1. SDA: PB7, SCL: PB6
 2. Omogoča 2 I2C povezavi
 3. | ADS 1115: | SCL | SDA | ADDR | ALRT         | VDD        |
    |-----------|-----|-----|------|--------------|------------|
    | STM32F0:  | PB6 | PB7 | GND  | (ni povezan) | 5 ALI 3.3V |
 4. Frekvenca znaša 400 KHz
 5. 1001000 bin = 0x48 HEX
 6. 6.144V
 
 
![Posnetek zaslona 2023-02-28 085711](https://user-images.githubusercontent.com/97598187/221790786-ab354530-127f-41f4-9d30-072b6241709a.png)
![Posnetek zaslona 2023-02-28 085638](https://user-images.githubusercontent.com/97598187/221790788-aab8f536-210d-4de6-b7ff-39fc147b6fae.png)
!(https://raw.githubusercontent.com/TomiHawky/Vaja8-I2C-ADS1115--STM32F0/main/IMG_20230228_085528.jpg)


7. Komentar: Z nalogo nisva imela velikih težav, edina večja težava je bila, da sistem ni zaznal potenciometra zato sva ga nadomestila z drugim.
