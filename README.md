# Media Tracker starter

A minimal, ready-to-deploy site using the
[hugo-mediatracker-theme](https://github.com/christt105/hugo-mediatracker-theme).
**This is the best place to start** — clone it and you have a working media tracker.

**Demo:** https://christt105.github.io/mediatracker-starter/

## Media Tracker ecosystem

Part of a small ecosystem that turns your media library into a website:

- 🚀 **mediatracker-starter** — this repo: the ready-to-clone site. Start here.
- 🎨 **[hugo-mediatracker-theme](https://github.com/christt105/hugo-mediatracker-theme)** —
  the Hugo theme that renders the library (gallery, search, filters, stats, RSS).
- 📥 **[hugo-mediatracker-plugin](https://github.com/christt105/hugo-mediatracker-plugin)** —
  an Obsidian plugin that creates theme-compatible entries from TMDB, TheTVDB, IGDB,
  Steam and Open Library (see [Adding entries](#adding-entries)).

## Use it

1. Click **Use this template** on GitHub (or clone).
2. Install [Hugo extended](https://gohugo.io/installation/) and Go.
3. Run it:

   ```bash
   hugo server
   ```

4. Edit `hugo.toml` (title, author, baseURL) and add your own entries under
   `content/movies/`, `content/games/`, etc. Each entry is a folder with an
   `index.md`; drop a cover image in the folder and set `image: cover.jpg`.

Add a new media type by editing `data/media_types.yml` and adding a matching
menu entry. See the theme README for all options.

## Adding entries

You can write each `index.md` by hand, but the easiest way is the companion
[hugo-mediatracker-plugin](https://github.com/christt105/hugo-mediatracker-plugin)
for Obsidian: search TMDB, TheTVDB, IGDB, Steam or Open Library (books) and it
creates a theme-compatible note (cover, banner, metadata) for you. Point Obsidian at
your `content/` folder and your entries are ready to commit.

## Deploy

The included GitHub Actions workflow builds and deploys to GitHub Pages. Enable
Pages (Settings → Pages → Source: GitHub Actions) and push to `main`.
