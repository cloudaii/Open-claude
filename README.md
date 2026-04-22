# Open-claude

# OpenClaude Android (Ollama Edition)

**Run an autonomous, hardware-aware AI agent directly on your Android device. This version is modified to run locally via Ollama with full "God-Mode" hardware control.**

# Features

• **Local LLM Support:** Run high-performance models locally using Ollama.

• **Autonomous UI Control:** The AI can "see" your screen and simulate taps, swipes, and typing using Shizuku and UIAutomator.

• **Hardware Integration:** Control WiFi, Battery, Camera, and Volume directly through the AI chat.

• **1-Click Setup:** Fully automated Termux environment configuration.

# Prerequisites

To use the "God-Mode" hardware features, you must have the following installed:

Termux (GitHub/F-Droid version): Do not use the Play Store version.Termux on F-Droid

Termux:API: Install the app from GitHub to allow the AI to access hardware sensors. Termux API on F-Droid

Ollama: Must be installed (pkg install ollama) and running (ollama serve) in a separate Termux tab.

Shizuku (Optional but Recommended): Required for autonomous UI interaction without root.

# Shizuku Configuration (System Control)

Shizuku is required to securely bypass the internal Android application sandbox. Without this service, your AI will not have the native authority to execute system commands.

1. Install **Shizuku** from the Google Play Store.

2. Enable **Developer Options** on your Android device (tap "Build Number" 7 times under Settings > About Phone).

3. Inside Developer Options, enable **Wireless Debugging**.

4. Open the Shizuku application, select **Pairing**, and follow the on-screen instructions to authorize the service using an Android pairing code.

5. Tap **Start** to initiate the background service.

# Ollama Installation

Open Termux and paste the following command. This will install and run the ollama on your phone

```termux-setup-storage
pkg install ollama
ollama serve
```
# One-Line Installation 

Open Termux and paste the following command. This will update your system, download the setup script, and configure everything automatically:

```
pkg update -y && pkg upgrade -y && pkg install curl -y && curl -sL https://raw.githubusercontent.com/AbuZar-Ansarii/Leaked-ClaudeCode/master/termux_setup.sh -o ~/termux_setup.sh && chmod +x ~/termux_setup.sh && bash ~/termux_setup.sh
```
# use Claude

```
claude
```

# Disclaimer

This project is for educational and research purposes only. Use "Limitless Mode" with caution as it allows the AI to execute commands on your device autonomously.
