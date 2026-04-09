# Firewall Auto Config

![Security](https://img.shields.io/badge/Security-Tool-red)
![Bash](https://img.shields.io/badge/Bash-Script-green)
![Firewall](https://img.shields.io/badge/Firewall-iptables-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

An automated firewall configuration tool that applies security rulesets to Linux servers using iptables/nftables. Enforces network-level security policies with minimal manual intervention.

## Description

Firewall Auto Config automates the deployment and management of firewall rules on Linux servers. It provides predefined security profiles for common use cases (web server, database, application server) and supports custom rule definitions. Designed for consistent firewall policy enforcement across multiple hosts.

## Features

- Automated iptables/nftables rule deployment
- Predefined security profiles for common server roles
- Default-deny ingress with configurable allow rules
- Rate limiting and connection tracking
- Logging of dropped and rejected packets
- Backup and rollback of firewall configurations
- Makefile-based build and test workflow

## Tech Stack

- **Language:** Bash
- **Tools:** iptables, nftables, ufw
- **Target OS:** Linux (Ubuntu / Debian / CentOS)
- **Build Tool:** GNU Make

## Quick Start

```bash
# Clone the repository
git clone https://github.com/razinahmed/firewall-auto-config.git
cd firewall-auto-config

# Review the configuration
make build
make test

# Apply firewall rules (requires root)
sudo bash scripts/configure.sh
```

## Usage

```bash
# Build and test
make build
make test
```

## Project Structure

```
firewall-auto-config/
  styles/
    theme.css          # UI theme configuration
  Makefile             # Build and test automation
  SECURITY.md          # Security policy
  LICENSE              # MIT License
```

## Contributing

Contributions are welcome. Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
