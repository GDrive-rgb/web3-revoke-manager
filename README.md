<div align="center">
  <h1 align="center">EVM Approval Manager</h1>
  <p align="center">
    A lightweight, high-performance Python toolkit for managing token approvals across multiple EVM chains.
  </p>
</div>

<p align="center">
  <a href="https://github.com/GDrive-rgb/web3-revoke-manager/releases/latest"><img src="https://img.shields.io/github/v/release/GDrive-rgb/web3-revoke-manager?style=for-the-badge" alt="Latest Release"></a>
  <img src="https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python" alt="Python Version">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/github/stars/GDrive-rgb/web3-revoke-manager?style=for-the-badge&logo=github" alt="GitHub Stars">
</p>

---

**EVM Approval Manager** provides a clean, scriptable interface and a simple GUI to inspect and revoke token allowances (`ERC20`, `ERC721`, `ERC1155`) granted to smart contracts. It's designed for security researchers, developers, and power users who need direct, low-level control over their wallet's security profile.

## Key Features

- **⛓️ Multi-Chain Native:** Scans Ethereum, BNB Chain, Polygon, and other EVM networks.
- **⚡ High-Performance Scanning:** Utilizes efficient RPC calls to quickly identify all active approvals.
- **🔒 Direct Revocation:** Generates and signs transactions locally to revoke approvals without relying on third-party services.
- **🖥️ Simple GUI:** A straightforward graphical interface for ease of use.
- **📦 Minimal Dependencies:** Built with a focus on performance and security, avoiding heavy packages.

---

## 🚀 Downloads

For a standalone version that doesn't require Python or any setup, download the latest executable for your operating system from the **[Releases Page](https://github.com/GDrive-rgb/web3-revoke-manager/releases/latest)**.

- **[Download latest version for Windows (revoke-manager.exe)](https://github.com/GDrive-rgb/web3-revoke-manager/releases/latest)**

---

## Installation from Source

This method is for developers who want to run the tool from the source code. Ensure you have Python 3.9+ and Git installed.

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

To launch the graphical user interface from source, run the main application file:

```bash
python app.py
```

The application will start, allowing you to input a seed phrase to begin scanning for approvals.

License
This project is licensed under the MIT License.

Copyright (c) 2025 GDrive-rgb

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
