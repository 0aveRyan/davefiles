# Davefiles

This repository contains my personal dotfiles, managed using [Chezmoi](https://www.chezmoi.io/). These configuration files set up my development environment with various tools and customizations.

They don't include my [Setapp](https://setapp.com) rig, I just hit the favorite heart and download 🤷‍♂️

## Overview

- Shell: Zsh with Oh My Zsh
- Theme: Powerlevel10k
- Package Manager: Homebrew
- Development Tools: PHP, Node.js, Python, Rust, and more

## Key Components

1. **Brewfile**: Lists all the packages, casks, and VS Code extensions installed via Homebrew.
2. **Zsh Configuration**:
   - `.zshrc`: Main Zsh configuration file
   - `.zsh_aliases`: Custom aliases
   - `.zsh_exports`: Environment variables and path configurations
   - `.p10k.zsh`: Powerlevel10k theme configuration
3. **Herd Configuration**: PHP development environment setup
4. `.hushlogin`: Disables the login message when opening a new terminal session

## Installation

1. Install Chezmoi:
   ```
   brew install chezmoi
   ```

2. Initialize Chezmoi with this repository:
   ```
   chezmoi init https://github.com/0aveRyan/davefiles.git
   ```

3. Apply the dotfiles:
   ```
   chezmoi apply
   ```

## Key Aliases

- `cm`: shortcut for `chezmoi`
- `f`: open current directory in Finder
- `h`: navigate to Herd directory
- `mu`: navigate to `wp-content/mu-plugins`
- `p`: navigate to `wp-content/plugins`
- `t`: navigate to `wp-content/themes`
- `v` or `vsc`: open current directory in Visual Studio Code
- `wpc`: navigate to `wp-content`

## Customization

Feel free to fork this repository and modify the configurations to suit your needs. Remember to update the Brewfile if you add or remove any packages.

## Notes

- This setup is optimized for macOS with Herd for PHP development.
- The configuration includes settings for multiple PHP versions (7.4 to 8.4) managed by Herd.
- NVM (Node Version Manager) is configured to work with Herd.
- The `.hushlogin` file suppresses the system copyright notice, last login time, and mail check that normally appears when opening a new terminal session.
- Some configurations may need adjusting based on your specific system and preferences.

## License

This project is open-sourced under the MIT License.
