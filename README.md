# Phishing Link Scanner

The Phishing Link Scanner is a Python-based tool designed to help identify potential phishing websites. By analyzing URL structures and comparing domains against a list of known legitimate domains, the scanner can detect misspelled domain names and suspicious subdomains that are commonly used in phishing attacks. This tool aims to enhance online security by providing a method to quickly and accurately identify phishing attempts.


## Introduction

Phishing is a cyber attack technique where attackers create fake websites that mimic legitimate ones to steal sensitive information, such as usernames, passwords, and credit card details. This project aims to help detect such phishing URLs by checking for domain similarities and other characteristics.

## Mechanics of Phishing Attempts

Phishing attempts often exploit domain similarities to trick users into believing they are visiting legitimate websites. Here are some common tactics:
- **Misspelled Domains**: Attackers use domains that look similar to legitimate ones by replacing characters (e.g., `gooogle.com` instead of `google.com`).
- **Subdomain Tricks**: Legitimate-looking subdomains are used to mask the actual malicious domain (e.g., `google.security-update.com`).
- **Homoglyphs**: Similar-looking characters from different scripts are used (e.g., `gοοgle.com` using Greek 'ο' instead of Latin 'o').

## How It Works

This project uses Python to extract and analyze URL components to detect potential phishing sites. It checks for:
- Known legitimate domains.
- Misspelled domains using Levenshtein distance.
- Suspicious subdomain patterns.

## Usage

The main script to run the phishing link scanner is `Phishing_Link_Scanner.py`. You can use it to check URLs against a list of legitimate domains.

### Example Usage

1. Prepare a list of legitimate domains in the script.
2. Add URLs you want to test.
3. Run the script:

    ```bash
    python Phishing_Link_Scanner.py
    ```
