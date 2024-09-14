# Schematic and PCB design for an ESP32-based smart pen circuit. 

The circuit uses an LM358 op-amp to amplify signals from a microphone and includes battery charging capabilities using the TP4057 charger IC.

ESP32-D0WD: The main microcontroller chip used for processing and wireless communication.


AP2112K-3.3: A 3.3V linear voltage regulator providing stable power to the ESP32.


TP4057: A lithium-ion battery charger IC for charging a 3.7V LiPo battery.


LM358: Operational amplifier used to amplify the microphone signal.


Microphone: Used to capture audio input from the user.


The gain of the op-amp can be adjusted using the potentiometer.


MPU-6050: Gyroscope and Accelerometer to track the movement and orientation of the smart pen. It uses the I2C protocol to communicate with the ESP32.


Vibration Motor: Powered by the 3.3V supply and is controlled by the ESP32 using a GPIO pin with a MOSFET circuit (n-channel) to drive the motor when needed.


The USB Type-C port is used to charge the 3.7V LiPo battery via the TP4057 charger IC. 


This basic circuit aims at taking input using microphone(on the body of smart pen) from the user and processing it to the ESP 32 which has bluetooth module used to send the speech to text code to the smart board connected.
