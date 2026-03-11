# OpenCode Dark Islands

An OpenCode theme inspired by [VS Code Dark Islands](https://github.com/bwya77/vscode-dark-islands).

![Dark Islands theme demo](demo.png)

## Install

OpenCode custom theme docs: https://opencode.ai/docs/themes

Install it globally with one command:

```bash
mkdir -p ~/.config/opencode/themes && curl -fsSL https://raw.githubusercontent.com/jacobjmc/opencode-dark-islands/main/islands-dark.json -o ~/.config/opencode/themes/islands-dark.json
```

Then open OpenCode, run `/theme`, and pick `islands-dark`.

If you want it only for one project, run this from the project root:

```bash
mkdir -p .opencode/themes && curl -fsSL https://raw.githubusercontent.com/jacobjmc/opencode-dark-islands/main/islands-dark.json -o .opencode/themes/islands-dark.json
```

Then run `/theme` and pick `islands-dark`.

If you want to make it your default theme, add this to `~/.config/opencode/tui.json`:

```json
{
  "$schema": "https://opencode.ai/tui.json",
  "theme": "islands-dark"
}
```

## Notes

- OpenCode looks best with truecolor enabled. `echo $COLORTERM` should print `truecolor` or `24bit`.
- Theme lookup order comes from the docs: built-in themes, user themes, project-root themes, then the current working directory.
- If you want the extra "glass" feel from the screenshot, pair this with a terminal that supports blur, opacity, and good font rendering like Ghostty.

## License

MIT License - see [LICENSE](LICENSE) file for details.
