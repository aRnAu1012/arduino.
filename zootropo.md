# Zootropo

## Informacion 

Los puentes H son un tipo de componente conocido como un circuito integrado(CI). Los CI son componentes que contienen circuitos grandes en un paquete de tamaño reducido.

Ayudan a simplificar circuitos mas complejos al colocarlos en un componente facil de reemplazar. Por ejemplo , el puente H que estas usando en este ejemplo, tiene 

un numero de transistores integrados. 

Con un CI, puedes acceder a estos circuitos a traves de las clavijas que salen por los lados .

### Puente H 

El puente H contiene:

-Transitor + DIODO 

-No hay modulacion de velocidad 

-Sentido 0 

-ON/OFF

### Circuito integrado 

El circuito integrado contiene:

-Puente H

-Velocidad 

-Sentido 

-ON/OFF

## Codigo

 codigo Zootropo
```
const int controlPin1 = 2;
const int controlPin2 = 3;
const int enablePin = 9;
const int directionSwitchPin = 4;
const int onOffSwitchStateSwitchPin = 5;
const int potPin = A0;

int onOffSwitchState = 0;
int previousOnOffSwitchState = 0;
int directionSwitchState = 0;
int previousDirectionSwitchState =0;
int motorEnabled = 0;
int motorSpeed = 0;

int motorDirection = 1;
void setup(){ 
  pinMode(directionSwitchPin, INPUT);
  pinMode(onOffSwitchStateSwitchPin, INPUT);
  pinMode(controlPin1, OUTPUT);
  pinMode(controlPin2, OUTPUT);
  pinMode(enablePin, OUTPUT);
  digitalWrite(enablePin, LOW);
  Serial.begin(9600);
}
void loop(){
  onOffSwitchState = digitalRead(onOffSwitchStateSwitchPin);
  delay(1);
  directionSwitchState = digitalRead(directionSwitchPin);
  motorSpeed = analogRead(potPin)/4;
  Serial.println("Valor del botón On/OFf:");
  Serial.println(onOffSwitchState);
  Serial.println("Valor del botón Dirección:");
  Serial.println(directionSwitchState);
    Serial.println("Valor de la velocidad:");
  Serial.println(motorSpeed);
  if(onOffSwitchState != previousOnOffSwitchState){
    if(onOffSwitchState == HIGH){
      motorEnabled = !motorEnabled;
    }
  }
  if (directionSwitchState !=
  previousDirectionSwitchState) {
  if (directionSwitchState == HIGH) {
    motorDirection = !motorDirection;
    }
  }
  if(motorDirection ==1) {
    digitalWrite(controlPin1, HIGH);
    digitalWrite(controlPin2, LOW);
  }
  else {
    digitalWrite(controlPin1,LOW);
    digitalWrite(controlPin2,HIGH); 
  }
  if (motorEnabled == 1) {
    analogWrite(enablePin, motorSpeed);
  }
  else {
    analogWrite(enablePin, 0);
  }
  previousDirectionSwitchState =

```

codigo sacado de christian

## Imagen Zootropo 
[Imagen](https://raw.githubusercontent.com/Baultek/Arduino/main/imagenes%20arduino/zooooo.jpg)

Imagen sacada de JM





















































































































































































