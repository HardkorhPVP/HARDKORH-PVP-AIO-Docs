# Header visual manifest

Developer reference for the decorative page headers. It is excluded from the built site (`_config.yml` → `exclude`).

Every documentation page has its own header composition: one illustration crop, masked into the right side of the page title
card. This file records each composition so that no two pages end up with the same header. Before adding or changing a header,
pick a source region or focal subject that is not already listed here, then re-run the header uniqueness check.

## Rules

- Illustrations are decorative brand atmosphere only. They never show gameplay, game UI or HARDKORH data.
- The 18 real screenshots in `assets/images/screenshots/` are the only evidence of HARDKORH behaviour. They are never filtered,
  overlaid, recoloured or used as header art.
- Header art lives in CSS backgrounds. It never sits behind body text, tables, code or screenshots.
- Each page loads only its own header image.

## Source artwork

All masters are Microsoft Copilot illustrations kept outside the repository. Only the web derivatives listed below are committed.
C2PA content credentials, where a master carries them, are not carried into the web crops.

| Master | Size | Content |
| --- | --- | --- |
| HARDKORH logo poster | 1672 × 941 | Panthers, moon, forest, waterfalls, fortress, banners, rune stone, braziers. All crops avoid the poster's lettering. |
| HARDKORH arena master | 1536 × 1024 | Night-time stone PvP arena: towers, crest, portcullis gate, torches, banners, open floor, entry stairs. No text, no UI. |
| HARDKORH roadmap artwork A | 1672 × 941 | Roadmap poster: Moonkin under a full moon, hilltop temple, night forest. Crops use only the illustrated margins: never the lettering, the roadmap table or the side panels. |
| HARDKORH roadmap artwork B | 1536 × 1024 | Roadmap poster: antlered Moonkin with a cosmic orb, crescent moon, druid with a roaring bear, standing stones, sunset sky. Crops use only the illustrated margins: never the lettering, the roadmap table, the side panels, the castle or the faction banners. |

## Treatment

- Card: `.hk-art .page__inner-wrap > header` (9.5rem tall; restrained pages with `hk-art--quiet` are 7rem).
- Art box: `header::before`, right-anchored, `background-size: cover`, box width capped at 1.12 × the crop's native width.
- Masks: **standard** = transparent → 55% at 35% → opaque at 75%; **narrow** (box < 36%) = transparent → opaque over the first 40%.
- Phone (≤ 600px): box width at least 46%, opacity × 0.72, quiet card 6rem.
- Classes are assigned per page in `_config.yml` → `defaults` (`hk-hdr--<page>`); values live in `assets/css/main.scss`.

## Pages

Region = crop box in master pixels (x, y, width × height). "Screenshots" = distinct real screenshots shown on the page.

| Page | Family | Asset | Source region | Box (cap) | Position | Opacity | Mask | Card | Unique visual ID | Screenshots | Illustration |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Home (hero) | Feral | `art/hk-art-feral.webp` + `brand/hardkorh-wordmark-large.webp` | poster 230, 0, 1442 × 330 | hero band 330px | 50% 0 / auto 100% | 1 | side + bottom fade | hero | HOME-PANTHER-MOON | 1 | yes |
| Requirements | Getting Started | `art/headers/hdr-requirements.webp` | poster 0, 540, 262 × 160 | 40% (293px) | 50% 50% | 0.7 | standard | quiet | GS-RUNE-STONE | 0 | yes |
| Installation | Getting Started | `art/headers/hdr-installation.webp` | poster 1420, 770, 252 × 171 | 40% (282px) | 50% 60% | 0.75 | standard | quiet | GS-FORGE-RACK | 1 | yes |
| First Launch | Getting Started (arena) | `art/headers/hdr-first-launch.webp` | arena 360, 760, 820 × 264 (saved 615 × 198) | 50% (689px) | 50% 45% | 0.7 | standard | quiet | GS-ARENA-ENTRY-STAIRS | 1 | yes |
| Keybinds | Getting Started | `art/headers/hdr-keybinds.webp` | poster 20, 650, 220 × 130 | 34% (246px) | 35% 50% | 0.6 | narrow | quiet | GS-PAW-RUNE | 1 | yes |
| Settings | HARDKORH | `art/headers/hdr-settings.webp` | poster 590, 692, 190 × 156 | 30% (213px) | 50% 45% | 0.55 | narrow | quiet | HK-THORN-VINES | 5 | yes |
| KORHVISION | HARDKORH (Feral) | `art/headers/hdr-korhvision.webp` | poster 0, 40, 340 × 265 | 56% (381px) | 50% 65% | 0.75 | standard | full | HK-STALKER-EYES | 3 | yes |
| KORHSIGHT | HARDKORH (arena) | `art/headers/hdr-korhsight.webp` | arena 330, 40, 880 × 290 (saved 660 × 218) | 60% (739px) | 50% 50% | 0.7 | standard | full | HK-ARENA-TOWERS-CREST | 1 | yes |
| KORHTRAP | HARDKORH (arena) | `art/headers/hdr-korhtrap.webp` | arena 700, 240, 410 × 420 (saved 308 × 315) | 40% (345px) | 50% 40% | 0.7 | standard | full | HK-ARENA-PORTCULLIS | 4 | yes |
| KORHSHIELD | HARDKORH (Feral) | `art/headers/hdr-korhshield.webp` | poster 440, 0, 300 × 335 | 48% (336px) | 50% 60% | 0.65 | standard | full | HK-MOON-CLAWS | 2 | yes |
| Arena Burst | HARDKORH (arena) | `art/headers/hdr-arena-burst.webp` | arena 470, 560, 780 × 340 (saved 585 × 255) | 58% (655px) | 50% 50% | 0.75 | standard | full | HK-ARENA-FLOOR-CENTRELINE | 1 | yes |
| Required Talents | Feral Druid | `art/headers/hdr-required-talents.webp` | poster 640, 0, 480 × 330 | 64% (538px) | 50% 40% | 0.75 | standard | full | FD-PANTHER-FACE | 1 | yes |
| Gear & Stats | Feral Druid | `art/headers/hdr-gear-and-stats.webp` | poster 1460, 640, 190 × 225 | 30% (213px) | 50% 25% | 0.75 | narrow | full | FD-HERALDIC-BANNER | 0 | yes |
| Arena & Solo Shuffle | Feral Druid (arena, canonical) | `art/hk-art-arena.webp` | arena full frame 1536 × 1024 (saved 1200 × 800) | 76% (1344px) | 50% 52% | 0.8 | standard | full | FD-ARENA-PANORAMA | 0 | yes |
| Battlegrounds | Feral Druid | `art/headers/hdr-battlegrounds.webp` | poster 1252, 570, 298 × 371 | 46% (334px) | 50% 12% | 0.75 | standard | full | FD-FORTRESS-FALLS | 0 | yes |
| PvE | Feral Druid | `art/headers/hdr-pve.webp` | poster 232, 330, 158 × 611 | 25% (177px) | 50% 42% | 0.6 | narrow | quiet | FD-WATERFALL-GORGE | 0 | yes |
| Troubleshooting | Support | `art/headers/hdr-troubleshooting.webp` | poster 20, 720, 230 × 221 | 36% (258px) | 50% 35% | 0.6 | standard | quiet | SU-BRAZIER-AMBER | 0 | yes |
| FAQ | Support | `art/headers/hdr-faq.webp` | poster 330, 40, 150 × 270 | 24% (168px) | 50% 50% | 0.7 | narrow | quiet | SU-RUNE-BANNER | 0 | yes |
| Changelog | Support | `art/headers/hdr-changelog.webp` | poster 760, 692, 160 × 158 | 26% (179px) | 50% 50% | 0.6 | narrow | quiet | SU-ENGRAVED-MEDALLION | 0 | yes |
| 404 | Feral | `art/headers/hdr-404.webp` | poster 1300, 25, 260 × 260 | 42% (291px) | 50% 40% | 0.7 | standard | full | 404-SPECTRAL-PANTHER | 0 | yes |
| Platform Overview | HARDKORH Platform | `art/headers/hdr-platform.webp` | roadmap B 262, 662, 178 × 268 | 40% (199px) | 50% 55% | 0.7 | standard | full | PL-STANDING-STONES | 0 | yes |
| Roadmap | HARDKORH Platform | `art/headers/hdr-roadmap.webp` | roadmap B 1098, 405, 172 × 195 | 40% (193px) | 50% 50% | 0.75 | standard | full | PL-WING-SUNSET | 0 | yes |
| Balance Overview | Balance Druid | `art/headers/hdr-balance.webp` | roadmap B 1250, 104, 206 × 196 | 46% (231px) | 50% 35% | 0.8 | standard | full | BD-ANTLERED-MOONKIN | 0 | yes |
| Balance KORHTHINK | Balance Druid | `art/headers/hdr-balance-korhthink.webp` | roadmap A 368, 0, 160 × 172 | 38% (179px) | 50% 40% | 0.75 | standard | full | BD-MOON-TEMPLE | 0 | yes |
| Balance Eclipse & Burst | Balance Druid | `art/headers/hdr-balance-eclipse.webp` | roadmap B 348, 0, 152 × 144 | 36% (170px) | 50% 50% | 0.8 | standard | full | BD-CRESCENT-MOON | 0 | yes |
| Balance Control & KORHKICK | Balance Druid | `art/headers/hdr-balance-control.webp` | roadmap B 1104, 215, 146 × 180 | 34% (164px) | 50% 45% | 0.75 | narrow | full | BD-COSMIC-VORTEX | 0 | yes |
| Balance KORHSHIELD | Balance Druid | `art/headers/hdr-balance-korhshield.webp` | roadmap B 150, 146, 285 × 158 | 52% (319px) | 50% 40% | 0.7 | standard | full | BD-ROARING-BEAR | 0 | yes |
| Balance KORHVISION | Balance Druid | `art/headers/hdr-balance-korhvision.webp` | roadmap B 200, 304, 145 × 102 | 30% (162px) | 50% 45% | 0.7 | narrow | quiet | BD-DRUID-GLOWING-EYE | 0 | yes |
| Balance Settings | Balance Druid | `art/headers/hdr-balance-settings.webp` | roadmap B 1040, 0, 148 × 100 | 28% (166px) | 50% 50% | 0.72 | narrow | quiet | BD-STARLIT-PINIONS | 0 | yes |
| Balance Scope & Limits | Balance Druid | `art/headers/hdr-balance-scope.webp` | roadmap A 1138, 0, 320 × 112 | 44% (358px) | 50% 50% | 0.6 | standard | quiet | BD-NIGHT-CANOPY | 0 | yes |

No two roadmap-artwork regions overlap. The Feral system pages keep their original headers and addresses; the sidebar now lists them
under Feral Druid.

All assets are under `assets/images/`.

## Uniqueness check (Phase 1.2, 1440px)

- 19 of 19 pages render a major header (at least 140px tall) and every header image loads.
- 19 unique treatment combinations (asset, position, size, box width, opacity, mask) and 19 different source assets.
- Every header capture is byte-unique, with and without the page title.
- Perceptual distance (mean absolute RGB difference of a 48 × 16 signature, title hidden): whole card closest pair 3.7
  (PvE / FAQ), median 13.7. Art zone only (right 40% of the card): closest pair 8.1 (Settings / FAQ), median 19.1. The closest
  pairs are restrained pages whose dark cards share most of their area, but their subjects are different (waterfall gorge,
  rune banner, thorn vines, medallion, rune stone).

## Uniqueness check (Balance and platform pages, 1440px)

- 29 of 29 pages render a major header (at least 140px tall) and every header image loads.
- 29 unique treatment combinations and 29 different source assets; every header capture is byte-unique, with and without the
  page title.
- Whole card: closest pair still 3.7 (PvE / FAQ), median 14.2. Art zone only: closest pair 8.0 (FAQ / Balance Settings, after
  raising Balance Settings from 0.6 to 0.72 opacity; 7.2 before), median 21.0. The two are a rune banner and a starlit wing.
