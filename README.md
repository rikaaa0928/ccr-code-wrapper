# Claude Code Wrapper (ccr-code-wrapper)

A simple wrapper script that provides a convenient `claude` command alias for the `ccr code` command.

## Overview

This project contains a bash wrapper script that allows you to use `claude` as a shorthand for `ccr code`, making it easier to invoke Claude Code functionality from the command line.

## Files

- `claude` - Main wrapper script that forwards all arguments to `ccr code`
- `LICENSE` - GNU General Public License v3.0

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/rikaaa0928/ccr-code-wrapper.git
   cd ccr-code-wrapper
   ```

2. Make the script executable:
   ```bash
   chmod +x claude
   ```

3. Add the script to your PATH or create a symbolic link:
   ```bash
   # Option 1: Add to PATH
   export PATH="$PWD:$PATH"
   
   # Option 2: Create symbolic link (adjust path as needed)
   ln -s "$PWD/claude" /usr/local/bin/claude
   ```

## Usage

After installation, you can use the `claude` command as a drop-in replacement for `ccr code`:

```bash
# Instead of typing:
ccr code [arguments]

# You can now type:
claude [arguments]
```

All arguments passed to the `claude` command are forwarded directly to `ccr code`.

## Prerequisites

- Bash shell
- `ccr` command must be installed and available in your PATH

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request