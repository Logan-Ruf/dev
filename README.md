# WSL Setup

Automated setup scripts for configuring a new WSL environment.

## Usage

```bash
./run
```

You will be prompted for your git name and email (defaults to the repo owner's credentials if left blank).

### Options

- `--dry` — Preview which scripts would run without executing them.
- Pass a filter string to only run scripts whose path matches it:

```bash
./run git_settings       # only run the git_settings script
./run --dry neovim       # dry-run the neovim script
```

## Scripts

The `runs/` directory contains individual setup scripts:

| Script | Description |
|---|---|
| `azure` | Azure CLI setup |
| `claude` | Claude Code setup |
| `git_settings` | Git global config (name, email, editor, defaults) |
| `locale` | Locale configuration |
| `neovim` | Neovim installation and config |
| `nvm` | Node Version Manager setup |
| `pinentry` | GPG pinentry configuration |
| `python` | Python tooling setup |
| `rust` | Rust toolchain setup |
| `tmux` | Tmux installation and config |
| `zsh` | Zsh and oh-my-zsh setup |
