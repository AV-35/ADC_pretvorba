# Enkratna_ADC_pretvorb

1. Cilj naloge: S pomočjo programskega okolja STM32CubeIDE in HAL knjižnicami sprogramirajte 
   ARM mikroprocesor tako,da bo izvedel posamične ADC pretvorbe z izbranim potenciometrom.

2. Postopek inicializacije periferije.  
    -  Uporabljena razvojna plošča je **NUCELO-F091RC**.  
    - Zeldena LED je priključena na **PA5** pinu, Modra LED pa na **PA6**. Na pin **PA0** je priključen potenciometer.  
    - Razvojna ploščica ima **1** ADC  pretvorbo.  
    - Trikotnik predstavlja opozorilo da je nekje knonflikt. V tem primeru je konflikt z:  

       * USART2: mode asynchronous na kanalu **IN2,IN3**  
       * PA5,PA6 ki sta uporabljena kot GPIO output na kanalih **IN5,IN6**

    - ADC ima **16** vhodnih kanalov.  
    - Za branje potenciometra je izbran kanal **IN0**. poleg pina se izpiše **ADC_IN0**.pin je **PA0**
    - Ostale možnosti ADC pretvorbe so:  
      |   6 bit    |    10 bit    |    12 bit    |
      | :--------: | :----------: | :----------: |
      | od 0 do 63 | od 0 do 1023 | od 0 do 4095 |
