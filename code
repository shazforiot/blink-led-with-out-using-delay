
int ledState = LOW;
unsigned long previousMillis = 0;

void setup()
{
  pinMode(12, OUTPUT);
  Serial.begin(9600);
}

void loop()
{
  
  unsigned long currentMillis = millis();
  Serial.println(currentMillis);
  
  if ( currentMillis - previousMillis >= 500){
      previousMillis = currentMillis;
    
    if (ledState == LOW) {
      ledState = HIGH;
    } else {
      ledState = LOW;
    }
    
    digitalWrite(12, ledState);
  
  }
}
