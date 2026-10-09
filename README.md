## 🛠 Hardware Requirements

To build the **LAKP Paper Analyzer**, you will need the following components:

* **Microcontroller:** ESP32-CAM module
* **Display:** 0.96" OLED Display (I2C, SSD1306)
* **Trigger Buttons:** 2x Tactile Push Buttons (6x6 mm) — for `RUN` and `TEST` functions
* **Power Source:** 18650 Li-ion Battery with holder
* **Lighting:** White LED for illumination
* **Wiring:** Dupont jumper wires (Female-to-Female / Female-to-Male)

---

### 🔌 Button Wiring Connection

Connect the tactile push buttons directly to the ESP32-CAM GPIO pins. No external pull-up resistors are required as internal `INPUT_PULLUP` is enabled in software.

| Button | ESP32-CAM Pin | Ground Pin |
| :--- | :--- | :--- |
| **RUN** | `GPIO 12` *(or your configured pin)* | `GND` |
| **TEST** | `GPIO 13` *(or your configured pin)* | `GND` |
