# Secure Password Generator
 
## Overview
A Python-based tool for generating strong, secure passwords with customizable complexity.

## Features
- Generate passwords with configurable length
- Include/exclude character types (uppercase, lowercase, numbers, symbols)
- Cryptographically secure random generation
- Simple command-line interface

## Installation
```bash
git clone https://github.com/yourusername/Secure-password-generator.git
cd Secure-password-generator
pip install -r requirements.txt
```

## Usage
```bash
python password_generator.py
```

## Requirements
- Python 3.7+
- `secrets` module (built-in)

## Security
- Uses `secrets` module for cryptographically strong random generation
- Avoids predictable password patterns

## License
MIT License
