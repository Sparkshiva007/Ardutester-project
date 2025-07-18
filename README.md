# ArduTester (Modified for Function Generator Use)

This is a modified version of the popular DIY ArduTester project. Originally developed to test electronic components using an Arduino, this version has been reworked to serve primarily as a **basic function generator**.

---

## 🎯 Purpose

While the original ArduTester could test resistors, capacitors, transistors, and more, this modified version is **focused on waveform generation**, making it useful for:

- Injecting test signals into amplifier or filter circuits
- Educational demonstrations for waveforms
- Simple signal analysis and experimentation

---

## ⚙️ Features

- Generates basic **square** and **triangle** waveforms
- Selectable **frequency ranges** (via code or button)
- Output available on a designated pin (D9 or D10)
- Compatible with Arduino Nano / Uno
- Can be powered via USB or battery
- Display shows current waveform type and frequency

---

## 🔌 Hardware Requirements

- **Arduino Uno**
- Use only aurdino UNO and not aurdino Nano (Ardutester code requires 32kb storage which is available only in UNO)
- If you are fixed with nano, then flash the UNO's Boot loader on the Nano and convert it into UNO.
- **16x2 LCD** (optional for UI feedback)
- **Push button(s)** for waveform/frequency selection (optional)
- **Output pin** wired to oscilloscope, speaker, or test circuit

---

## 🛠️ Notes

- The waveform generation uses `analogWrite()` for square waves and timer-based DAC simulation for triangle waves.
- The output voltage and frequency are limited by the Arduino's capabilities.
- You can extend this project to support sine waves using external DACs or PWM filtering.

---

## 💡 Future Ideas

- Add rotary encoder for fine control
- Add frequency display on LCD
- Expand waveform types using external DAC (MCP4725)
- 3D printable enclosure for clean look

---

## Credits

The original ArduTester project was developed by **Karl-Heinz Kübbeler** and contributors. This modified version is developed by **Shiva Projects**, adapted for use as a basic function generator for educational and experimental use.

---

## 📄 License

Open-source under the same license as the original ArduTester. You are free to modify and distribute, but please credit the original developers and this project if reused.

