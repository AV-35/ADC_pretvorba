# Enkratna_ADC_pretvorb

1. Cilj naloge: S pomočjo programskega okolja STM32CubeIDE in HAL knjižnicami sprogramirajte 
   ARM mikroprocesor tako,da bo izvedel posamične ADC pretvorbe z izbranim potenciometrom.

2. Postopek inicializacije periferije.  
    -  Uporabljena razvojna plošča je **NUCELO-G431RB**.  
    - Zeldena LED je priključena na **PA5** pinu, Modra LED pa na **PA6**. Na pin **PA0** je priključen potenciometer.  
    - Razvojna ploščica ima **2** ADC  pretvorbo.  
    - Trikotnik predstavlja opozorilo da je nekje med pini knonflikt.  
    - ADC ima **17** vhodnih kanalov.  
    - Za branje potenciometra je izbran kanal **IN1**. poleg pina se izpiše **ADC1_IN1**.pin je **PA0**
    - Ostale možnosti ADC pretvorbe so:  
      |   6 bit    |    10 bit    |    12 bit    |
      | :--------: | :----------: | :----------: |
      | od 0 do 63 | od 0 do 1023 | od 0 do 4095 |
