# EVM Approval Manager

A lightweight, high-performance Python toolkit for managing token approvals across multiple EVM chains.

![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![GitHub Stars](https://img.shields.io/github/stars/GDrive-rgb/web3-revoke-manager?style=for-the-badge&logo=github)

---

**EVM Approval Manager** provides a clean, scriptable interface and a simple GUI to inspect and revoke token allowances (`ERC20`, `ERC721`, `ERC1155`) granted to smart contracts. It's designed for security researchers, developers, and power users who need direct, low-level control over their wallet's security profile.

## Key Features

- **⛓️ Multi-Chain Native:** Scans Ethereum, BNB Chain, Polygon, and other EVM networks.
- **⚡ High-Performance Scanning:** Utilizes efficient RPC calls to quickly identify all active approvals.
- **🔒 Direct Revocation:** Generates and signs transactions locally to revoke approvals without relying on third-party services.
- **🖥️ Simple GUI:** A straightforward graphical interface for ease of use.
- **📦 Minimal Dependencies:** Built with a focus on performance and security, avoiding heavy packages.

---

## Installation

Ensure you have Python 3.9+ and Git installed.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/GDrive-rgb/web3-revoke-manager.git
    cd web3-revoke-manager
    ```

2.  **Install dependencies:**
    It is highly recommended to use a virtual environment.
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

3.  **Configure Environment:**
    The application requires RPC and Explorer API keys. Copy the example file and populate it with your credentials.
    ```bash
    cp .env.example .env
    ```
    Then, edit the `.env` file with your keys.

## Usage

To launch the graphical user interface, run the main application file from the project root:

```bash
python app.py
```

The application will start, allowing you to input a seed phrase to begin scanning for approvals.
⚠️ Security Notice
This application is designed to handle sensitive cryptographic data (seed phrases). All operations that use this data are intended to be performed locally on your machine.
AUDIT THE CODE: Always review the source code before use to ensure it performs as expected.
USE IN ISOLATED ENVIRONMENT: For maximum security, run this tool in a sandboxed or isolated environment.
USE AT YOUR OWN RISK: The authors and maintainers of this project are not liable for any direct or indirect damages or loss of funds resulting from the use of this software.
License
This project is licensed under the MIT License.

Copyright (c) 2024 GDrive-rgb

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
