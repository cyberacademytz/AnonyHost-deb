# AnonyHost

**AnonyHost** is a powerful tool designed for cybersecurity and anonymity management on Linux systems. It helps users configure privacy-focused network settings, manage identity-related system information, and support secure testing workflows on Debian-based distributions such as Debian and Kali Linux.

> **Important:** Use AnonyHost only on systems and networks you own or are authorized to test. Anonymity tools do not guarantee legal or complete privacy, and they must not be used for unlawful activity.

## Features

- Designed for Linux-based cybersecurity and privacy workflows
- Simple installation through a Debian package (`.deb`)
- Supports Debian and Kali Linux environments
- Helps manage anonymity-related system and network configurations
- Suitable for security researchers, penetration testers, and privacy-conscious users
- Lightweight command-line-oriented workflow

## Requirements

Before installing AnonyHost, ensure your system meets the following requirements:

- Debian, Kali Linux, or another compatible Debian-based distribution
- A 64-bit (`amd64`) system
- Terminal access
- Administrative (`sudo`) privileges for installation
- An active internet connection to download the package

## Installation

To install AnonyHost on Debian or Kali Linux, follow these simple steps:

1. **Download** the latest `.deb` package (`anonyhost_1.0.0_amd64.deb`) from the [Releases page](https://github.com/cyberacademytz/AnonyHost/releases).
2. **Open your terminal** and navigate to the folder where you downloaded the file (usually your Downloads folder):

   ```bash
   cd ~/Downloads
   ```

3. **Install the package** using `apt`:

   ```bash
   sudo apt install ./anonyhost_1.0.0_amd64.deb
   ```

   Alternatively, install it using `dpkg`:

   ```bash
   sudo dpkg -i anonyhost_1.0.0_amd64.deb
   ```

   If dependency errors appear after using `dpkg`, run:

   ```bash
   sudo apt --fix-broken install
   ```

4. **Verify the installation**:

   ```bash
   anonyhost --version
   ```

   If the version command is not available, check the installed package with:

   ```bash
   dpkg -l | grep anonyhost
   ```

## Getting Started

After installation, open a terminal and run:

```bash
anonyhost
```

You can also view the available commands and options with:

```bash
anonyhost --help
```

Use the help menu to explore the available anonymity, network, and system-management features.

## Usage

AnonyHost is intended to assist with cybersecurity and anonymity management tasks, such as:

- Reviewing and managing privacy-related system settings
- Supporting secure and anonymous testing workflows
- Managing network-related configurations
- Assisting security professionals during authorized assessments
- Providing a simple interface for anonymity-focused Linux operations

Always review the tool’s output before applying system changes, especially when running commands with administrative privileges.

## Security and Responsible Use

AnonyHost should be used responsibly and only for legitimate purposes.

- Use it only on devices you own or have explicit permission to test.
- Do not use anonymity tools to bypass laws, terms of service, or organizational policies.
- Keep your operating system and security tools updated.
- Back up important system settings before making network or identity-related changes.
- Understand that no tool can guarantee complete anonymity or security.
- Do not use AnonyHost for harassment, fraud, unauthorized access, malware distribution, or other illegal activity.

## Uninstallation

To remove AnonyHost from your system, run:

```bash
sudo apt remove anonyhost
```

To remove the package along with its configuration files, run:

```bash
sudo apt purge anonyhost
```

Then clean up unnecessary dependencies:

```bash
sudo apt autoremove
```

## Troubleshooting

| Issue | Possible solution |
|---|---|
| Permission denied during installation | Run the installation command with `sudo` |
| Package cannot be installed | Ensure you downloaded the `amd64` package and are using a 64-bit Debian-based system |
| Dependency errors after `dpkg -i` | Run `sudo apt --fix-broken install` |
| Command not found after installation | Restart your terminal or check whether `/usr/local/bin` or `/usr/bin` is in your `PATH` |
| Installation fails | Verify the downloaded file is complete and matches the latest release |

## Contributing

Contributions are welcome. If you would like to improve AnonyHost, report a bug, suggest a feature, or submit documentation updates:

1. Fork the repository.
2. Create a new branch for your change.
3. Make your changes and test them.
4. Submit a pull request with a clear description.

## License

This project is provided for educational and authorized cybersecurity purposes. Review the repository’s license file for exact terms before redistribution or modification.

## Disclaimer

AnonyHost is intended for lawful cybersecurity research, privacy management, and authorized testing only. The developers are not responsible for misuse, damage, or illegal activity performed with this tool.
