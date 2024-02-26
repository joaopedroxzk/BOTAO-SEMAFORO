# BOTAO-SEMAFORO
// C++ code
//
const int buttonPin = 3;
int buttonState = 0;

void setup()
{
  Serial.begin(9600);
  pinMode(buttonPin,INPUT);
  pinMode(13, OUTPUT);//VERMELHO 1
  pinMode(12, OUTPUT);//VERDE 1
  pinMode(11, OUTPUT);//AMARELO 1
  pinMode(10, OUTPUT);//VERMELHO 2 
  pinMode(9, OUTPUT);//VERDE 2
  pinMode(8, OUTPUT);//AMARELO 2
  pinMode(7, OUTPUT);// vermelho P/1
  pinMode(6, OUTPUT);// verde p/1
  pinMode(5, OUTPUT);//vermelho P/2
  pinMode(4, OUTPUT);//verde P/2
 //o 1 é o de carros, e o 2 de pedestres 
  
}

void loop() { 

buttonState = digitalRead(buttonPin);

if (buttonState == HIGH){ 
  //SEMAFORO 1
  digitalWrite(13,HIGH);//VERMELHO 1
  Serial.println("Semaforo 1:");
  Serial.println("Vermelho está aceso");
  digitalWrite(12, LOW);//VERDE 1
  Serial.println("Verde está apagado");
  digitalWrite(11, LOW);// AMARELO 1
  Serial.println("Amarelo está apagado");
  
  //SEMAFORO 2
  digitalWrite(10,LOW);//VERMELHO 2
  Serial.println("Semaforo 2:");
  Serial.println("Vermelho está apagado");
  digitalWrite(9, HIGH);//VERDE 2
  Serial.println("Verde está aceso");
  digitalWrite(8, LOW);// AMARELO 2
  Serial.println("Amarelo está apagado");

  //pedestre 1
  digitalWrite(7,LOW);//VERMELHO p/1
  Serial.println("Pedestre 1:");
  Serial.println("Vermelho está apagado");
  digitalWrite(6,HIGH);// verde P/1
  Serial.println("Verde está aceso");

  //PEDESTRE 2
  digitalWrite(5,HIGH);//VERMELHO P/2
  Serial.println("Pedestre 2:");
  Serial.println("Vermelho está aceso");
  digitalWrite(4,LOW);//VERDE P/2 
  Serial.println("Verde está apagado");

  
  delay(3000); // Wait for 1000 millisecond(s)
  
  //SEMAFORO 1
  digitalWrite(13, HIGH);//VERMELHO 1
  Serial.println("Semaforo 1:");
  Serial.println("Vermelho está aceso");
  digitalWrite(12, LOW);//VERDE 1
  Serial.println("Verde está apagado");
  digitalWrite(11, LOW);//AMARELO 1
  Serial.println("Amarelo está apagado");

  //SEMAFORO 2
  digitalWrite(10,LOW);//VERMELHO 2
  Serial.println("Semaforo 2:");
  Serial.println("Vermelho está apagado");
  digitalWrite(9, LOW);//VERDE 2
  Serial.println("Verde está apagado");
  digitalWrite(8, HIGH);// AMARELO 2
  Serial.println("Amarelo está aceso");

  // PEDESTRE 1
  digitalWrite(7,LOW);//VERMELHO p/1
  Serial.println("Pedestre 1:");
  Serial.println("Vermelho está apagado");
  digitalWrite(6,HIGH);// verde P/1
  Serial.println("Verde está aceso");

  //PEDESTRE 2
  digitalWrite(5,HIGH);//VERMELHO P/2
  Serial.println("Pedestre 2:");
  Serial.println("Vermelho está aceso");
  digitalWrite(4,LOW);//VERDE P/2 
  Serial.println("Verde está apagado");
  
  delay(1500); // Wait for 1000 millisecond(s)
  
  //SEMAFORO 1
  digitalWrite(13, LOW);//VERMELHO 1
  Serial.println("Semaforo 1:");
  Serial.println("Vermelho está apagado");
  digitalWrite(12, HIGH);//VERDE 1
  Serial.println("Verde está aceso");
  digitalWrite(11,LOW);//AMARELO 1
  Serial.println("Amarelo está apagado");

  //SEMAFORO 2
  digitalWrite(10,HIGH);//VERMELHO 2
  Serial.println("Semaforo 2:");
  Serial.println("Vermelho está aceso");
  digitalWrite(9, LOW);//VERDE 2
  Serial.println("Verde está apagado");
  digitalWrite(8, LOW);// AMARELO 2
  Serial.println("Amarelo está apagado");

  //PEDESTRE 1
  digitalWrite(7,HIGH);//VERMELHO p/1
  Serial.println("Pedestre 1:");
  Serial.println("Vermelho está aceso");
  digitalWrite(6,LOW);// verde P/1
  Serial.println("Verde está apagado");

  //PEDESTRE 2
  digitalWrite(5,LOW);//VERMELHO P/2
  Serial.println("Pedestre 2:");
  Serial.println("Vermelho está apagado");
  digitalWrite(4,HIGH);//VERDE P/2 
  Serial.println("Verde está aceso");
  
  delay(3000); // Wait for 1000 millisecond(s)
  
  //SEMAFORO 1
  digitalWrite(13, LOW);//VERMELHO 1
  Serial.println("Semaforo 1:");
  Serial.println("Vermelho está apagado");
  digitalWrite(12, LOW);//VERDE 1
  Serial.println("Verde está apagado");
  digitalWrite(11,HIGH);//AMARELO 1
  Serial.println("Amarelo está aceso");

  //SEMAFORO 2
  digitalWrite(10,HIGH);//VERMELHO 2
  Serial.println("Semaforo 2:");
  Serial.println("Vermelho está aceso");
  digitalWrite(9, LOW);//VERDE 2
  Serial.println("Verde está apagado");
  digitalWrite(8, LOW);// AMARELO 2
  Serial.println("Amarelo está apagado");

  //PEDESTRE 1
  digitalWrite(7,HIGH);//VERMELHO p/1
  Serial.println("Pedestre 1:");
  Serial.println("Vermelho está aceso");
  digitalWrite(6,LOW);// verde P/1

  //PEDESTRE 2
  Serial.println("Verde está apagado");
  digitalWrite(5,LOW);//VERMELHO P/2
  Serial.println("Pedestre 2:");
  Serial.println("Vermelho está apagado");
  digitalWrite(4,HIGH);//VERDE P/2
  Serial.println("Verde está aceso");
  
  delay(1500); // Wait for 1000 millisecond(s)
  
} else {
      //SEMAFORO 1
  digitalWrite(13,HIGH);//VERMELHO 1
  digitalWrite(12, HIGH);//VERDE 1
  digitalWrite(11, HIGH);// AMARELO 1
  
  //SEMAFORO 2
  digitalWrite(10,HIGH);//VERMELHO 2
  digitalWrite(9, HIGH);//VERDE 2
  digitalWrite(8, HIGH);// AMARELO 2

  //pedestre 1
  digitalWrite(7,HIGH);//VERMELHO p/1
  digitalWrite(6,HIGH);// verde P/1

  //PEDESTRE 2
  digitalWrite(5,HIGH);//VERMELHO P/2
  digitalWrite(4,HIGH);//VERDE P/2 

  
  delay(1500); // Wait for 1000 millisecond(s)
  
  //SEMAFORO 1
  digitalWrite(13, LOW);//VERMELHO 1
  digitalWrite(12, LOW);//VERDE 1
  digitalWrite(11, LOW);//AMARELO 1

  //SEMAFORO 2
  digitalWrite(10,LOW);//VERMELHO 2
  digitalWrite(9, LOW);//VERDE 2
  digitalWrite(8, LOW);// AMARELO 2

  // PEDESTRE 1
  digitalWrite(7,LOW);//VERMELHO p/1
  digitalWrite(6,LOW);// verde P/1

  //PEDESTRE 2
  digitalWrite(5,LOW);//VERMELHO P/2
  digitalWrite(4,LOW);//VERDE P/2 

  delay(1500);
  }
}
