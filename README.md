# Media Tracker starter

A minimal, ready-to-deploy site using the
[hugo-mediatracker-theme](https://github.com/christt105/hugo-mediatracker-theme).

**Demo:** https://christt105.github.io/mediatracker-starter/

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
for Obsidian: search TMDB, TheTVDB, IGDB or Steam and it creates a
theme-compatible note (cover, banner, metadata) for you. Point Obsidian at your
`content/` folder and your entries are ready to commit.

## Deploy

The included GitHub Actions workflow builds and deploys to GitHub Pages. Enable
Pages (Settings → Pages → Source: GitHub Actions) and push to `main`.
