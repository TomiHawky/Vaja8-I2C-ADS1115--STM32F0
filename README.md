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
