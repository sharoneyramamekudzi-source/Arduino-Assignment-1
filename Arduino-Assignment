int startValue = 5;
int ledPin = 13;

// Function to blink the LED
void flashLED(int times) {
  int i = 0;

  while (i < times) {
    digitalWrite(ledPin, HIGH);
    delay(300);

    digitalWrite(ledPin, LOW);
    delay(300);

    i++;
  }
}

void setup() {
  pinMode(ledPin, OUTPUT);

  Serial.begin(9600);

  Serial.println("=== Smart Countdown Starting ===");

  int currentCount = startValue;

  while (currentCount >= 1) {
    Serial.print("Count: ");
    Serial.println(currentCount);

    flashLED(currentCount);

    delay(1000);

    currentCount--;
  }

  Serial.println("=== Countdown Complete ===");
}

void loop() {
}
