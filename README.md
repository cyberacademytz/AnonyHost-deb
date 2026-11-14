# AnonyHost

**AnonyHost** is a powerful tool designed for cybersecurity and anonymity management on Linux systems. It is designed for Debian-based distributions, including Debian and Kali Linux.

## Features

- Designed for cybersecurity and anonymity management on Linux
- Supports Debian and Kali Linux
- Simple `.deb` package installation
- Helps manage privacy- and anonymity-related system settings
- Suitable for security researchers, penetration testers, and privacy-conscious users
- Lightweight and command-line oriented

## Requirements

Before installing AnonyHost, ensure that your system meets the following requirements:

- Debian, Kali Linux, or another compatible Debian-based distribution
- A 64-bit (`amd64`) system
- Terminal access
- Administrative (`sudo`) privileges
- An internet connection to download the package

## Installation

### 1. Download AnonyHost

Download the AnonyHost Debian package as a ZIP archive:

**[Download AnonyHost-deb as ZIP](https://github.com/cyberacademytz/AnonyHost-deb/archive/refs/heads/main.zip)**

This will download a ZIP file containing the AnonyHost `.deb` package.

### 2. Extract the ZIP file

After the download completes, extract the ZIP file.

You can extract it using your file manager, or use the terminal:

```bash
cd ~/Downloads
unzip AnonyHost-deb-main.zip
cd AnonyHost-deb-main
```

If `unzip` is not installed, install it first:

```bash
sudo apt update
sudo apt install unzip
```

After extraction, locate the Debian package:

```bash
anonyhost_1.0.0_amd64.deb
```

### 3. Verify the package integrity

Before installing, verify that the `.deb` file has not been modified or corrupted by checking its SHA-256 hash.

Run the following command from the folder containing the `.deb` file:

```bash
sha256sum anonyhost_1.0.0_amd64.deb
```

The expected output is:

```text
2aa592476f865fa1e3d85535157090e5baef710b1fe536495afdcf7b11df41f4  anonyhost_1.0.0_amd64.deb
```

If the hash matches exactly, the package is intact and safe to install.

If the hash does **not** match, do **not** install the package. Delete the downloaded ZIP file and `.deb` file, then download them again.

### 4. Install AnonyHost

With the verified `.deb` file in your current terminal directory, install it using `apt`:

```bash
sudo apt install ./anonyhost_1.0.0_amd64.deb
```

Alternatively, install it using `dpkg`:

```bash
sudo dpkg -i anonyhost_1.0.0_amd64.deb
```

If dependency errors occur after using `dpkg`, run:

```bash
sudo apt --fix-broken install
```

### 5. Verify the installation

Check that AnonyHost was installed successfully:

```bash
dpkg -l | grep anonyhost
```

## Getting Started

After installation, open a terminal and run:

```bash
anonyhost
```

To view available commands, options, and usage information, run:

```bash
anonyhost --help
```

## Security and Responsible Use

Use AnonyHost responsibly and only for legitimate purposes.

- Use it only on devices you own or have explicit permission to test.
- Do not use AnonyHost to bypass laws, organizational policies, or terms of service.
- Keep your operating system and security tools updated.
- Back up important settings before changing network or identity-related configurations.
- Remember that no tool can guarantee complete anonymity or security.
- Do not use AnonyHost for harassment, fraud, unauthorized access, malware distribution, or other illegal activity.

## Uninstallation

To remove AnonyHost, run:

```bash
sudo apt remove anonyhost
```

To remove the package and its configuration files, run:

```bash
sudo apt purge anonyhost
```

Then remove unnecessary dependencies:

```bash
sudo apt autoremove
```
## Contributing

Contributions are welcome. To contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make and test your changes.
4. Submit a pull request with a clear description.

## License

This project is provided for educational and authorized cybersecurity purposes. Review the repository’s license file for exact terms before redistribution or modification.

## Disclaimer

AnonyHost is intended for lawful cybersecurity research, privacy management, and authorized testing only. The developers are not responsible for misuse, damage, or illegal activity performed with this tool.
