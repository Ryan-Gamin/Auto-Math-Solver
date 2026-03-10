# 🧮 Auto Math Solver (Hardware Edition)

![Python Version](https://img.shields.io/badge/Python-3.10%2B-blue)
![OS](https://img.shields.io/badge/OS-Linux%20(evdev)-orange)
![Browser](https://img.shields.io/badge/Browser-Chrome%20Extension-green)
![AI](https://img.shields.io/badge/AI-Gemini%202.5%20Pro-purple)

A fully autonomous, OS-level math homework solver. Built to bypass aggressive anti-bot protections (like Microsoft SSO and strict React event listeners) by operating as a **virtual hardware keyboard**. 

Instead of fighting web frameworks with JavaScript, this bot drops down to the Linux kernel using `evdev`, taking screenshots via a Chrome extension and physically injecting the AI's keystrokes back into the OS. To the browser, it looks exactly like a human typing on a plastic keyboard.

---

## ✨ Current Features
* **Hardware-Level Evasion:** Bypasses DOM-based bot detection by injecting raw keycodes directly into the Linux kernel.
* **Smart State Machine:** Autonomously detects if a page is "unanswered", "correct", or "incorrect" and reacts accordingly.
* **Auto-Correction & Escalation:** Defaults to high-speed models (Gemini Flash) but automatically escalates to Gemini 2.5 Pro if it gets a question wrong.
* **Hybrid Architecture:** Uses a Python Flask backend for heavy AI lifting and a lightweight Chrome Extension for screen capture and element targeting.
* **Human Takeover Mode:** Instantly pause the bot with a GUI button to manually solve a question if the AI gets stuck.

---

## 🚀 Roadmap / To-Do List

> **⚠️ Release Notice:** Version 1.0 (V1) will not be officially released until every item on the V1 Checklist is 100% complete. 

### 🟢 V1 Checklist
- [ ] **Multiple Box Support:** Logic to handle complex algebra questions that require tabbing between multiple input fields (e.g., fractions, coordinates).
- [ ] **Backup Model Chooser:** Automatically failover to alternative APIs (like Claude or OpenAI) if the primary Gemini API goes down or hits rate limits.
- [ ] **Smarter AI:** Improved prompting and vision-context interpretation to handle multi-part questions and complex spatial screen layouts seamlessly.

### <img src="https://github.com/user-attachments/assets/2c45494e-b934-4d68-a608-fcfe8efca386" height="24" style="vertical-align: middle;" alt="V1 Plus"> Future Features
- [ ] **AIO Install Script:** A single-command bash script to automatically install dependencies, configure `xhost`, set up `evdev` rules, and pack the Chrome extension.
- [ ] **Humanized Typing Cadence:** Add randomized, per-character milliseconds delays and occasional "typo-then-backspace" logic to defeat behavioral biometrics.
- [ ] **Interactive Graphing Support:** Enable the AI to click and drag points on interactive coordinate plane questions.
- [ ] **Cross-Platform Presets:** Pre-configured rule sets tailored for specific platforms (Sparx Maths, DrFrostMaths, Hegarty, etc.) to optimize answer formatting.
- [ ] **Local OCR Pre-processing:** Run lightweight local OCR on the screenshots to extract text before sending to the LLM, reducing token costs and improving accuracy.
- [ ] **Headless VM Support:** Allow the entire bot (browser and virtual keyboard) to run completely invisibly inside a Docker container with a virtual display buffer (Xvfb).

---

*(Installation and Usage instructions coming soon!)*

---

## ⚠️ Disclaimer

This project is created for educational purposes, specifically to demonstrate OS-level hardware emulation, computer vision, and state-machine automation. The creators do not endorse academic dishonesty. Use responsibly and abide by your institution's terms of service.
