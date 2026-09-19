# Sea Slug

![Sea Slug — a soft pastel Obsidian theme; illustrative notes UI](assets/sea-slug-social.png)

Soft colors, flexible callouts, and styled Bases. A practical remix of [Chime](https://github.com/Bluemoondragon07/chime-theme) for Obsidian 1.13+. [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) is recommended.

## Differences from Chime

- Updated for current Obsidian layouts, callouts, and plugins.
- Adds inactive-pane dimming, hover-expanding ribbon, dark-mode media dimming, list and outline threading, seamless embeds, and banners.
- Builds in list grids/cards, tree lists, floating and multi-column callouts, alternate checkboxes, and priority tags.
- Adds styling for Bases, Commander, Calendar, and Kanban.
- Removes Chime's legacy layouts, background images, `wiki-page`, `novel`, outdated color schemes, Page Gallery, and other obsolete plugin rules.
- Everything else is labeled under `Obsidian Settings → Style Settings → Sea Slug`.

## Styling Guide

`mailbox-cards` adds airmail-style Bases cards. `musicshelf` adds record sleeves; `pokemonbox` is the existing collection-card class. `no-fade` keeps Bases cards fully opaque.

- Preview static note pages [here](https://share.note.sx/93dfz98e). 
- Preview the available color schemes [here](/palettes).

### Page Classes

Add these under the note's `cssclasses` property.

| Use      | Classes                                                                                  |
| -------- | ---------------------------------------------------------------------------------------- |
| Width    | `width-800`, `width-900`, `width-1000`, `width-1200`, `width-1600`             |
| Cleanup  | `no-backlinks`, `no-count`, `no-fold`, `clean-embed`                             |
| Banners  | `banner`, `banner-fade`                                                              |
| Bases    | `no-head`, `case-card`, `center-card`, `oneline`, `no-fade`, `mailbox-cards`, `pokemonbox`, `musicshelf` |
| Text     | `colorful-headings`, `colorful-headings-alt`, `underlined-highlight`               |
| Headings | `h1-center`–`h6-center`, `h1-bottom-border`–`h6-bottom-border`                 |

`aside-left` and `aside-right` are HTML element classes for margin notes, not page classes.

### Banners & Images

```yaml
---
cssclasses: [banner, banner-fade]
---
```

```markdown
![[image.jpg|banner]]
```

Image aliases also support `center` and `right`.

### Lists

| Tag                | Result                    |
| ------------------ | ------------------------- |
| `#mcl/list-grid` | Column grid               |
| `#mcl/list-card` | Card grid                 |
| `#tree-view`     | Collapsible threaded tree |

Put the tag inside the list. It is hidden in Reading view.

### Callouts

```markdown
> [!issue] Issue
> What legal question must be resolved?

> [!note|float-right-small] Small floating note
> Text wraps around it.

> [!lucide-scale|custom-icon purple] Custom icon
> Omit the color metadata to use the purple default.
```

| Group        | Types or metadata                                                                                                 |
| ------------ | ----------------------------------------------------------------------------------------------------------------- |
| Legal        | `facts`, `posture`, `issue`, `rule`, `analysis`, `conclusion`, `concurrence`, `dissent`                           |
| Other types  | `email`, `conversation`, `conversation-outline`, `conversation-minimalist`, `timeline`, `polaroid` |
| Custom icon  | `[!lucide-icon\|custom-icon]`; add a color after `custom-icon` when needed                                        |
| Layout types | `blank`, `multi-column`                                                                                           |
| Colors       | `gray`, `brown`, `red`, `orange`, `yellow`, `green`, `cyan`, `blue`, `purple`, `pink`                             |
| Cleanup      | `no-bg`, `no-background`, `no-icon`, `no-title`, `blank`, `wide`, `black-and-white`, `b-w`                        |
| Floats       | `left`, `right`, `float-left`, `float-right`; sized forms: `float-left-small` / `float-right-small` (also `medium`, `large`)                                |
| Timeline     | `horizontal`, `numbered`, `skip`                                                                                  |
| Email        | `sep`                                                                                                             |

### Checkboxes


| Marker | Meaning     | Marker | Meaning   | Tag             | Meaning         |
| ------ | ----------- | ------ | --------- | --------------- | --------------- |
| `/`    | Incomplete  | `-`    | Canceled  | `#A`            | High priority   |
| `>`    | Forwarded   | `<`    | Scheduled | `#B`            | Medium priority |
| `?`    | Question    | `!`    | Important | `#C`            | Low priority    |
| `*`    | Star        | `“`    | Quote     | `#rsvp`         | Recurring       |
| `l`    | Location    | `b`    | Bookmark  | `#show`         | Event           |
| `i`    | Information | `I`    | Idea      | `#productivity` | Productivity    |
| `S`    | Savings     | `p`    | Pro       |                 |                 |
| `c`    | Con         | `f`    | Fire      |                 |                 |
| `k`    | Key         | `w`    | Win       |                 |                 |
| `u`    | Up          | `d`    | Down      |                 |                 |
| `R`    | Rule        | `m`    | ???       |                 |                 |

## Installation

1. Install and enable [BRAT](https://github.com/TfTHacker/obsidian42-brat).
2. Choose `Add a beta theme` and enter `https://github.com/t-if/gastrodon`.
3. Select `Sea Slug` under `Settings → Appearance → Themes`.

BRAT uses `theme-beta.css`. `theme.css` has the same features with my personal defaults.

## Credits & License

Based on [Chime](https://github.com/Bluemoondragon07/chime-theme), with adapted work from [MCL Multi Column](https://github.com/efemkay), [Obsidian Banner Snippet](https://github.com/HandaArchitect/obsidian-banner-snippet), [Fancy-a-Story](https://elsatam.github.io/obsidian-fancy-a-story/), [Minimal](https://github.com/kepano/obsidian-minimal), [r-u-s-h-i-k-e-s-h&#39;s snippets](https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets), [Maple](https://github.com/subframe7536/obsidian-theme-maple), and [Adrenaline](https://github.com/Spekulucius/obsidian-adrenaline). Source comments contain detailed attribution.

Licensed under [GPL-3.0-or-later](LICENSE).