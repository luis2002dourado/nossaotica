# DESIGN.md - Nossa Ótica (Tuntum & Presidente Dutra / MA)

## 1. Brand Brief & Visual Direction
- **Brand Name**: Nossa Ótica ("Ver bem é tradição" · "A visão de quem entende")
- **Surface Type**: High-Converting Optical Boutique Landing Page & Interactive Catalog (`@nossaotica_tuntumdutra`)
- **Aesthetic Direction**: Warm Obsidian Liquid-Glass Luxury & Editorial Optical Craft
- **Reference Lock**: Deep espresso-black surfaces inspired by actual store cabinetry (`#0a0806`), illuminated by warm golden LED display accents (`#d9ac47` / `#f6e3a1`), paired with tactile liquid-glass cards (`backdrop-filter: blur(22px)`).

## 2. Color Palette & Strict Semantic Roles
- **Primary Canvas (`--bg`)**: `#0a0806` (Deep Espresso Obsidian)
- **Elevated Canvas (`--bg-2`)**: `#0f0b07` (Warm Dark Onyx)
- **Liquid Glass Surface (`--panel`)**: `rgba(22, 17, 9, 0.58)` with `1px solid rgba(255, 255, 255, 0.13)` and top specular highlight `inset 0 1px 0 rgba(255, 255, 255, 0.22)`
- **Primary Text (`--cream`)**: `#f3ead6` (Warm Ivory Cream)
- **Secondary Text (`--dim`)**: `rgba(243, 234, 214, 0.72)`
- **Muted / Caption Text (`--faint`)**: `rgba(243, 234, 214, 0.48)`
- **Brand Gold Gradient (`--gold-1` -> `--gold-3`)**: `#f6e3a1` -> `#d9ac47` -> `#a97a1f` (Reserved strictly for Primary CTAs, Eyebrow Badges, and Display Highlights)
- **Live Store Open Status (`--emerald`)**: `#34d399` (Used strictly to indicate the Tuntum unit is open and operating)

## 3. Typography & Numeric Discipline
- **Display & Headings (`--font-serif`)**: `'Playfair Display', Georgia, serif` (`font-weight: 700-800`, `letter-spacing: -0.01em`, `text-wrap: balance`)
- **Body & UI Controls (`--font-sans`)**: `'Plus Jakarta Sans', 'Raleway', system-ui, sans-serif` (`font-weight: 400-600`, `text-wrap: pretty`)
- **Numeric Discipline**: `font-variant-numeric: tabular-nums` on all hours, phone numbers, counts, and metrics.

## 4. Component & Motion Architecture (Cult UI + Shader Gradient)
- **3D Shader Gradient Canvas**: Scoped `<canvas class="shader-gradient-canvas">` inside the Hero visual stage and Promo/Vision Life spotlight cards, rendering a 3D animated wave mesh in `#d9ac47`, `#f6e3a1`, and `#1a1206` with automatic offscreen pause (`IntersectionObserver`).
- **Direction-Aware Filter Tabs**: Interactive category switcher for the `@nossaotica_tuntumdutra` real product showcase (`Todos`, `Miu Miu & Italy`, `AT Eyewear`, `Solar Rimless`, `Lentes & Exame`).
- **Tactile CTA Hierarchy**: One primary gold shimmer CTA per card/section, paired with ghost glass secondary actions (`Ver no Instagram`, `Ver Rota`).
