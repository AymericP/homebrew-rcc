# homebrew-tap

Homebrew tap for **[rcc](https://github.com/AymericP/rcc-ai)** — the Rust Code
Compactor. Transparent Claude Code hooks that strip comments/docstrings from what
Claude reads and dedupe re-reads, cutting token use 30–50% per read. Your files
never change.

## Install

```bash
brew install AymericP/tap/rcc
```

That's it — the formula **also wires up the Claude Code hooks** for you
(`rcc init --global`, which backs up `~/.claude/settings.json` first). Restart
Claude Code, then watch your savings:

```bash
rcc gain
```

> Prefer the [Claude Code plugin](https://github.com/AymericP/rcc-ai/tree/main/plugins/rcc)?
> Use the plugin **or** this formula — both register the hooks, so running both
> would register them twice.

## Updating

```bash
brew update && brew upgrade rcc
```

---

`Formula/rcc.rb` is generated from the
[rcc release assets](https://github.com/AymericP/rcc-ai/releases) and pushed here
automatically by the rcc release workflow. Source + issues:
[AymericP/rcc-ai](https://github.com/AymericP/rcc-ai).
