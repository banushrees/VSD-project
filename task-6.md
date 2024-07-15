# TASK -6

  ### WORKING OF SEQUENTIAL TRAFFIC LIGHT CONTROLLER USING VSD Squadron mini processor

   ### Project components:
    - Breadboard
    - VSD squadron mini board
    - LED lights 
    - Resistors
    - Connecting wires
    - Power supply (USB cable)

Circuit diagram:

  ![image](https://github.com/user-attachments/assets/06fffaab-4d5a-4c97-9aba-fa9361a03301)





   PIN CONNECTIONS:
   
    PIN PD1-  YELLOW LIGHT
    PIN PD2 - RED LIGHT
    PIN PD3 - RED LIGHT
    PIN PD4 - YELLOW LIGHT
    PIN PD6 - GREEN LIGHT 
    PIN PD7 - GREEN LIGHT 
    PIN GND - GROUND

   ### WORKING CONDITIONS:
   
- North-South Green Light:

North-South direction has green light (vehicles proceed).
East-West direction has red light (vehicles stop).
Duration: 60 seconds.

- North-South Yellow Light:

North-South direction changes to yellow light (prepare to stop).
East-West direction remains red.
Duration: 5 seconds.

- North-South Red Light:

North-South direction changes to red light (vehicles stop).
East-West direction remains red (brief all-red phase for safety).
Duration: 2 seconds.

- East-West Green Light:

East-West direction changes to green light (vehicles proceed).
North-South direction remains red.
Duration: 60 seconds.

- East-West Yellow Light:

East-West direction changes to yellow light (prepare to stop).
North-South direction remains red.
Duration: 5 seconds.

- East-West Red Light:

East-West direction changes to red light (vehicles stop).
North-South direction remains red (brief all-red phase for safety).
Duration: 2 seconds.

### Pedestrian Signals:

- North-South Green Light:
  
  Pedestrian signal allows crossing E-W.

- East-West Green Light:

 Pedestrian signal allows crossing N-S.
 
- Sensor Integration (if equipped):

- Vehicle Detection:

   Sensors adjust green light duration based on traffic volume.

- Pedestrian Buttons:
  
    Allow pedestrians to request crossing, extending green light duration if needed.

 - Emergency Vehicles:

   Sensor detects emergency vehicle, overrides normal sequence to give green light to the direction of the emergency vehicle.
 - All-Red Flash:
   
    Activates in emergencies or malfunction for safety.

 - Maintenance and Monitoring:

Regularly check lights and controller for proper operation.
Monitor system for real-time malfunctions and address promptly.

- Backup Power:
Ensure uninterrupted operation during power outages with backup power supply.

 Manual Override:
Manual control by operators during special events or maintenance work.

- Sequence Directon timing example:
```
N-S Green, E-W Red (60 seconds)
N-S Yellow, E-W Red (5 seconds)
N-S Red, E-W Red (2 seconds)
E-W Green, N-S Red (60 seconds)
E-W Yellow, N-S Red (5 seconds)
E-W Red, N-S Red (2 seconds)
```
##  C CODE:

```bash
 #include <stdio.h>
#include <unistd.h>  // For sleep function

// Define the light durations in seconds
#define GREEN_DURATION 60
#define YELLOW_DURATION 5
#define RED_DURATION 2

// Function prototypes
void northSouthGreen();
void northSouthYellow();
void northSouthRed();
void eastWestGreen();
void eastWestYellow();
void eastWestRed();

int main() {
    while (1) {
        // North-South direction green light sequence
        northSouthGreen();
        northSouthYellow();
        northSouthRed();

        // East-West direction green light sequence
        eastWestGreen();
        eastWestYellow();
        eastWestRed();
    }

    return 0;
}

void northSouthGreen() {
    printf("North-South Green, East-West Red\n");
    sleep(GREEN_DURATION);
}

void northSouthYellow() {
    printf("North-South Yellow, East-West Red\n");
    sleep(YELLOW_DURATION);
}

void northSouthRed() {
    printf("North-South Red, East-West Red\n");
    sleep(RED_DURATION);
}

void eastWestGreen() {
    printf("East-West Green, North-South Red\n");
    sleep(GREEN_DURATION);
}

void eastWestYellow() {
    printf("East-West Yellow, North-South Red\n");
    sleep(YELLOW_DURATION);
}

void eastWestRed() {
    printf("East-West Red, North-South Red\n");
    sleep(RED_DURATION);
}
```
WORKING VIDEO:

https://github.com/user-attachments/assets/a249638d-d0ed-4adb-a628-3aa4288736e9









   


    
