# 🧮 Newabacus - Advanced Calculator Suite

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

A collection of sophisticated web-based calculators and encryption tools featuring modern dark-themed interfaces with responsive design. Built with vanilla HTML, CSS, and JavaScript for maximum compatibility and performance.

## 🎯 Features

- **🔐 Dual Encryption Systems**: Two different Fernet encryption implementations
- **📱 Responsive Design**: Works seamlessly on desktop and mobile devices
- **🌙 Dark Theme**: Modern, eye-friendly dark interface with cyan accents
- **🔢 Calculator Interface**: Intuitive keypad-style input for passwords and equations
- **⚡ Zero Dependencies**: Self-contained HTML files for easy deployment
- **🔒 Secure**: Uses industry-standard Fernet encryption with SHA-256 hashing

## 🛠️ Tools Overview

### 1. Mẹ's Encrypt/Decrypt Calculator
**File**: `index.html`

![Mẹ's Encrypt/Decrypt Calculator](https://github.com/user-attachments/assets/e83d0253-b595-4c71-97de-20aa9568e090)

A user-friendly encryption tool with a calculator-style interface for password input.

**Features:**
- **Fernet Encryption**: Military-grade symmetric encryption
- **SHA-256 Hashing**: Secure password derivation
- **Keypad Interface**: Easy numeric password input
- **Instant Results**: Real-time encryption/decryption
- **Error Handling**: Clear feedback for invalid inputs

**Dependencies:**
- `crypto-js.min.js` - Cryptographic functions
- `fernet.min.js` - Fernet encryption implementation

### 2. Secret Key Calculator (Pyodide)
**File**: `pyodide.html`

![Secret Key Calculator (Pyodide)](https://github.com/user-attachments/assets/6010a9b7-0ea6-48c3-8022-b7889dba95b3)

A Python-powered encryption tool running in the browser using Pyodide.

**Features:**
- **Python Backend**: Full Python cryptography library support
- **Browser-based**: No server required, runs entirely in browser
- **Advanced Encryption**: Access to Python's cryptography ecosystem
- **Scientific Computing**: Powered by Pyodide for complex operations
- **Same Interface**: Consistent UI with the JavaScript version

**Dependencies:**
- Pyodide CDN (v0.23.4)
- Python cryptography library (loaded via Pyodide)

### 3. KAYSIO fx-115ES PLUS Calculator
**File**: `equation_solver.html`

![KAYSIO fx-115ES PLUS Calculator](https://github.com/user-attachments/assets/a963e79c-0ee0-4cf8-adb9-140a1f145dfb)

A calculator inspired by the popular CASIO fx-115ES PLUS scientific calculator.

**Features:**
- **Equation Solver**: Evaluate mathematical expressions
- **Scientific Display**: Green-on-black display mimicking real calculators
- **Formula Support**: Built-in equation solving capabilities
- **Classic Design**: Faithful recreation of calculator aesthetics
- **Error Handling**: Robust error detection and display

## 🚀 Getting Started

### Quick Start
1. Clone the repository:
   ```bash
   git clone https://github.com/NancyCu/Newabacus.git
   cd Newabacus
   ```

2. Open any HTML file in your browser:
   ```bash
   # For local development
   python -m http.server 8000
   # Then open http://localhost:8000/index.html
   ```

3. Or simply open the HTML files directly in your browser.

### Usage Examples

#### Encryption/Decryption
1. **Enter your message** in the "Plain Text" field
2. **Set a password** using the numeric keypad
3. **Click "Encrypt"** to generate a Fernet token
4. **Copy the token** to the "Encrypted String" field
5. **Click "Decrypt"** to recover your original message

#### Equation Solving
1. **Enter an equation** in the input field (e.g., `2 + 3 * 4`)
2. **Click "SOLVE"** or press the solve button
3. **View the result** in the display area

## 🔧 Technical Details

### Encryption Specification
- **Algorithm**: Fernet (AES 128 in CBC mode with HMAC SHA-256)
- **Key Derivation**: SHA-256 hash of user password
- **Base64 Encoding**: All tokens are Base64 encoded for safe transmission
- **Time-based**: Tokens include timestamp for security

### Browser Compatibility
- **Chrome**: ✅ Full support
- **Firefox**: ✅ Full support
- **Safari**: ✅ Full support
- **Edge**: ✅ Full support
- **Mobile**: ✅ Responsive design

### Security Features
- **No Server Required**: All encryption happens client-side
- **No Data Storage**: Nothing is saved or transmitted
- **Memory Safe**: Secure handling of sensitive data
- **Open Source**: Full transparency of security implementation

## 🎨 Design Philosophy

The Newabacus suite follows modern web design principles:

- **Dark Theme**: Reduces eye strain during extended use
- **Cyan Accents**: High contrast for accessibility
- **Responsive Layout**: Adapts to any screen size
- **Intuitive Controls**: Calculator-style interfaces feel familiar
- **Clean Typography**: Segoe UI font stack for readability

## 📂 Project Structure

```
Newabacus/
├── index.html              # Main encryption tool
├── pyodide.html           # Python-powered encryption
├── equation_solver.html   # Scientific calculator
├── crypto-js.min.js       # Cryptographic library
├── fernet.min.js         # Fernet implementation
└── README.md             # This file
```

## 🔐 Security Notice

This tool is designed for educational and personal use. While it uses industry-standard encryption:

- **Client-side only**: No server-side security validation
- **Password strength**: User responsible for strong passwords
- **Local storage**: No automatic secure storage of keys
- **Review code**: Always review cryptographic implementations

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues, fork the repository, and create pull requests.

### Development Setup
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **Fernet Encryption**: Based on the cryptographic specification
- **Pyodide**: For bringing Python to the browser
- **CryptoJS**: For JavaScript cryptographic functions
- **Modern CSS**: For responsive design techniques

---

**Made with ❤️ for secure, accessible computing**