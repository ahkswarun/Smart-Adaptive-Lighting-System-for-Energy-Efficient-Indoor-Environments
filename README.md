The Smart Lighting System operates through a layered sensing mechanism to ensure efficient lighting control based on occupancy and ambient conditions.

1. Motion Detection with PIR Sensor
The PIR sensor acts as the first trigger. Positioned strategically, it senses motion by detecting changes in infrared radiation when a person enters or moves within the room. Upon detecting motion, it activates the system to evaluate further conditions, avoiding unnecessary LED activation if no one is present.

2. Occupancy Confirmation with IR and Ultrasonic Sensors
After the PIR sensor detects motion, the system uses both the active IR and ultrasonic sensors to confirm actual occupancy.

The IR sensor detects the presence of stationary or slow-moving individuals by sensing reflected infrared light.

The Ultrasonic sensor emits sound waves and measures their reflection time to detect objects within a specific range.
If both sensors confirm occupancy, the system concludes that someone is present, even if they are not moving significantly.

3. Ambient Light Detection with LDR
The LDR continuously measures the ambient light in the room. Its readings are processed by the Arduino to determine whether artificial lighting is necessary.

If sufficient natural light is present (e.g., during the day), the system dims or turns off the LED.

If ambient light is low (e.g., evening or cloudy conditions), the system prepares to increase LED brightness for adequate illumination.

4. Light Intensity Control with Digital Potentiometer
Based on LDR readings, the Arduino adjusts the digital potentiometer to regulate the brightness of the LED.

Lower ambient light results in decreased resistance, allowing more current and increasing LED brightness.

Higher ambient light causes increased resistance, dimming or switching off the LED.
This provides smooth, precise brightness control rather than abrupt changes.

5. Adaptive LED Illumination
The LED serves as the system’s light source. Its brightness is dynamically managed based on the occupancy status and light levels.

When the room is occupied and ambient light is low, the LED brightens to ensure visibility.

If the room is empty or naturally well-lit, the LED dims or turns off, conserving energy.

This coordinated sensor-based approach enables the Smart Lighting System to maintain optimal lighting comfort while maximizing energy efficiency.
