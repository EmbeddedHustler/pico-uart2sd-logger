# pico-uart2sd-logger

A UART-to-SD card data logger using the Raspberry Pi Pico and C++ SDK.  
Ideal for field debugging where a PC is not available.

---

## 🔧 Features

- Uses Pico SDK (C++)
- Receives data via UART
- Saves serial input to SD card (CSV or raw log format)
- Timestamping with millis (optional)
- Ideal for logging sensor, debug, or Modbus data in the field

---

## 📦 Hardware Requirements

| Component            | Quantity |
|----------------------|----------|
| Raspberry Pi Pico    | 1        |
| MicroSD Card Module  | 1        |
| SD Card (FAT32)      | 1        |
| Jumper Wires         | As needed |

---

## 🔌 Wiring

| Pico Pin | Module Pin |
|----------|------------|
| GP0      | UART RX    |
| GP1      | UART TX    |
| GP5      | CS         |
| GP6      | MOSI       |
| GP7      | MISO       |
| GP10     | SCK        |
| 3.3V     | VCC        |
| GND      | GND        |

---

## 🚀 Getting Started

1. Clone this repo
2. Build using `cmake` and `make` (Pico SDK setup required)
3. Flash the `.uf2` to your Pico
4. Connect UART source and insert SD card
5. Data will be saved to `/log.txt`

---

## 📂 Folder Structure

pico-uart2sd-logger/<br>
├── src/<br>
│ └── main.cpp<br>
├── CMakeLists.txt<br>
├── README.md<br>
