
https://github.com/d-prieto

# 1 Trimestre

##  Arduino 


# Errores de programacion.
![imagen](https://user-images.githubusercontent.com/90753272/137865734-e17053bf-9ccb-49f3-998d-a25b733f8065.png) imajen de christian

# Errores de programacion.
![imagen](https://user-images.githubusercontent.com/90753272/137865875-96d1987e-9cdb-4ee9-bdbd-adf1bc371ddc.png) imajen de christian


 # Circuitos Electricos 
Intentamos programar , el programa de ejemplo blink.ing, lo que ocurrio fue,
que el programa , con el USB no daba permiso.


## Erorres y exepciones 
-BUG:Es un tipo de error pero no esperado ( el programa deberia hacer una cosa y hace otra cosa totalmente diferente). 
-GLITCH: Es un tipo de Bug grafico , cualquier comportamiento grafico no esperado.                                       
-ERROR : Operacion no permitida.
-Excepcion: Son errores que estan controloados por el mismo programa.
-Lag: Es un retraso en las comunicaciones.

## Primeros circuitos 
Esto pese a funcionar y dar luz genera dos problemas:
El primero se calienta y es incomodo de tocar. 
El segundo puede fundir el led.
 +5 voltios ----LED1----LED2----LED3----LED4
 
 En los circuitos en serie ----> Si desconectamos una parte todo se apaga
 
 ## Primera prueba con boton
 
 ![imagen](https://user-images.githubusercontent.com/90753272/137865286-424499cd-6f6f-4f85-b709-84e09d1b6365.png) imajen de christian

 
 ## Apuntes sobre electricidad :
  Voltaje ---> Altura (Diferencia de potencial)
  Intensidad o Amperaje ---> Cantidad de agua a rotuladores
  Resistencia ----> Resistencia al paso del agua a rotuladores
  Intensidad = Voltaje /resistencia ---> Ley de Ohm
 
 Voltaje = Intensidad * Resistencia
 
 Resistencia = Voltaje/Intensidad
  
### Por que necesitamos ressistencias con los Leds ?  
  Tenemos 2 circuitos 
  5V le ponemso un led  Y VAMOS A GND
  5V le ponemos una resistencia y vamos a GND
  
  El voltaje de los dos circuitos es de 5V
  
  ¿La resistencia?
  1 OHM 
  
  I = V(V)/R(OHM)
  
  5V/441 OHM = 11'33 mA
  
  5V/1 OHM = 5 Amperios 
  
  Cortocircuito Evitar:
  5V / 0 ohm = INFINITO A 
  
  ### Primera "Prueba.md"
  Lenguaje:
 descodificador de señales extraterrestres 
 Lenguaje maquina 
 Lenguaje de programacion :
 C
 C++
 Python
 JAVA
 
1010---->
  
### Lenguaje de programacion :

### C++:
2 FUNCIONES:
(Preparacion)SETUP()----> LO QUE SE PONE AL PRINCIPIO SE EJECUTA UNA SOLA VEZ : HACER UN PASTEL()
(Bucle)LOOP()----->Se ejecuta despues y se repite indefinidamente : HACER UNA TORTILLA()

## ejemplo:
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}



## Probando diferentes numeros  

// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever

void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(50);                       // wait for a second
}
 Lo que ha pasado es que se enciende mas de 1 segundo pero al apagarse se apaga muy rapido para que se vuelva a encender-se 
 
 void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   
  delay(150);                      
  digitalWrite(LED_BUILTIN, LOW);    
  delay(200); 


  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000);
  digitalWrite(LED_BUILTIN, LOW);
  delay(250);
}



 ## Como programar Arduino:
 -Primero tenemos arduino IDE instalado.
 -Tenemos un usuario con permiso.
 - Despues conectamos el Arduio por USB.
 - Cargamos el programa Blink.INO 
 - Desde dentro de Arduino buscamos Archivo ---> ejemplos ---> 1.Basics--->Blink.
 - Pulsamos el boton Subir
 
 - Errores posibles:
 - Si no hay puertos --->Herramientas ---> Puerto.
 - Fert Busy ---> Esperad 1 min aprox , sin desenchufar Arduino.
 - Conseguimos programar el Blink.INO 
   1-> buscarlo en Internet --->Arduino.cc
   2->Subirlo nosotros / Programas --->Blink.INO ---> subimos la carpeta al repositorio .
   3->Enlazar en primeras pruebas.md
   
   Otras opciones:
   -Captura de pantalla (Dificil de Regular)
   -Copiar ,pegar el codigo 
   """ C++ ---> 3 acentos graves.
   Bien para añadir texto.
  
  
  
  ## codigo morse nombre:



-->Morse 1: Hicimos modificaciones en el codigo para canbiar el tiempo de brillo.Para eso hicimos cambios en las lineas delay(-);

  # Que hace Blink.INO
  
  void loop ()[
  cuatro sentencias (o lineas)
  ]
 
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second

  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second

   digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(200);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(500);                       // wait for a second
  }
  delay(_)
  Nos pide un numero 
  Ese numero seran los milisegundos de espera 
  50 = 0"05 ---> el ojo humano no lo ve.
  1000 ----> 1s 
  60.000---> 1 minuto 
  500---> medio segundo
  -Hicimos un pulso largo y un pulso corto.


Morse 2 
 [enlace]("file:///home/usuario/Escritorio/morse_2") 
 
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop(){
  
  punto();
  raya();
  punto();
  raya();
  punto();
  raya();
  punto();
  punto();
  raya();
  punto();
  punto();
  raya();
  delay(2000);
}

// the loop function runs over and over again forever
  void punto  () {
  digitalWrite(LED_BUILTIN, HIGH);   
  delay(100);                      
  digitalWrite(LED_BUILTIN, LOW);    
  delay(300); 
  }

void raya (){
  digitalWrite(LED_BUILTIN, HIGH);
  delay(800);
  digitalWrite(LED_BUILTIN, LOW);
  delay(300);
}

  




[enlace]("file:///home/usuario/Escritorio/morse_3") morse 3

void loop(){
  //A
  punto();
  raya();
  //R
  punto();
  raya();
  punto();
  //N
  raya();
  punto();
  //A
  punto();
  raya();
  //U
  punto();
  punto();
  raya();
  delay(2000);
}

// the loop function runs over and over again forever
  void punto  () {
  digitalWrite(LED_BUILTIN, HIGH);   
  delay(100);                      
  digitalWrite(LED_BUILTIN, LOW);    
  delay(300); 
  }

void raya (){
  digitalWrite(LED_BUILTIN, HIGH);
  delay(800);
  digitalWrite(LED_BUILTIN, LOW);
  delay(300);
}
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
