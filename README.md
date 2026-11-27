# Nocturne Add-On Library

Official community and studio add-on repository for **Nocturne Lyrics DAW**, featuring custom UI color themes and downloadable language/slang packs.

---

## 🎨 Included UI Themes

**20 dark themes** to match your writing mood.

| Theme Name | Accent Style | Accent Color | File |
| :--- | :--- | :--- | :--- |
| **Arctic Frost** | Ice Blue | `#93C5FD` | `Arctic Frost.json` |
| **Aurora Borealis** | Teal / Cyan | `#2DD4BF` | `Aurora Borealis.json` |
| **Champagne Gold** | Warm Gold | `#D4AF6A` | `Champagne Gold.json` |
| **Deep Ocean** | Cobalt Blue | `#3B82F6` | `Deep Ocean.json` |
| **Electric Lime** | Neon Lime | `#A3E635` | `Electric Lime.json` |
| **Holographic Iris** | Periwinkle | `#A5B4FC` | `Holographic Iris.json` |
| **Indigo Nightfall** | Deep Indigo | `#6366F1` | `Indigo Nightfall.json` |
| **Lavender Haze** | Soft Violet | `#C4A7E7` | `Lavender Haze.json` |
| **Lemon Haze** | Lemon Yellow | `#FDE047` | `Lemon Haze.json` |
| **Matcha Lofi** | Sage Green | `#A3C76D` | `Matcha Lofi.json` |
| **Mint Breeze** | Fresh Mint | `#86EFC9` | `Mint Breeze.json` |
| **Mocha Velvet** | Warm Espresso | `#C8956D` | `Mocha Velvet.json` |
| **Monochrome Noir** | Stealth Silver | `#D4D4D8` | `Monochrome Noir.json` |
| **Neon Synthwave** | Electric Magenta | `#E040FB` | `Neon Synthwave.json` |
| **Peach Soda** | Soft Peach | `#FDBA8C` | `Peach Soda.json` |
| **Prism Carnival** ✨ | Rainbow Multicolor | `#FF5CA8` + gradient | `Prism Carnival.json` |
| **Rose Gold Reverie** | Rose Gold | `#E8A598` | `Rose Gold Reverie.json` |
| **Ruby Noir** | Ruby Red | `#E5484D` | `Ruby Noir.json` |
| **Sakura Dusk** | Soft Pink | `#F472B6` | `Sakura Dusk.json` |
| **Sunset Cassette** | Retro Orange | `#FF7A45` | `Sunset Cassette.json` |

### ✨ Special: Prism Carnival

A multicolor theme: pink accent, orange hover, violet soft highlight and cyan border on a deep violet background. It also includes an optional `accent_gradient` key:

```css
linear-gradient(135deg, #FF5CA8 0%, #FFB84D 25%, #FDE047 45%, #4ADE80 65%, #22D3EE 82%, #A78BFA 100%)
```

> The gradient only appears if the app supports `accent_gradient`.

---

## 🚀 How to Install in Nocturne

1. Open **Nocturne** and click **`+add-ons`** in the top bar.
2. Switch to the **`🎨 App Themes`** tab.
3. Ensure the repository field is set to:
   ```text
   muhdrasydan99/nocturne-addon-lib
   ```

---

## 🧩 Theme File Format

Each theme is a single JSON file. Example (`Sakura Dusk.json`):

```json
{
  "id": "sakura",
  "name": "Sakura Dusk",
  "bg_base": "#0F0A0E",
  "bg_surface": "#191117",
  "bg_elevated": "#231821",
  "border": "#32222F",
  "accent": "#F472B6",
  "accent_hover": "#F9A8D4",
  "accent_soft": "rgba(244, 114, 182, 0.16)",
  "accent_border": "rgba(244, 114, 182, 0.45)"
}
```

| Key | Description |
| :--- | :--- |
| `id` | Unique theme identifier |
| `name` | Theme display name |
| `bg_base` | Base background color |
| `bg_surface` | Surface background color |
| `bg_elevated` | Elevated background color |
| `border` | Border color |
| `accent` | Main accent color |
| `accent_hover` | Accent color on hover |
| `accent_soft` | Accent at 16% opacity |
| `accent_border` | Accent at 45% opacity |
| `accent_gradient` | Optional CSS gradient (used by Prism Carnival) |

---

## 🤝 Contributing a Theme

1. Copy an existing theme file and rename it to match your theme name.
2. Give it a unique `id` and `name`.
3. Update the colors. `accent_soft` and `accent_border` should use the same RGB color as `accent` (multicolor themes such as Prism Carnival are an exception).
4. Check that text stays readable on your background and accent colors.
5. Add your theme to the table above, then open a pull request.
