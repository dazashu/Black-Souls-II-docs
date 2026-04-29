# Black Souls II - Documentation Site

Static HTML documentation for the [Black Souls II Mod Loader](https://github.com/dazashu/Black-Souls-II-Mod-Loader). Designed to be hosted on **GitHub Pages**.

🌐 **Live site: <https://dazashu.github.io/Black-Souls-II-docs/>**

## Companion repos

- 🔧 [Black-Souls-II-Mod-Loader](https://github.com/dazashu/Black-Souls-II-Mod-Loader) — runtime mod loader
- 🧩 [Black-Souls-II-Mod](https://github.com/dazashu/Black-Souls-II-Mod) — bundled mods (`creative_mode` + 5 starter templates)
- 📦 [Black-Souls-II-Asset-Extractor](https://github.com/dazashu/Black-Souls-II-Asset-Extractor) — extract / repack `Game.rgss3a`

---

## What's covered

> These are pages on the live site. Clicking them on GitHub would open the HTML source — use these links to view the rendered docs.

| Page | Topic |
|---|---|
| [Installation](https://dazashu.github.io/Black-Souls-II-docs/pages/installation.html) | Install the loader and run your first mod |
| [Creating Mods](https://dazashu.github.io/Black-Souls-II-docs/pages/creating-mods.html) | `main.rb`, the mod loader API, common hooks |
| [Asset Overrides](https://dazashu.github.io/Black-Souls-II-docs/pages/asset-overrides.html) | Drop-in PNG / OGG / data replacements |
| [API Reference](https://dazashu.github.io/Black-Souls-II-docs/pages/api-reference.html) | `ModLoader.*` helpers and registered hooks |
| [Templates](https://dazashu.github.io/Black-Souls-II-docs/pages/templates.html) | Walkthroughs of the 5 starter templates |
| [Asset Extractor](https://dazashu.github.io/Black-Souls-II-docs/pages/asset-extractor.html) | Extracting and repacking `Game.rgss3a` |
| [How It Works](https://dazashu.github.io/Black-Souls-II-docs/pages/how-it-works.html) | Archive patching, Marshal injection, runtime eval |
| [Script Index](https://dazashu.github.io/Black-Souls-II-docs/pages/script-index.html) | Recon dump: all 224 BS2 scripts in load order |
| [Class Reference](https://dazashu.github.io/Black-Souls-II-docs/pages/class-reference.html) | Recon dump: every class/module mapped to its defining script |

The two recon files are also viewable as raw markdown on GitHub:

- [`recon/INDEX.md`](recon/INDEX.md) — script index
- [`recon/DOCUMENTATION.md`](recon/DOCUMENTATION.md) — class reference

These are auto-generated from `Game.rgss3a` by `recon.py` in the [Mod Loader](https://github.com/dazashu/Black-Souls-II-Mod-Loader) repo. The decompiled `.rb` source files themselves are **not** redistributed — run `recon.py` against your own copy of the game to produce them.

---

## Folder Layout

```
Black-Souls-II-docs/
├── README.md
├── _config.yml          disables Jekyll preprocessing
├── index.html           landing page (tile grid)
├── style.css            dark-fantasy theme
├── pages/
│   ├── installation.html
│   ├── creating-mods.html
│   ├── asset-overrides.html
│   ├── api-reference.html
│   ├── templates.html
│   ├── asset-extractor.html
│   ├── how-it-works.html
│   ├── script-index.html      ── client-side renders recon/INDEX.md
│   └── class-reference.html   ── client-side renders recon/DOCUMENTATION.md
└── recon/
    ├── INDEX.md             auto-generated script catalog
    └── DOCUMENTATION.md     auto-generated class/method reference
```

---

## Hosting on GitHub Pages

1. Go to **Settings → Pages**.
2. **Source**: Deploy from a branch.
3. **Branch**: `main`, folder `/ (root)`.
4. Save.

Your site goes live at `https://<your-username>.github.io/Black-Souls-II-docs/` within a minute or two.

`_config.yml` disables Jekyll so the HTML is served as-is — no build step.

---

## Local preview

Just open `index.html` in a browser. There's no build pipeline; everything is plain HTML + CSS.

---

## License

MIT.
