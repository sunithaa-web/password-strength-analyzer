# 🔐 Password Strength Analyzer with Custom Wordlist Generator

## Overview

The **Password Strength Analyzer with Custom Wordlist Generator** is a Python-based cybersecurity project designed to help users evaluate the security of their passwords while demonstrating how attackers may create targeted password guesses using publicly available personal information.

This project combines password strength analysis, entropy calculation, common pattern detection, and custom wordlist generation into a single application. It is intended for **educational purposes, cybersecurity awareness, and authorized security testing** only.

---

## Features

### 🔒 Password Strength Analysis

* Evaluates password strength using the **zxcvbn** library.
* Calculates password entropy based on length and character diversity.
* Detects the use of uppercase, lowercase, digits, and special characters.
* Provides password strength ratings:

  * Very Weak
  * Weak
  * Moderate
  * Strong
  * Very Strong
* Estimates the time required to crack the password.
* Offers recommendations for creating stronger passwords.

### 🛡️ Weak Password Detection

The analyzer identifies common security weaknesses, including:

* Dictionary words
* Repeated characters
* Sequential patterns (e.g., `123456`, `abcdef`)
* Keyboard patterns (e.g., `qwerty`, `asdfgh`)
* Common passwords
* Passwords containing personal information

### 📖 Custom Wordlist Generator

Generate personalized password wordlists using user-provided information such as:

* First name
* Last name
* Nickname
* Pet name
* Birth year
* Birthday
* Favorite team
* Favorite movie
* City
* Phone number digits

The application automatically creates hundreds or thousands of realistic password combinations.

### 🔄 Password Mutation Engine

The generator produces multiple password variations using common techniques such as:

* Leetspeak substitutions (`a → 4`, `e → 3`, `o → 0`, etc.)
* Uppercase and lowercase combinations
* Appending years
* Adding special characters
* Combining multiple personal details
* Prefixes and suffixes

### 📂 Export Functionality

Generated wordlists can be exported as:

* `.txt` files for educational password auditing tools
* JSON statistics containing generation details

### 💻 User Interface

The project supports:

* Command-Line Interface (CLI) using `argparse`
* Graphical User Interface (GUI) using `tkinter`

---

## Technologies Used

* Python 3
* zxcvbn
* NLTK
* argparse
* tkinter
* itertools
* pathlib
* datetime
* JSON
* Regular Expressions (re)

---

## Project Structure

```text
PasswordStrengthAnalyzer/
│
├── analyzer.py
├── entropy.py
├── wordlist_generator.py
├── mutations.py
├── exporter.py
├── reports.py
├── gui.py
├── main.py
│
├── output/
│   ├── custom_wordlist.txt
│   └── stats.json
│
├── requirements.txt
└── README.md
```

---

## How It Works

1. The user enters a password to evaluate its security.
2. The analyzer measures password complexity, entropy, and resistance to common attack techniques.
3. The user can optionally provide personal information to generate a custom wordlist.
4. The application creates realistic password combinations using mutation techniques such as leetspeak, year appending, and symbol insertion.
5. The generated wordlist can be exported for educational password auditing and security testing.

---

## Learning Objectives

This project helps users understand:

* Password security principles
* Entropy and password complexity
* Dictionary and brute-force attacks
* Social engineering risks
* Wordlist generation techniques
* Secure password creation best practices
* Ethical password auditing

---

## Future Enhancements

* Password breach checking using the Have I Been Pwned API
* Machine learning-based password strength prediction
* Custom rule creation for mutations
* PDF report generation
* Multi-language dictionary support
* Advanced GUI with CustomTkinter
* Cross-platform desktop packaging

---

## Disclaimer

This project is intended **solely for educational purposes, cybersecurity awareness, and authorized security assessments**. It must only be used on systems, accounts, or data for which you have explicit permission. The developers are not responsible for any misuse or unauthorized activities involving this software.
