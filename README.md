# Nodepay Referral Bot

This script automates the process of registering accounts on Nodepay using referral codes. It allows you to configure captcha services and proxies, and it stores account details for each successful referral.

## Features

- **Captcha Solver Integration**: Supports multiple captcha services (Capmonster, Anticaptcha, 2Captcha).
- **Proxy Support**: Optionally uses a list of proxies for each request.
- **Automatic Account Registration**: Generates random usernames, emails, and passwords for new accounts.
- **Account Logging**: Saves successfully registered account details to `accounts.txt`.
- **Customizable**: Easily configurable to adjust the number of referrals and captcha services.

## Requirements

- Python 3.7 or higher.
- Dependencies listed in the `requirements.txt` file.

## Installation

1. Clone this repository or download the script file:

    ```bash
    git clone https://github.com/juliwicks/nodepay-referral
    cd nodepay-referral
    ```

2. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Ensure you have the `proxies.txt` file (if using proxies), which should contain your proxy list in the following format:

    ```
    protocol://user:pass@ip:port
    ```

## Configuration

1. **Captcha Service**: You can choose from the following captcha services:
   - **Capmonster**: Requires a Capmonster API key.
   - **Anticaptcha**: Requires an Anticaptcha API key.
   - **2Captcha**: Requires a 2Captcha API key.

2. **Proxies**: If you want to use proxies, you can specify them in the `proxies.txt` file. Each line should contain a proxy in the format `protocol://user:pass@ip:port`.

## Usage

Run the script using the following command:

```bash
python script.py
