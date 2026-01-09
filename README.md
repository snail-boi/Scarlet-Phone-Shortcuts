# Phone App Shortcut Creator

## Overview

**Phone App Shortcut Creator** is a tool for creating seamless shortcuts to Android apps on Windows. It allows you to connect your phone via USB with USB debugging enabled, select an app from the list, and create a shortcut that seemingly opens the app on Windows.

### How It Works

1. **Connect Your Phone**: Connect your Android phone to the PC via USB with USB debugging enabled.
2. **Select an App**: Choose an app from the list of installed apps.
3. **App Icon Extraction**: The tool will attempt to collect the app's icon (Note: The icon may not always be 100% accurate due to limitations).
4. **Shortcut Creation**: It generates a shortcut that runs the modified `scrcpy-noconsole.vbs` script with the required arguments to launch the app.
5. **Seamless Experience**: This process creates a nearly seamless experience where the app is launched in a virtual window on your desktop.

### Future Features

- **Integration with Vermilia Phone Utils**: This tool will eventually be integrated with my larger project, **Vermilia Phone Utils**, providing additional functionality.
- **Standalone Mode**: It will be capable of running standalone, though it is currently dependent on resources from **Phone Utils**.
- **An installer**

### Known Issues

- **DeX Environment on Samsung Phones**: Samsung devices with DeX enabled may attempt to output the virtual display in a DeX-like environment. Unfortunately, I haven’t found a solution for this yet.
- **Icon Accuracy**: The tool attempts to collect the app icon but can't guarantee full accuracy. The current approach relies on minimal dependencies, so including tools like `AAPT` just for icon extraction seems excessive.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/phone-app-shortcut-creator.git
    ```

2. Ensure you have Phone Utils installed. The program currently relies on the tools provided by it for interacting with your device and displaying the app.


## Usage

1. Launch the application.
2. Connect your Android phone via USB with USB debugging enabled.
3. Select an app from the list of installed apps.
4. Choose whether to include audio or not.
5. The tool will generate a shortcut for the selected app, and you can launch the app in a virtual display on your Windows machine.

## Troubleshooting

- **DeX Mode**: If your Samsung device switches to DeX mode, try disabling DeX on the phone or use an alternative device.
- **Icon Extraction**: Icons may not always be fully accurate. If you need more reliable icon extraction, consider using tools with additional dependencies like `AAPT`.

---

**Disclaimer**: This tool is a work in progress and may contain bugs. It is currently dependent on resources from the **Vermilia Phone Utils** project and may require updates for future compatibility.
