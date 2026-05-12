# studious-OGB
// C++ code
//
int led=13;
void setup()
{
  pinMode(led, OUTPUT);
}

void loop()
{
  digitalWrite(LED_BUILTIN, HIGH);
  delay(2000); // LED ON for 2 second(s)
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // LED OFF for 1 second
}
