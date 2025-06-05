# door-lock-with-Huskylens
🧠🔒 HuskyLens Face Recognition Door Lock with Arduino
A smart and secure door lock system using the HuskyLens AI Camera and Arduino. This project uses real-time face recognition to grant access, making your door smarter and safer.

📸 Features
Face recognition using HuskyLens

Access control via servo motor

Easy face training and management on HuskyLens

Integration with Arduino for real-world hardware control

Optional buzzer for feedback

🧰 Hardware Requirements
HuskyLens AI Camera

Arduino Uno (or any compatible Arduino board)

Servo motor (SG90 or similar)

Breadboard & jumper wires

5V power supply (or battery pack)

Buzzer (optional)

Door lock or latch mechanism

🧠 How It Works
Face Training: Use the onboard buttons on the HuskyLens to train and label known faces.

Recognition Loop: Arduino constantly reads data from HuskyLens via UART/I2C.

Face Match: If a recognized face ID is detected, the servo rotates to unlock the door.

Timeout Auto-Lock: After a delay, the door automatically locks again.

🔌 Wiring Diagram
Component	Arduino Pin
HuskyLens TX	RX (Pin 0)
HuskyLens RX	TX (Pin 1)
Servo Signal	Pin 9
Buzzer (+)	Pin 8 (Optional)
Ground/Power	GND/5V

⚠️ If you're using Serial for debugging, consider using SoftwareSerial or I2C to avoid conflict with HuskyLens.

📦 Installation & Setup
Connect all components according to the wiring diagram.

Train your face on the HuskyLens (Face Recognition mode > long-press the "learning" button).

Upload the Arduino code provided in the code/ folder.

Power up your system and test face recognition.

✅ Tips
Use I2C mode for better serial management if your board supports it.

Mount the HuskyLens in a fixed position for consistent detection.

Adjust the servo angle to match your locking mechanism.

![IMG_20250529_183928](https://github.com/user-attachments/assets/5e02d4c5-19df-4b80-b7a7-15f7616b2745)
![IMG_20250529_183939](https://github.com/user-attachments/assets/e7bd9c31-02b1-48a0-8bb3-8a06ee414198)
![IMG_20250529_183933](https://github.com/user-attachments/assets/2f4ce39e-24cf-472a-9dce-6951035c2e53)

