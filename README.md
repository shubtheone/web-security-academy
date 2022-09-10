# Burp
Experiements with [Burp Suite](https://portswigger.net/burp) and [Kali](https://www.kali.org/).

## Setup
```sh
# Install https://brew.sh/
brew bundle
vagrant up
```
Configure Chromium to trust the Burp CA certificate:

1. In the VM, open Burp's integrated Chromium browser.
2. Go to `http://burpsuite` and download the `cacert.der` certificate.
3. Go to `chrome://settings/certificates` and select `Authorities`.
4. Click `Import`, select `cacert.der`, and trust for web identies.

## Contents
- [SQL injection](sql-injection/README.md)