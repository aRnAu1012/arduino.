# Operaciones 

Y
O
NO

IF (condicion) ---- SI (True) ------No (FALSE)
    VARIABLE   VALOR          
OUTPUT ---> Stiven activate

if (temperature <= baselinetemp)
}

TEMPERATURA ( 15 C - 80 C)

Sensorvalue (0 - 1.024)



Leer PIN A0
    Analog read ---> 0 - 1023 (8 bytes ) 

Transforma los valores :
          Y, de Regalo , las pinta en pantalla.
         
 -Decidir:
  T < 20 
  
  DigitalWrite = Es una función que nos pide un numero de pin y el valor HIGH ( 1 ) o LOW (0)
  
  si el valor es HIGH la placa suministrara 5 voltios en ese pin 
  
  si el valor es LOW la placa suministrara 0 voltios en ese Pin.
  
  Si hay 5 V se activaran dos circuitos si es 0 V no se activaran.
  
  ejemplo:
   
 DigitalWrite ( 4 ; LOW ); o digitalWrite (4,0); se desactivaran los numeros de los pines 
  
 Si es high se activaran 5 V A los numeros de los pines.
  
  
  
} Else if (temperature >= baselineTemp +2 && temperature < baselineTemp +4){

DW ( 2,HIGH );
DW (3,LOW );
DW (4,LOW );

} Else if (temperature >= baselineTemp +4 && temperature < baselineTemp +6){

DW (2,HIGH);
DW (3,HIGH);
DW (4,LOW);


 } Else if (temperature >= baselineTemp +6) {
 
DW (2,HIGH);
DW (3,HIGH);
DW (4,HIGH);

## Conectar dos botones 

-Ejercicio 
Vamos a conectar 2 botones y 2 leds 
 
Haremos diferentes programas con diferentes comportamientos 

Para poner un boton necesitamos una resistencia de 10.000 Ohmios. Estas son las que tienen cuerpo BEIGE y una linia naranja.

Esquema de boton " Por defecto arriba o "pulled -HIGH "

Conectaremos 2 botones .UNO al Pin 2 , Pin 3 

Para poner un Led necesitamos una resistencia de 220 OHMIOS las de cuerpo azul.

Hay que tener en cuenta la polaridad del led.

La pata mas corta va hacia el GND ( o 0 V ) y la larga hacia el Voltaje.

Pin -----> led ----> 220 OHMNIOS --- GND 

Da igual si la resistencia va detras o delante del led.

Conectaremos 2 leds . Uno al Pin 4 y otro al Pin 5.






































  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
