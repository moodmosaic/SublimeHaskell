This is *my* fork of [SublimeHaskell/SublimeHaskell][SublimeHaskell/SublimeHaskell]. — Key improvements:

- Syntax for Haskell and Cabal is rewritten (in sync with [sublimehq#2225][sublimehq#2225])
- Syntax for Haskell has its own *dedicated* Monokai-based color scheme
- Output pane is removed in favor of built-in gutter icons

The ultimate goal is to turn this into a SublimeHaskell-*Lite*; support only [hsdev][hsdev], put everything in a single source file, remove everything except icons.

---

### Haskell color scheme

Provided with this package is a *dedicated* Monokai-based color scheme, tuned by myself for Haskell files. To enable it you'll need to create the following file:

Haskell-SublimeHaskell.sublime-settings with content:

```json
// These settings override both User and Default settings for the Haskell-SublimeHaskell syntax
{
  "color_scheme": "Packages/SublimeHaskell/Themes/Haskell.sublime-color-scheme"
}
```

If you want to use this syntax globally (outside the context of SublimeHaskell, even if you have the plugin turned off) then you'll need to create another file:

Haskell.sublime-settings with content:

```json
// These settings override both User and Default settings for the Haskell syntax
{
  "color_scheme": "Packages/SublimeHaskell/Themes/Haskell.sublime-color-scheme"
}
```

[SublimeHaskell/SublimeHaskell]:
  https://github.com/SublimeHaskell/SublimeHaskell
[sublimehq#2225]:
  https://github.com/sublimehq/Packages/pull/2225
[hsdev]:
  https://github.com/mvoidex/hsdev
