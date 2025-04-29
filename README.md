# macOS Development Environment Setup

Automated idempotent setup script for macOS development environment. This script installs and configures essential development tools, programming languages, and applications commonly used in software development.

## Quick Install

```bash
curl -H 'Cache-Control: no-cache' -O https://raw.githubusercontent.com/sartaj/macos-configurator/master/configure.sh && bash configure.sh
```

## What Gets Installed

The script sets up the following:

### System Configuration
- macOS system preferences (Finder, keyboard, mouse settings)
- Rosetta 2 (for Apple Silicon Macs)
- XCode Command Line Tools

### Development Tools
- Homebrew (package manager)
- GitHub CLI
- Oh My Zsh (shell configuration)

### Programming Languages & Environments
- Python (via Miniconda and Pyenv)
- Node.js (via NVM)
- Go
- Docker Desktop
- Ollama (AI model runner)

## Shell Configuration

Warning: The shell overrides ~/.zprofile.

No manual configuration is needed - the script handles all environment setup automatically.

## Post-Installation

After running the script:

1. Restart your terminal for all changes to take effect
2. Launch Docker Desktop manually (if installed)
3. Configure GitHub CLI by running `gh auth login`

## Requirements

- macOS (Apple Silicon)
- Administrator privileges (for installing system packages)
- Internet connection

## Customization

You can modify the `configure.sh` script directly to customize which tools and configurations are installed.
