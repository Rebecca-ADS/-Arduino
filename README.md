# -Arduino
// Define os pinos
int pinoBotao = 2;
int pinoLed = 13;
int estadoBotao = 0;

void setup() {
  pinMode(pinoLed, OUTPUT);
  pinMode(pinoBotao, INPUT);
}

void loop() {
  estadoBotao = digitalRead(pinoBotao);

  if (estadoBotao == HIGH) {
    digitalWrite(pinoLed, HIGH);
  } else {
    digitalWrite(pinoLed, LOW);
  }
}

