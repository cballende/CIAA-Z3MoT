# CIAA-Z3MoT
Simplificación de base board Silabs subGHz :
EZR32 Happy gecko board for QFP48 parts (EZR32HG)
https://www.silabs.com/products/development-tools/wireless/proprietary/slwstk6244a-ezr32-happy-gecko-169-mhz-starter-kit

| Kit        | Frequency(MHz)| Output Power(dBm) |Included Device |
| ------------- |:-------------:| -----:|-----:|
| SLWSTK6244A     | 169 | +20 | ZR32HG330FG63G |

#### Caracteristicas

Adaptacion de CIAA-Z3R0 hacia un enfoque de MoTe.

Los pines entre Z3R0 y Z3MoT son compotatibles en cierto grado, con exepción de los destinados a las interfase RF.

Puertos y pines deprecados de la version Z3RO a la Z3MoT:
A:2,8,9,10.
C:0,1,2,3,4.

Introduce 4 GPIO: 
Se utilizan 3 lineas para configurar puerto I2C para memoria EEPROM y posibles MEMs(disponibles V2.0,temperatura,humedad,6DOF,Altimetro-barometro,luxometro)

Deja un GPIO libre comfigurable sobre los restantes puertros:
A:0,1.
B:7,8,11,13,14.
C:8,9,10,14,15.
D:4,5,6,7.
E:10,11,12,13.
F:0,1,2,3,4.

USB:
El conector usb se modifico, no se utiliza conector  soldable. Se implemento un plub en pcb USB A troquelable, brindando la posiblidad soldar tira de pines de paso 1,27" o soldar en PCB tipo castellated.

Alimentacion:
La alimentación se lecciona mediante jumper permitiendo conmutar bateria o (USB / PCBtarget).
La alimentacion mediante bateria, implementa una fuenta DC/DC tipo boost.

Autonomía:
El stick Z3MoT tiene la posiblidad de usar baterias tipo boton CR2034(3V) o mediante Pila AAA(1,5V). 

Conectores RF:
Es posible utilizar dos tipos de conectores uno SMD(por defecto) y otro SMA(soldando via).

JTAG:
Los pines utilizados en Z3RO son los mismos que para Z3MoT. Se adiciona tira de pines para conección ordenada de JTAG  mediante sondas con resortes montadas sobre una pinza o base con balancin.
 
![board schematic](https://i.ebayimg.com/images/g/XOYAAOSwB3tZplju/s-l1600.jpg)
![board schematic](ciaa-z3mot.svg)
![alt text](https://i.ebayimg.com/images/g/XOYAAOSwB3tZplju/s-l1600.jpg)

#### Schematic

[Schematic in pdf](ciaa-z3mot.pdf)
![board schematic](ciaa-z3mot.svg)


#### 3D view

![boar dimage](ciaa-z3mot-front.png)
![boar dimage](ciaa-z3mot-lat.png)

Vista con opciones de bateria y conector RF
![boar dimage](ciaa-z3mot-perspec.png)

![boar dimage](hand-coin.jpeg)

