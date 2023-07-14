# Raspberry PI for CC1101 E07-M1101S Modules

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-spring.jpg" alt="Pi with spring antenna"> 

This shield is used to hold [CC1101][1] Transceiver module with Raspbery PI. As soon as pinout is the same it should also works with 868 and/or 915 modules. You can easily find theese modules on Aliexpress.

It has just few minimal features, it has been created to be used for [Cyble RF 433Mhz][4] everblue reading water meter in France.

This shield can also act as a RF transceiver according already made or custom made software.    

## Features

**Version 1.0**

- Placement for E07-CC1101S 433MHz module
- Placement for choosing single Wire, SMA or u-FL Antenna type
- 3 x LED for visual indication

I received V1.0 boards from JLCPCB, they are working fine and as expected.


## Detailed Description

Look at the schematics for more informations.

SPI connexion is classic (MOSI/MISO/CLK), Chip Select is connected to CE0.


```
Raspberry PI   CC1101 Module 1
   GPIO22  <---->  GDO2 (unused in code)
   GPIO25  <---->  GDO0

Raspberry PI   On Board LEDS
   GPIO23  <---->  LED1 (Red)
   GPIO24  <---->  LED2 (Green)
   GPIO7   <---->  LED3 (Blue)
```


### Schematics

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-sch.png" alt="Schematics">    

### Boards  

### PCB

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-top.png" alt="Top">    

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-bot.png" alt="Bottom"> 

### Assembled boards

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-top.jpg" alt="Top Assembled">    

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-bot.jpg" alt="Bottom Assembled"> 

### Connected to Raspberry PI.

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-spring.jpg" alt="Pi with spring antenna"> 

<!--
<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-sma.jpg" alt="Pi with spring antenna"> 
-->

### Batch

<img src="https://raw.githubusercontent.com/hallard/cc1101-e07-pi/master/images/cc1101-pi-batch.jpg" alt="CC1101-PI Batch"> 

I'll put some of these board on tindie so you will be able to get one soon.

## Firmware

Software original code (but also all the hard work to get thingd working was originaly done [here][4] then put on github by @neutrinus [here][5].

I added some changes to the original firmware and this [one][6] should run out of the box with this board, just plug, and play.

## License

You can do whatever you like with this design.

## Misc

See news and other projects on my [blog][2] 

[1]: https://www.cdebyte.com/products/E07-M1101S
[2]: https://hallard.me
[3]: https://oshpark.com/shared_projects/BVwV2j3b
[5]: https://github.com/neutrinus/everblu-meters
[6]: https://github.com/hallard/everblu-meters-pi
[4]: http://www.lamaisonsimon.fr/wiki/doku.php?id=maison2:compteur_d_eau:compteur_d_eau
