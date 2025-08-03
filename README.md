# ASCII Digital Countdown Timer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A simple, elegant, and feature-rich countdown timer for your terminal. It displays the remaining time in a large, solid ASCII digital clock format, providing a clear visual indicator for any task. Written in pure Bash.


![timer](https://i.imgur.com/Cm9vAQG.png)

---

## Features

* **Customizable Color:** Easily change the timer's color using ANSI escape codes within the script.
* **Flexible Duration Input:** Set timers in hours (`h`), minutes (`m`), or seconds (`s`).
* **Custom Messages:** Add a custom message to your timer for context (e.g., `mytimer 10m "coffee process"`).
* **Desktop & Audible Alerts:** Get a system notification and terminal beeps when the timer finishes.
* **Portable:** No complex dependencies. Just a standard Bash environment.

---

## 🛠️ Requirements

* **Bash:** A modern version of Bash (standard on most Linux distros and macOS).
* **(Optional) `notify-send`:** For desktop notifications to work. On Debian/Ubuntu-based systems, you can install it with:
    ```bash
    sudo apt update && sudo apt install libnotify-bin
    ```

---

## Installation

Make the script a global command so you can call it from anywhere in your terminal.

1.  **Make the script executable:**
    ```bash
    chmod +x timer.sh
    ```

2.  **Move it to a directory in your PATH:**
    The recommended location is `/usr/local/bin`. We'll also rename it to just `mytimer` to make it feel like a native command.
    ```bash
    sudo mv timer.sh /usr/local/bin/mytimer
    ```

---

## Usage

**Syntax:**
timer <duration> [custom_message]


**Examples:**

* **Set a 30-second timer:**
    ```bash
    timer 30s
    ```

* **Set a 5-minute timer with a custom message:**
    ```bash
    timer 5m "Take a break"
    ```

* **Set a 1-hour timer for a specific task:**
    ```bash
    timer 1h "Compile the project"
    ```

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

