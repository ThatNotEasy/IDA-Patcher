# IDA Pro Patcher & License Generator

![Python](https://img.shields.io/badge/python-3.7+-blue.svg)
![Platform](https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-lightgrey.svg)

A Python utility that automates patching IDA Pro binaries and generating valid license files. This tool supports the IDA Pro 9.1 version and can be run on Windows, Linux, and macOS.

## Features

- 🛠️ **Binary Patching**: Automatically patches IDA's core binaries to bypass cryptographic checks.
- 🔑 **License Generation**: Creates a valid 10-year license file (`idapro.hexlic`) for IDA Pro.
- 📦 **All Add-ons Included**: Includes support for multiple architectures like x86, ARM, MIPS, PPC, RISC-V, and ARC.
- ⚡ **Cross-platform**: Fully compatible with Windows, Linux, and macOS.
- ✅ **Verification**: Ensures that binaries are patched correctly and checks if they are already patched.

## Supported Versions

- [IDA Pro 9.1 ](https://t.me/drmechan1sm/392)

## Installation

### Requirements

Before running the tool, ensure the following dependencies are installed:

- Python 3.7+ (We recommend using Python 3.8 or above)
- An existing IDA Pro installation

### Clone the repository

```bash
git clone https://github.com/ThatNotEasy/IDA-Patcher
cd IDA-Patcher
```

### Usage

Run the tool with the following command:

```bash
python main.py
```

Follow the on-screen prompts:

1. The tool will **generate a license file** (`idapro.hexlic`).
2. You'll be asked to **provide the path to your IDA Pro installation**.
3. It will automatically **patch the necessary binaries** and move the generated license file to the correct IDA directory.

## Technical Details

- **Patch Pattern**: The patch modifies the cryptographic verification in the IDA Pro binaries.
  
  **Original Pattern**: `EDFD425CF978`  
  **Patched Pattern**: `EDFD42CBF978`

- **License Features**:
  - 10-year validity
  - All processor modules included
  - RSA-signed for authenticity
 
- ![{AB95A9B8-E0F7-45BE-A254-38EEAE780CF3}](https://github.com/user-attachments/assets/b9860e13-16ab-4aef-a062-9880a72289c5)

## Disclaimer

⚠️ **Important**: This tool is provided for **educational purposes only**. Use it only on software you legally own or have permission to modify. The maintainers are **not responsible** for any misuse of this tool or any resulting consequences. Always respect software licenses and intellectual property rights.
