# Glasshouse Theme

Refined dark glass for Home Assistant: a deep navy page with soft colour light, frosted cards, and one
accent colour per device type. It is the theme behind the **Glasshouse** card suite
([room](https://github.com/petergCA/glasshouse-room-card), [hero](https://github.com/petergCA/glasshouse-hero-card),
[stat](https://github.com/petergCA/glasshouse-stat-card)) and also styles Home Assistant's own cards to match.

## Install

1. In Home Assistant open **Marketplace** (HACS) → ⋮ → **Custom repositories**, add
   `https://github.com/petergCA/glasshouse-theme` with category **Theme**, then download it.
2. Make sure `configuration.yaml` loads themes:
   ```yaml
   frontend:
     themes: !include_dir_merge_named themes
   ```
3. Reload themes (**Developer tools → Actions → `frontend.reload_themes`**).
4. Pick **Glasshouse** for a single dashboard view (`theme: Glasshouse` on the view) or in your profile.

## What it sets

| Area | Values |
|---|---|
| Glasshouse tokens | `glasshouse-surface`, `-surface-2`, `-border`, `-blur`, `-radius`, `-text`, `-text-2`, `-text-3`, `-font` |
| Page | layered radial gradients on `#070b13`, translucent header |
| Cards | `rgba(255,255,255,0.045)` glass, 22px radius, hairline border |
| State colours | lights amber `#ffb547`, fans cyan `#4dd6e8`, covers periwinkle `#a3a8ff`, switches green `#7ee08a`, heat `#ff7a59`, cool `#58a6ff` |

Every Glasshouse card reads the `glasshouse-*` variables, so changing them here restyles the whole suite.

## License

MIT
