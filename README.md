# zsh-completions

A Zsh plugin providing custom tab completions for various CLI tools.

## Requirements

No external dependencies are required. If [Homebrew](https://brew.sh) is installed, its `site-functions` directory is automatically added to the `$fpath` for additional completions.

## Installation

### zinit

```zsh
zinit light mikkelkaysen/zsh-completions
```

### Oh My Zsh

Clone the repository into your custom plugins directory:

```zsh
git clone https://github.com/mikkelkaysen/zsh-completions.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-completions
```

Then add `zsh-completions` to your plugins list in `~/.zshrc`:

```zsh
plugins=(... zsh-completions)
```

### zimfw

Add the following to your `~/.zimrc`:

```zsh
zmodule mikkelkaysen/zsh-completions
```

Then run:

```zsh
zimfw install
```

## Provided Completions

| Completion | Command | Description |
|------------|---------|-------------|
| `_dotnet` | `dotnet` | Tab completion for the [.NET CLI](https://github.com/dotnet/cli) |
| `_git-flow` | `git-flow` | Tab completion for [git-flow AVH Edition](https://github.com/petervanderdoes/gitflow-avh) |

### git-flow (AVH Edition) subcommands

The `git-flow` completion supports the following subcommands:

- `init` — Initialize a new git repo with support for the branching model
- `feature` — Manage feature branches
- `bugfix` — Manage bugfix branches
- `config` — Manage configuration
- `release` — Manage release branches
- `hotfix` — Manage hotfix branches
- `support` — Manage support branches
- `version` — Show version information
- `finish` — Finish the current branch
- `delete` — Delete the current branch
- `publish` — Publish the current branch
- `rebase` — Rebase the current branch

## License

[MIT](./LICENSE) — Copyright (c) 2020 Mikkel Kaysen
