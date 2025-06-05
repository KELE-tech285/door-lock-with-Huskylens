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

![1000001723](https://github.com/user-attachments/assets/d5c54161-596f-4925-a6c5-d31c1127c693)
![1000001727](https://github.com/user-attachments/assets/d1af9127-a1d3-48d3-9cad-cc276d0d0a42)
![1000001726](https://github.com/user-attachments/assets/1fb22020-4b6a-4203-a177-134710c2ecbb)
![1000001725](https://github.com/user-attachments/assets/96c95ae8-8240-4920-b052-6a6d67f49afa)
![1000001724](https://github.com/user-attachments/assets/27a1a0a9-5b36-44ad-bc0f-33f28a1c3904)
