# Molinillo Motorizado 

## INFORMACION

Transistores = son componentes que te permiten controlar fuentes de alta corriente y alto voltaje desde la salida de baja corriente del Arduino. 

Los transistores son como unos interruptores digitales.

Cuando suministras voltaje a una de las clavijas del transistor , llamado compuerta , la clavija cierra el circuito entre las otras dos clavijas, llamadas fuente

DRENAJE . De esta manera , puedes encender y apagar un montor de corriente/voltaje mas altos con arduino.

Los Motores = Son un tipo de dispositivo inductivo. 

La induccion es un processo por el que una corriente electrica variable en un cable puede producir un campo magnetico variable alrededor del cable.

Cuando a un motor se le suministra electricidad , una tensa bobina dentro de la carcasa de cobre crea un campo magnetico.Este campo hace que el eje gire.

Energia = Potencia * Tiempo

E = P*T

P = I * V2

Potencia = intensidad * Voltaje al cuadrado 

0,20W =   40 mA/0,04 A , 5V

I = V/R

Intensidad = Voltaje / Resistencia

## Codigo Molinillo
Codigo Molinillo
```C++
const int switchPin = 2;
const int motorPin = 9;
int switchState = 0;
void setup() {
  pinMode(motorPin, OUTPUT);
  pinMode(switchPin, INPUT);
}
void loop(){
  switchState = digitalRead(switchPin);

  if (switchState == HIGH){
    digitalWrite(motorPin, HIGH); 
  }
  else{ digitalWrite(motorPin, LOW);
}
}

```


## Foto
![foto](https://github.com/Samael696/arduino/blob/main/IMG_20220119_101702.jpg?raw=true)

Foto sacada por el repositorio de Andree.
             



