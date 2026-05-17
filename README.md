# Starship Config

Personal Starship prompt configuration.

This repository is intentionally separate from terminal emulator configs.
It only manages:

```text
.config/starship.toml
```

## Requirements

- Starship
- A Nerd Font compatible terminal font

This repository does not require sudo. Installing the `starship` binary depends
on the target device. Use an existing install, Nix user profile, Homebrew /
Linuxbrew, or a user-local binary when sudo is unavailable.

## Install Config

```bash
git clone https://github.com/AMkuro/starship-config.git
cd starship-config
./install.sh
```

Preview first:

```bash
./install.sh --dry-run
```

## Shell Setup

Add this to `~/.zshrc`:

```bash
if command -v starship >/dev/null 2>&1; then
  export STARSHIP_CONFIG="$HOME/.config/starship.toml"
  eval "$(starship init zsh)"
fi
```

## License

MIT. See `LICENSE`.

