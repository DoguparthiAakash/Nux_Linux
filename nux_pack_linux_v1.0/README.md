# Nux Programming Language - Linux Distribution

```
███╗  ██╗██╗  ██╗██╗  ██╗
████╗ ██║██║  ██║╚██╗██╔╝
██╔██╗██║██║  ██║ ╚███╔╝
██║╚████║██║  ██║ ██╔██╗
██║ ╚███║╚██████╔╝██╔╝ ██╗
╚═╝  ╚══╝ ╚═════╝ ╚═╝  ╚═╝
```

**Version:** 1.0.0  
**Platform:** Linux (x86_64, ARM64)

## Quick Start

Install Nux with a single command:

```bash
sudo ./setup.sh
```

## System Requirements

- **OS:** Ubuntu 20.04+, Debian 11+, Fedora 35+, Arch Linux, or compatible
- **Dependencies:** gcc, make, git (auto-installed if missing)
- **Disk Space:** ~100 MB
- **RAM:** 512 MB minimum

## Installation

### 1. Extract the Package

```bash
cd nux_pack_linux
```

### 2. Run the Installer

```bash
sudo ./setup.sh
```

The installer will:
- ✓ Check system dependencies
- ✓ Create installation directories
- ✓ Install Nux runtime and libraries
- ✓ Configure environment variables
- ✓ Set up PATH

### 3. Verify Installation

Open a new terminal and run:

```bash
nux --version
```

You should see: `Nux v1.0.0 (Linux)`

## Getting Started

### Start the REPL

```bash
nux repl
```

### Run Example Programs

```bash
# Hello World
nux examples/hello.nux

# Web Server
nux examples/web_server.nux

# AI Demo
nux examples/ai_demo.nux
```

### Create Your First Program

```bash
echo 'import "std.io"; println("Hello, Nux!");' > hello.nux
nux hello.nux
```

## What's Included

- **Standard Libraries** (79 files)
  - `lib/std/` - Core utilities, I/O, networking, graphics
  - `lib/ai/` - Neural networks, transformers, GANs, RL
  - `lib/os/` - Kernel, scheduler, memory management
  - `lib/embedded/` - Hardware control, GPIO, sensors

- **Examples**
  - `hello.nux` - Basic syntax and I/O
  - `web_server.nux` - HTTP server
  - `ai_demo.nux` - Neural network training

- **Tools**
  - `nux` - Runtime and REPL
  - `nuxc` - Compiler
  - `nuxr` - Script runner

## Troubleshooting

### Permission Denied

Make sure to run the installer with `sudo`:
```bash
sudo ./setup.sh
```

### Command Not Found

Restart your terminal or manually source the environment:
```bash
source /etc/profile.d/nux.sh
```

### Missing Dependencies

The installer auto-installs gcc, make, and git. If you encounter issues:
```bash
# Ubuntu/Debian
sudo apt-get install gcc make git

# Fedora
sudo dnf install gcc make git

# Arch
sudo pacman -S gcc make git
```

## Uninstallation

```bash
sudo ./setup.sh uninstall
```

## Documentation

- **Language Guide:** https://nux-lang.org/docs
- **API Reference:** https://nux-lang.org/api
- **Examples:** https://github.com/nux-lang/examples

## Support

- **Issues:** https://github.com/nux-lang/nux/issues
- **Community:** https://discord.gg/nux-lang
- **Email:** support@nux-lang.org

## License

Nux Programming Language is released under the MIT License.  
See LICENSE file for details.

---

**Happy Coding!** 🚀
