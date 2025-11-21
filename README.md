# Vaja2-ADC-continuos-conversion-Nucleo
PINOUT KONFIGURACIJA:\
![pinout](https://github.com/Hudi452/Vaja2-ADC-continuos-conversion-Nucleo/blob/main/Izrezek%20pinout.png)

SLIKI KONFIGURACIJSKIH OKEN:\
![konfig1](https://github.com/Hudi452/Vaja2-ADC-continuos-conversion-Nucleo/blob/main/Izrezek%20konfiguracijskega%20okna1.png)\
![konfig2](https://github.com/Hudi452/Vaja2-ADC-continuos-conversion-Nucleo/blob/main/Izrezek%20konfiguracijskega%20okna2.png)

FOTOGRAFIJA VEZAVE:\
![vezje](https://github.com/Hudi452/Vaja2-ADC-continuos-conversion-Nucleo/blob/main/Slika%20vezja.PNG)

VIDEO DELOVANJA:


ODGOVORI NA VPRAŠANJA:\
b)Pod Analog so 3 ADC pretvorniki.\
c)PC0\
d)ADC1_IN1\
e)Spremenijo se frekvence od HCLK in APB1 Prescaler\
g)Preskalirana vrednost je sedaj 4MHz (f_preskalirana = 16 MHz/4 = 4 MHz).\
i)t_vz_ciklih = 247,5    
t'_vz_ciklih = t_vz_ciklih + 12,5 = 247,5 + 12,5 = 260\
t_vz = t'_vz_ciklih/f_preskalirana = 260/(4000000)= 65 us

KOMENTAR:\
Večkratna ADC pretvorba deluje po pričakovanjih. S tem ko potenciometer sučemo iz ene lege proti drugi se analogna vrednost spreminja od 0 do 255. ADC pretvorba se izvaja zelo hitro in je omejena samo s časom vzorčenja. Ko jo pričnemo z HAL_ADC_Start() pod USER CODE BEGIN 2 se pretovrba začne izvajati neprekinjeno.


