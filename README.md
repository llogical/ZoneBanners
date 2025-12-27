# ZoneBanners (Ashita v4)

A lightweight addon that shows a **PNG zone banner** when you zone in.

- **No text fallback / no small zone label**
- PNGs live in `zonebanners/assets/zones/<zoneId>.png`
- Banner timing and placement are configurable via Ashita settings

## Demo

**Video:** (https://github.com/user-attachments/assets/9f0f3609-2e26-4974-97dd-7494a35626a0)

![ZoneBanners demo screenshot](docs/demo-thumb.png)


GitHub README files don’t reliably embed local `.mp4` files inline. The most reliable way is:

1. Open your repo on GitHub.
2. Create an **Issue** (or edit a comment on an existing issue).
3. Drag & drop `docs/zonebanners-demo.mp4` into the comment box.
4. GitHub uploads it and gives you a hosted URL like `https://github.com/<user>/<repo>/assets/...`
5. Paste that URL here in the README.

Example:

```md
## Demo Video
https://github.com/<user>/<repo>/assets/<...>
```

Optional “clickable thumbnail” style:

```md
[![ZoneBanners Demo](docs/demo-thumb.png)](https://github.com/<user>/<repo>/assets/<...>)
```

## Install (Ashita v4)

1. Copy the **`zonebanners`** folder into:

   `Ashita/addons/`

   You should end up with:

   `Ashita/addons/zonebanners/zonebanners.lua`  
   `Ashita/addons/zonebanners/assets/zones/1.png`  
   etc.

2. Load it in-game:

```txt
/addon load zonebanners
```

## Config

Settings are saved via Ashita’s `settings` library.

- `banner_delay` (seconds)
- `banner_fade_in` (seconds)
- `banner_hold` (seconds)
- `banner_fade_out` (seconds)
- `banner_y_frac` (0.0–1.0, fraction of screen height)
- `banner_scale` (1.0 = original PNG size)

## Making new banners

- Name your PNG by **zone ID** (e.g. `251.png`)
- Place it in: `zonebanners/assets/zones/`

## License

MIT (see `LICENSE`).
