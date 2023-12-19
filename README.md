int sensorPin = A0; // select the input pin for LDR

int sensorValue = 0; // variable to store the value coming from the sensor
void setup() {
  Serial.begin(9600); //sets serial port for communication
   // while the serial stream is not open, do nothing:
while (!Serial)
{
    // do nothing
}
Serial.println("I am in setup");
    
  // put your setup code here, to run once:
//pinMode(8,OUTPUT);
}
void loop() {
  // put your main code here, to run repeatedly:
/*digitalWrite(8,HIGH);
delay(3000);
digitalWrite(8,LOW);
delay(1000);
*/
sensorValue = analogRead(sensorPin); // read the value from the sensor
Serial.println(sensorValue); //prints the values coming from the sensor on the screen

delay(1000);
}
