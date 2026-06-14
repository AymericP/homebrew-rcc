# homebrew-rcc

Homebrew tap for **[rcc](https://github.com/AymericP/rcc-ai)** — the Rust Code
Compactor. Transparent Claude Code hooks that strip comments/docstrings from what
Claude reads and dedupe re-reads, cutting token use 30–50% per read. Your files
never change.

## Install

```bash
brew install AymericP/rcc/rcc
```

Then wire up the Claude Code hooks (this backs up `~/.claude/settings.json`
first) and restart Claude Code:

```bash
rcc init --global
```

Track your savings with `rcc gain`.

> Using the [Claude Code plugin](https://github.com/AymericP/rcc-ai/tree/main/plugins/rcc)
> instead? Then skip `rcc init` — the plugin registers the hooks for you.

## Updating

```bash
brew update
brew upgrade rcc
```

---

The formula is generated from the
[rcc release assets](https://github.com/AymericP/rcc-ai/releases). Issues and
the source live in the [main repo](https://github.com/AymericP/rcc-ai).
