Harmonybrew

The Harmonybrew project is a port of Homebrew to the OpenHarmony platform, providing HarmonyOS users with an out-of-the-box package manager and accompanying software repository, supporting operation on various HarmonyOS devices such as HarmonyOS PCs, HarmonyOS development boards, and HarmonyOS containers.

Device Support

Device Type | Representative Product | Minimum System Version | Command Line Environment | Architecture | Support Level

HarmonyOS PC | HUAWEI MateBook Pro | HarmonyOS 6.1.0.117 SP68 | HiShell arm64 | Tier 2 (Low)

HarmonyOS Development Board | dayu200 (rk3568) | OpenHarmony 6.1 | hdc shell | arm64 | Tier 1 (High)

HarmonyOS Container | DockerHarmony | OpenHarmony 6.1 | Any arm64 | Tier 1 (High)


💡 About Platform Compatibility


HarmonyOS, as a commercial distribution of OpenHarmony, theoretically inherits its ecosystem, so this project can also run on HarmonyOS.


However, please note: Running does not guarantee perfect support. Some packages may function correctly on the development board (hdc shell) or in containers, but may be limited in the HarmonyOS PC's HiShell environment due to system security restrictions or other factors. This is a system-level native limitation, not a problem with the project itself.


Installation Guide

HarmonyOS PC

HarmonyOS Development Board

HarmonyOS Container

Common Operations

The following are some commonly used Homebrew operations. For more information, please refer to the official Homebrew documentation.

`zsh -c "$(curl -fsSL https://harmonybrew.atomgit.com/install.sh)" # Install HarmonyOS version of Homebrew
`zsh -c "$(curl -fsSL https://harmonybrew.atomgit.com/uninstall.sh)" # Uninstall HarmonyOS version of Homebrew
`brew update # Update Homebrew package manager and package index
`brew formulae # List the available packages in the software repository
`brew search [keyword] # Search for packages in the software repository by keyword
`brew install [formula] # Install a package
`brew uninstall [formula] # Uninstall a package
`brew list # View the list of installed packages
`rm -rf $(brew --cache) # Clear the cache` `/storage/Users/currentUser/.harmonybrew` # Completely delete the Homebrew installation directory (cleaner than an uninstallation script)

Note: Homebrew is a "rolling update" package management system. Its package version maintenance strategy differs from apt in Ubuntu or yum in Red Hat. If you are unfamiliar with Homebrew or other rolling update package management systems, please familiarize yourself with their characteristics to avoid confusion.

Other Documentation

Contribution Guidelines

Feedback

Community Notices

FAQ
Featured Software
