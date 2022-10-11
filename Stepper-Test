/* Open Electronika NEMA 17 Stepper Motor Control Test
SGMA CNC
John Papagiannopoulos
v1.0.0 Development Build*/

// Imports
#include <Stepper.h> //L298N Motor Driver

const int STEPS_PER_REVOLUTION = 200; //360 degrees / 1.8 degree step angle (defined in data sheet)
Stepper stepTest (STEPS_PER_REVOLUTION, 4, 5, 6, 7); //Creates Stepper object corresponding to Step angle and 4 Digital board pinouts.

void setup() {
  // Testing different speeds
  Serial.println("10 rpm");
  stepTest.setSpeed(10); // 10 rpm
  delay(1500);
  
  Serial.println("20 rpm");
  stepTest.setSpeed(20); // 20 rpm
  delay(1500);
  
  Serial.println("40 rpm");
  stepTest.setSpeed(40); // 40 rpm
  delay(1500);
  
  Serial.println("60 rpm");
  stepTest.setSpeed(60); // 60 rpm
  delay(1500);

  Serial.begin(9600); //Serial port initialization

}

void loop() {
  // Testing direction shifts
  stepTest.step(STEPS_PER_REVOLUTION); //Clockwise
	delay(1500);
	
  stepTest.step(-STEPS_PER_REVOLUTION); //Counterclockwise (-) sign
	delay(1500);

}
