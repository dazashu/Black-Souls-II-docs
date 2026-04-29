# Black Souls II - Documentation Site

Static HTML documentation for the [Black Souls II Mod Loader](https://github.com/dazashu/Black-Souls-II-Mod-Loader). Designed to be hosted on **GitHub Pages**.

🌐 **Live site: <https://dazashu.github.io/Black-Souls-II-docs/>**

## Companion repos

- 🔧 [Black-Souls-II-Mod-Loader](https://github.com/dazashu/Black-Souls-II-Mod-Loader) — runtime mod loader
- 🧩 [Black-Souls-II-Mod](https://github.com/dazashu/Black-Souls-II-Mod) — bundled mods (`creative_mode` + 5 starter templates)
- 📦 [Black-Souls-II-Asset-Extractor](https://github.com/dazashu/Black-Souls-II-Asset-Extractor) — extract / repack `Game.rgss3a`

---

## What's covered

| Page | Topic |
|---|---|
| [Installation](pages/installation.html) | Install the loader and run your first mod |
| [Creating Mods](pages/creating-mods.html) | `main.rb`, the mod loader API, common hooks |
| [Asset Overrides](pages/asset-overrides.html) | Drop-in PNG / OGG / data replacements |
| [API Reference](pages/api-reference.html) | `ModLoader.*` helpers and registered hooks |
| [Templates](pages/templates.html) | Walkthroughs of the 5 starter templates |
| [Asset Extractor](pages/asset-extractor.html) | Extracting and repacking `Game.rgss3a` |
| [How It Works](pages/how-it-works.html) | Archive patching, Marshal injection, runtime eval |

---

## Folder Layout

```
Black-Souls-II-docs/
├── README.md
├── _config.yml          disables Jekyll preprocessing
├── index.html           landing page (tile grid)
├── style.css            dark-fantasy theme
└── pages/
    ├── installation.html
    ├── creating-mods.html
    ├── asset-overrides.html
    ├── api-reference.html
    ├── templates.html
    ├── asset-extractor.html
    └── how-it-works.html
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
