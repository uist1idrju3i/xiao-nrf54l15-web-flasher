# study-DAP.js

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/uist1idrju3i/study-dapjs)

A browser-based factory reset and recovery tool for Seeed XIAO nRF54L15. Using WebUSB and CMSIS-DAP, you can recover devices and flash firmware directly from your browser without any installation.

## Disclaimer

This is an **unofficial tool** and is not affiliated with, endorsed by, or supported by Seeed Studio, Nordic Semiconductor, or OpenBlink.org. This tool is provided "AS IS" without warranty of any kind. Use of this tool is entirely **at your own risk**. The author(s) are not responsible for any damage to your device, data loss, or any other issues that may arise from using this tool.

## Features

- **Recover Only**: Performs a mass erase via CTRL-AP to unlock protected devices
- **Factory Reset**: Performs a mass erase followed by flashing the factory firmware (firmware.hex) to restore the device to its original state
- **OpenBlink XIAO nRF54L15 Firmware Flash**: Performs a mass erase followed by flashing the [OpenBlink firmware](https://github.com/uist1idrju3i/openblink_XIAO_nRF54L15_Sense)

## Verified Environment

- MacBook Pro (Apple M3)
- macOS 26.2
- Google Chrome 143.0.7499.170 (Official Build) (arm64)

## How to Use

1. Start a local HTTP server in the project directory:
   ```console
   $ python3 -m http.server 8000
   ```
2. Open `http://localhost:8000/index.html` in Chrome or Edge browser
3. Accept the disclaimer
4. Click the button for the operation you want to perform
5. Select Seeed XIAO nRF54L15 from the WebUSB device picker
6. Wait for the operation to complete

## How to Get

To clone the repository and initialize the submodules, run the following commands:

```console
$ git clone https://github.com/uist1idrju3i/study-dapjs.git
$ git submodule init
$ git submodule update
```

## License

This project is licensed under the BSD 3-Clause License.

Libraries used:
- [DAP.js](https://github.com/ARMmbed/dapjs) - MIT License
- [platform-seeedboards](https://github.com/Seeed-Studio/platform-seeedboards/) - Apache License 2.0 (configuration reference)

## Recommended VS Code Extensions

- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
