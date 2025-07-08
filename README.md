
# 🚀 Stepper Motor Testing Code with Arduino UNO, CNC Shield + A4988

Welcome to the **Stepper Motor Testing Code** repository! This project provides tested and reliable Arduino code to control a **NEMA 17 Stepper Motor** using the **CNC Shield V3** paired with **A4988 stepper drivers** and **Arduino UNO**.

Whether you're building a CNC machine, 3D printer, or simply learning how stepper motors work—this code offers a clean and easy way to get started.

---

## 🔧 Features

* ✅ Compatible with **Arduino UNO + CNC Shield**
* ✅ Controls **NEMA 17 Stepper Motor**
* ✅ Uses **A4988 Driver Modules (via CNC Shield)**
* ✅ Simple and modular code
* ✅ Adjustable speed and direction
* ✅ Ideal for testing motor axes (X, Y, Z)

---

## 📁 Repository Contents

```bash
Stepper_testing_code/
│
├── x_axis_test.ino        # Test code for X-axis motor
├── y_axis_test.ino        # Test code for Y-axis motor
├── z_axis_test.ino        # Test code for Z-axis motor
├── multi_axis_test.ino    # Run X, Y, Z motors in sequence
└── README.md              # You're reading it!
```

---

## 🧰 Hardware Requirements

* 🧠 Arduino UNO
* 🧩 CNC Shield V3
* 📦 A4988 Stepper Driver Module(s)
* ⚙️ NEMA 17 Stepper Motor(s)
* 🔌 12V DC Power Supply (recommended)
* 🔗 Jumper caps for microstepping (optional)

---

## 🧠 How It Works

This project uses the **CNC Shield’s STEP and DIR pins** for X, Y, and Z axes:

| CNC Shield Axis | STEP Pin | DIR Pin |
| --------------- | -------- | ------- |
| X-Axis          | D2       | D5      |
| Y-Axis          | D3       | D6      |
| Z-Axis          | D4       | D7      |

The Arduino sends step pulses and direction signals to A4988 drivers, which control the NEMA 17 motors.

Each `.ino` file in this repo is designed to test a specific axis or run multiple axes in a loop for full setup testing.

---

## ⚙️ Microstepping Tips

To enable microstepping on the A4988 via the CNC Shield, place jumper caps under the driver module on the **MS1, MS2, and MS3** pins:

* No jumpers = Full Step
* 1 jumper = Half Step
* 3 jumpers = 1/16 Step (Smoothest)

---

## 📷 Demo (Optional)

> *(You can add a short video or GIF showing the motor spinning when using X, Y, Z test sketches)*

---

## 👨‍💻 Author

Developed by [**Sunanda Dutta**](https://github.com/duttasunanda)
🎓 Diploma in CST | 💡 IoT & Robotics Enthusiast | 💻 Arduino & Web Developer

---

## 🛠️ License

This project is licensed under the **MIT License**.
Use, modify, share, and learn—freely!

