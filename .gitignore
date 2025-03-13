// Pin Definitions
const int ldrPin = A0; // LDR connected to analog pin A0
const int ledPin = 9;  // LED connected to digital pin 9

// Threshold for light detection
const int lightThreshold = 500; // Adjust based on your environment

void setup() {
  pinMode(ledPin, OUTPUT);
  Serial.begin(9600); // Start serial monitor
}

void loop() {
  // Read LDR value
  int ldrValue = analogRead(ldrPin);
  Serial.print("LDR Value: ");
  Serial.println(ldrValue);

  // Light detection logic
  if (ldrValue > lightThreshold) {
    digitalWrite(ledPin, HIGH); // Turn LED ON if it's bright
  } else {
    digitalWrite(ledPin, LOW);  // Turn LED OFF if it's dark
  }

  delay(500); // Delay for stability
} 
