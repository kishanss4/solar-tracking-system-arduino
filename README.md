# 🌞 Dual Axis Solar Tracking System

A **Dual Axis Solar Tracker** that uses an Arduino, two servo motors, and four LDRs (Light Dependent Resistors) to maximize the solar panel’s exposure to sunlight.  
This system automatically adjusts the solar panel in **both horizontal and vertical directions** to follow the sun’s position throughout the day.

---

## 📌 Features
- Tracks sunlight in **two axes (horizontal & vertical)**.
- Uses **4 LDRs** for precise light detection.
- Moves the solar panel using **two servo motors**.
- Enhances solar panel efficiency compared to a fixed setup.
- Compact and easy-to-build design.

---

## 🛠 Components Required
- **Arduino UNO / Nano / Mega**  
- **Solar Panel** (mounted on tracking frame)  
- **2x Servo Motors** (horizontal + vertical rotation)  
- **4x LDRs (Light Dependent Resistors)**  
- **4x 10kΩ Resistors** (voltage dividers for LDRs)  
- **Breadboard / PCB**  
- **Connecting Wires**  
- **Mounting Frame** (to hold panel + servos)

---

## ⚡ Circuit Connections

| Component         | Arduino Pin  |
|-------------------|--------------|
| Horizontal Servo  | Pin **10**   |
| Vertical Servo    | Pin **9**    |
| LDR (Top Right)   | **A1**       |
| LDR (Top Left)    | **A2**       |
| LDR (Bottom Right)| **A0**       |
| LDR (Bottom Left) | **A3**       |

🔹 Each LDR must be connected in a **voltage divider** with a **10kΩ resistor** before connecting to the Arduino’s analog pins.  
🔹 Servos are powered from Arduino, but for stability, use an **external 5V supply** if needed.

---

## ⚙️ Working Principle
1. The **LDRs** continuously sense the light intensity in four directions (top-left, top-right, bottom-left, bottom-right).  
2. The system calculates the **average intensity** of top vs. bottom and left vs. right.  
3. Depending on the comparison, the **vertical servo** adjusts the tilt and the **horizontal servo** adjusts the rotation.  
4. This ensures the solar panel always faces the direction with maximum sunlight.  

---

## 🚀 Setup & Usage
1. Assemble the **solar panel frame** with two servo motors for horizontal and vertical movement.  
2. Place the **4 LDRs** at the panel corners (top-left, top-right, bottom-left, bottom-right).  
3. Wire up the circuit as per the table above.  
4. Upload the Arduino sketch to the board.  
5. Power on the system — the panel will automatically align with sunlight.  

---

## 📈 Applications
- Solar energy systems for **maximizing power generation**.  
- Research and educational projects.  
- Renewable energy demonstrations.  
- IoT-based smart solar systems (with upgrades).  

---

## 🔮 Future Enhancements
- Add a **real-time clock (RTC)** for night reset position.  
- Use **MPPT (Maximum Power Point Tracking)** with sensors for higher efficiency.  
- Integrate **IoT monitoring** for remote performance tracking.  
- Upgrade to **stepper motors** for more precise movement.  

---

## 📷 Project Preview
(*Insert images or diagrams of your circuit and assembled project here*)  

---

## 👨‍💻 Author
Developed by **[Your Name]**  
