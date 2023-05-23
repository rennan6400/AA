const byte led = 12;
const byte potenciomentro = A1;
unsigned int valorPot;
void setup()
{
  pinMode(led, OUTPUT);
  pinMode(potenciomentro, INPUT);
}

void loop()
{
  valorPot = analogRead(potenciomentro);
  digitalWrite(led, HIGH);
  delay(valorPot); 
  digitalWrite(led, LOW);
  delay(valorPot);
}
