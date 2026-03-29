# Grad Research Project — Image Guide

## Usage Map

| File | Role | Where to Use | Notes |
|------|------|-------------|-------|
| `01_hero_reactive_astrocyte.jpeg` | Hero/Banner | Top of project page | Single GFAP+ astrocyte, visually stunning. Best image in the set. |
| `02_astrocyte_field_view.jpeg` | Supporting | About or gallery card | Wide field GFAP/DAPI tile scan, shows scale of experiments |
| `03_tbi_mechanism_diagram.png` | Context | Problem section | BioRender diagram: injury site, normal vs reactive astrocytes |
| `04_multichannel_fluorescence_results.png` | Key Result | Results section | 9-panel grid: Collagen IV / Laminin / GFAP across conditions and time points |
| `05_2d_vs_3d_gfap_comparison.png` | Result | Results section | 6-panel: 2D vs 3D GFAP at Day 2 and Day 5, shows morphology differences |
| `06_platform_engineering.jpg` | Engineering | Approach section | Plasma bonder + PDMS platform CAD exploded view with labels |
| `07_shear_modulus_results.png` | Quantitative | Results section | Bar charts: blast vs control shear modulus across time points |
| `08_ecm_architecture_illustration.png` | Context | Problem section or background | Neural ECM illustration (neurons, astrocytes, blood vessels) |
| `09_hydrogel_lab_photos.png` | Lab work | Approach section | Real photos: hydrogels in well plates + rheometer setup |

## Image Optimization Notes (for web)

Some of these are large (the fluorescence PNGs are 8-19 MB). Before deploying to the site:
- Resize to max 1600px wide for full-width images, 800px for inline
- Convert PNGs to WebP for ~80% size reduction while preserving quality
- Keep JPEGs as-is (already reasonable size)
- Consider lazy loading for images below the fold

## Skipped Images (not copied)

These remain in the project root if needed later:
- `Rheology figure.png` — too technical (rheometer schematic)
- `2D vs 3D GFAP .png` — statistical charts, less visual impact
- `Cell_Viability.jpg` — validation data, not portfolio material
- `Improved Rheometer Results.png` — method optimization detail
- `Laminin_CollagenIV_GFAP Expression.png/.jpg` — duplicate box plots, the fluorescence grid tells the story better
