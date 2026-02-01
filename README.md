# embedded-esp32

> Summary: This repository contains a collection of Rust-based ESP32 embedded examples covering LEDs, servos, sensors, displays, WiFi, RFID, storage, and other common peripherals and features. Each example is organized in its own `mXX_*` directory and includes its own `Cargo.toml`, `build.rs`, and `rust-toolchain.toml`.

---

## 🚀 Overview
**embedded-esp32** is a set of ESP32 embedded Rust example projects intended for learning and demonstration. It's suitable for developers who want to explore or prototype with Rust. Examples are concise and can be built and run independently.

## 🔧 Highlights
- Each example is placed in a separate directory (format `mNN_name`) and can be built and flashed independently ✅
- Wide coverage: LEDs, PWM/servos, buzzers, ultrasonic/IR sensors, OLED/TFT/EPaper displays, WiFi (STA/AP/Web), BLE, RFID, SD card, etc. 🔌
- Each example contains necessary toolchain configuration (`rust-toolchain.toml`) for reproducibility and easy switching 🔁

## 📁 Structure
The root directory contains multiple example folders, for example:
- `m1_led_in`, `m2_fading_led_in`, `m3_fading_led_out`: LED demos
- `m10_servo_motor`, `m11_servo_motor_mcpwm`: servo / PWM
- `m13_wifi_sta`, `m15_wifi_web`, `m18_wifi_ap`: WiFi client/server/web demos
- `m22_oled_text`, `m23_oled_sig_image`, `m24_oled_mul_image`: OLED displays
- `m28_rfid_uid`, `m29_rfid_read_data`: RFID operations
- Others: sensors (temperature, LDR, ultrasonic), displays, SD card, E-Paper, BLE, etc.

> Note: Each subdirectory usually contains more detailed example instructions and build/flash steps. Please read the subdirectory README or comments first.

## ⚙️ Quick start
1. Install Rust and required tools: `rustup`, `cargo`, and make sure you can use or switch to the toolchain specified by the example directory (`rust-toolchain.toml`).
2. Enter an example directory:
   ```bash
   cd m15_wifi_web
   ```
3. Read that example's instructions and install external tools as needed (e.g., `cargo-espflash`, `esptool.py`, `probe-run`).
4. Build:
   ```bash
   cargo build --release
   ```
   cargo run --release

