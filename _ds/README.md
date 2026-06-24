# Maccabi Ofek — Design System

> תוכנית פיתוח מנהלי יחידות · 2026
> Internal management-development program for **מכבי שירותי בריאות**, run in partnership with **NGG** consulting.

---

## What this is

A design system that captures the visual + verbal language of **"אופק" (Ofek — "Horizon")**, Maccabi's executive development program. The program is delivered as a structured **seven-meeting journey** with paired **"מפגש ממונים"** (supervisor meeting) decks that brief the participants' direct managers between modules.

The system is built so design agents can produce on-brand artifacts — slides, handouts, internal interfaces, supervisor communications, certificates — without re-deriving the brand each time.

## Products / surfaces represented

| Surface | What it is |
|---|---|
| **Participant decks** (`מפגש 01–07`) | The seven training-module slide decks delivered live to participants. Heavy use of models (DISC, GROWTH, North-Star), iconography, horizon/journey metaphor. |
| **Supervisor decks** (`מפגש ממונים`) | Two shorter decks delivered to the participants' bosses, briefing them on what their report just learned + how to coach them between modules. The two source decks for this system. |
| **"אופק PLAY" video sub-brand** | A video micro-learning library used between meetings. Has its own sub-mark — a circular "play" symbol, a colored `PL<Y` wordmark, tagline *"ללמוד · להתעדכן · להתחדש"*. |
| **Homework cards** ("פינוקי בית") | Take-home assignments between modules — presented in a pink-framed card on the right side of the supervisor decks. |

## Sources used

All visual decisions were derived from artifacts the user uploaded:

- `uploads/מפגש ממונים 2 אופק 2026.pptx` → `extracted/deck1/` (13 slides, 54 media files, full theme).
- `uploads/סיכום לממונים - אופק.pptx` → `extracted/deck2/` (6 slides, canonical color stripe + Maccabi logo).
- `uploads/לוגו NGG-02.png` → NGG partner logo → `assets/ngg-logo.png`.
- `uploads/Ploni-{Ultralight,Regular,Medium,Demibold}-AAA.ttf` → official Hebrew typeface → `fonts/`.

> **Note on missing sources.** The original brief referenced `אופק.zip`, `מפגש ממונים 1 אופק 2026.pptx`, and `אופק מפגש 2- תקשורת בינאישית 2026.pptx`, but only the two supervisor decks above arrived. Conclusions are based on what was available. Re-attaching the missing files would sharpen this further — especially the iconography and section-divider rules.

---

## Content fundamentals

### Brand voice — calm, respectful, practical, model-driven

The register is closer to an **HR / L&D professional briefing supervisors** than to a marketing site. Warm but measured, never breezy, never flashy.

**Defining traits**
- **Direct plural address to supervisors** (`אתם`, `שאלו`, `חשבו`, `תכננו`) — they are partners in the learning, not an audience.
- **Sentence shape: imperative → context → outcome.** *"שאלו את המנהל מהו הכיוון הניהולי שאתה רוצה לחזק בתקופה הקרובה, ומה הפער המרכזי שאתה מזהה כיום?"*
- **Named models in Latin inline with Hebrew** — `GROWTH`, `DISC`, `GTD`, `PL<Y`. Magenta in titles, plain ink in body.
- **Numbered modules.** Always `מפגש 01 / 02 / …` with a leading zero. Never `שיעור 1` or just `1`.
- **Light bureaucracy.** *"כדי ליישם את הלמידה, המשתתפים התבקשו: …"* — passive construction to keep authority neutral.
- **No exclamation pile-ups, no emoji, no slang.** The closing slide says simply *"תודה"*.

**Casing.** Hebrew has no case. For Latin terms: **Title-case acronyms** (`DISC`, `GROWTH`, `GTD`) — never all-caps shouting, never lowercase.

**Quoted program vocabulary.** Don't translate these — they're the program's signature terms:
- *"מצפן ניהולי"* — managerial compass
- *"מכירת השינוי"* — selling the change
- *"כוכב הצפון"* — north-star
- *"תפיסת התפקיד הניהולי"* — the program's central concept

**Recurring section labels worth knowing**
- *"בין המפגשים — מבט לאופק"* — between-meetings header (plays on *"horizon"*).
- *"פינוקי בית"* — homework / take-home. Affectionate but professional.
- *"מה הלאה?"* — closing question on every supervisor deck.
- *"כיווני פעולה להמשך"* — action directions for what's next.

See `preview/voice-and-tone.html` for DO / DON'T copy examples.

---

## Visual foundations

### In one paragraph

**Calm corporate-instructional, not digital-startup.** A primary deep navy carries authority and structure; a single magenta accent does almost all emphasis work; six secondary colors handle category-coding (modules, chart series, decorative stripes) and otherwise stay out of the way. Lots of white space. Big confident Hebrew headings in Ploni Demibold. Soft cream + sky-blue gradients. Hand-photographed horizon imagery (cactus, hills, sunrise) used as a recurring metaphor for *"אופק"* / horizon. Curved organic crops on photography. Thin **3px magenta "frames"** for video & homework cards. A **six-color band along the bottom** of every slide.

### Colors

| Token | Hex | Role |
|---|---|---|
| `--ofek-navy-900` | `#040450` | Deepest navy. Title-slide ink, gradient anchor. |
| `--ofek-navy-700` | `#1E3C95` | **Primary brand.** Sidebar fill, section headers, primary CTAs. |
| `--ofek-navy-500` | `#2B92B7` | Secondary teal. Chart highlights, secondary links. |
| `--ofek-magenta-700` | `#D25089` | **Primary accent.** Pink frames, icon badges, emphasis runs in titles. |
| `--ofek-magenta-900` | `#AD2185` | Deeper magenta — hover on accent. |
| `--ofek-magenta-300` | `#F1B4CE` | Powder — soft backgrounds, on-dark accent text. |
| `--ofek-blush-500` | `#DEAFB7` | **Large-area panel fill.** Dusty rose paired with navy on "הפסקה" / break / "מבט לאופק" slides. A 30/70 or 40/60 split with navy is canonical. |
| `--ofek-blush-300` / `100` | `#ECCAD0` / `#F6E4E7` | Lighter blush variants for secondary panels & soft backgrounds. |
| Categorical | `#6B76EC` lavender · `#73D9F0` cyan · `#A7C86F` green · `#F9BE94` peach · `#F1717E` coral · `#D25089` magenta | The **fixed-order** six-step stripe. Each module owns one color. |
| `--ofek-ink` | `#171616` | Body ink. |
| `--ofek-gray-700/500/300/100` | `#535353` / `#808285` / `#C9CACC` / `#F3F4F6` | Neutral scale. |
| `--bg-soft` | `#F4F1ED` | Warm cream — the recurring slide background tint. |

**Rule of thumb.** A given slide uses **at most three** of these: a neutral (background), navy (chrome/headings), magenta (emphasis). The categorical six appear only as the bottom-of-slide stripe or to color-code modules — they're decorative, never used to color body content.

### Typography

**Ploni AAA (Fontef)** — Hebrew + Latin sans, four weights:
- **200 Ultralight** — sparingly, for very large display set above 60px.
- **400 Regular** — body copy, lists, secondary text.
- **500 Medium** — UI elements, eyebrow labels, list items, callouts.
- **600 Demibold** — all headings, display, button labels, branded numerals.

Hierarchy is built with **weight + size**, never all-caps. Letter-spacing is near-zero in body and slightly tightened (`-0.01em`) on display sizes. Numerals always lining; module numbers always two-digit padded.

### Spacing & layout

- **4-grid spacing scale** (`--space-1` 4px → `--space-9` 96px).
- **Wide outer margins** on slides — typically `60–90px` from edges before any content. The white space is part of the brand.
- **Asymmetric two-column layouts** are signature: a narrow dark-navy sidebar (~36%) on one side, wide cream content area on the other.
- **Bottom 10–14px reserved** for the color stripe on every slide.

### Corner radii

Medium-soft — not sharp, not pillowy. Signature pink-framed cards use `~18–22px`. Buttons and chips are full pills. Avatars and category badges are full circles.

`r-xs` 4 · `r-sm` 8 · `r-md` 14 · `r-lg` 22 · `r-xl` 32 · `r-pill` 999.

### Elevation

**Shadows are used sparingly.** Most surfaces are flat — separation comes from the **3px magenta border** ("pink frame") or from the **navy background panel**, not from depth cues. When shadows appear they are very soft, low-opacity, and blue-tinted (`rgba(20,24,60,…)`) rather than neutral black.

### Backgrounds & imagery

Three recurring background treatments:
1. **Warm cream gradient** (`#FFFFFF → #F4F1ED`) — standard content slides.
2. **Soft sky gradient** (`#DCE3EE → #F3EFE8`) — content-heavy slides, gives a "morning light" feel.
3. **Deep navy gradient** (`#1E3C95 → #040450`) — title, section, and thank-you slides only.

**Photography style.** Real, slightly desaturated, warm. Recurring subjects: **horizon/landscape** (cactus in desert, rolling hills, sunrise), **abstract tactile objects** (wooden-peg figures as leadership/team metaphor), **documentary workshop photos**. The horizon metaphor is *the* visual anchor — it's the program's name.

**Photo crops.** Photos are placed inside **organic asymmetric arcs** — half-ellipses, large arc clips. They are almost never rectangular.

### Borders & frames

- **The 3px magenta border** is the signature container. Wraps videos, homework cards, action prompts.
- **Inner shadows** are never used.
- **Capsule (pill) shapes** for any badge containing a number, status, or category — and for buttons.

### Motion

Very restrained. The source decks read as **printed PDF** more than digital. Use motion only for:
- **Cross-fade slide transitions** (≤300ms).
- **Reveal-on-build** for lists and the GROWTH model letters (left-to-right or right-to-left, 80ms stagger).
- **Never use bounce, never use elastic curves.** Standard CSS `ease-out` (`cubic-bezier(.2, .8, .25, 1)`) covers ~everything.

### The signature elements (memorize these)

1. **Six-color bottom stripe** — `lavender / cyan / green / peach / coral / magenta`, 10–14px tall, full slide width, fixed order. Appears on every slide.
2. **Magenta circle icon badge** — a 46–80px filled magenta disc with a white line-icon, often sitting on the upper edge of a pink-framed card.
3. **Navy sidebar with white headline + cream body area** — the canonical content-slide layout. Sidebar is ~36% wide.
4. **The "אופק PLAY" lockup** — circle + `PL<Y` wordmark + horizon photo background.
5. **3px-magenta-bordered "pink frame"** — for video thumbnails and homework cards.

---

## Iconography

The source decks use **outlined, single-weight line icons** at consistent ~2px stroke. Icons are flat-colored (no gradients, no fills), and are recolored per category:
- **Navy** (`#1E3C95`) for primary actions and modules in their "neutral" state.
- **Magenta** (`#D25089`) when sitting inside the signature magenta circle badge (then the icon is `white`) or for emphasis on cream backgrounds.
- **Category colors** when icons appear next to a category label in journey/legend layouts.

Subjects observed in the source decks:
- People / discussion bubbles / meeting icons (the most common — they appear on nearly every slide)
- Light bulb (ideation, insight)
- Compass / target / arrow (the "north-star" / "horizon" metaphor)
- Document / clipboard / checkmark (homework + tasks)
- Stopwatch / clock (time-bounded exercises)

If an exact icon isn't available, **use a placeholder rather than draw a new one** — drawing icons by hand will produce off-brand line-weight inconsistencies. The user has the full icon set in the participant decks; this system extracted only a representative sample to `assets/icons/`.

See `preview/iconography.html` for the icon recoloring matrix.

---

## How to use this system

1. **Always include `colors_and_type.css`** at the top of any HTML you produce:
   ```html
   <link rel="stylesheet" href="../colors_and_type.css" />
   ```
2. **For 16:9 slide-style artifacts**, also include `slides/slide-base.css` and use a `1280×720` `.stage` container with the `.stripe`, `.footer-logos`, `.sidebar` + `.main` patterns shown in `slides/03-content-sidebar.html`.
3. **Always set `<html lang="he" dir="rtl">`** for Hebrew content. Use `dir="ltr"` only for fully-English artifacts.
4. **Footer logos** — every slide-style artifact should include the Maccabi + NGG lockup in the bottom-right.
5. **Read `SKILL.md`** before producing new artifacts — it has the per-artifact patterns.

---

## File map

```
colors_and_type.css         ← canonical tokens. Always import.
SKILL.md                    ← per-artifact recipes (slides, supervisor briefs, video lockups).
fonts/                      ← Ploni AAA — four weights.
assets/                     ← brand logos, photography, icon library (.png from source decks).
  ngg-logo.png              ← NGG partner logo.
  maccabi-logo.png          ← Maccabi master brand (in deck footers).
  ngg-30th-logo.png         ← NGG 30-years anniversary mark.
  cactus-horizon.jpeg       ← the canonical horizon photo (cactus + sunrise).
  hills-illustration.jpeg   ← abstract landscape illustration.
  wooden-pegs-leadership.png← tactile leadership/team metaphor.
  soft-gradient-bg.jpeg     ← the cream/sky background tint.
  color-stripe-vertical.png ← the 6-color stripe (vertical orientation).
  icons/                    ← line icon samples.
preview/                    ← review-pane swatches & component specs.
slides/                     ← slide patterns + 7 sample slides demonstrating the system.
  slide-base.css            ← .stage / .stripe / .sidebar / .pink-frame patterns.
  01-title.html             ← deep navy hero, 120px display.
  02-section-divider.html   ← cream + magenta breadcrumbs.
  03-content-sidebar.html   ← the signature layout — navy sidebar + pink-framed video.
  04-program-journey.html   ← 7 modules as colored timeline.
  05-growth-model.html      ← six-letter coaching model.
  06-discussion.html        ← 3-up question cards with numbered badges.
  07-thank-you.html         ← navy closing with magenta accent.
  index.html                ← deck shell containing all 7 sample slides.
extracted/                  ← raw text + media extracted from the source PPTX files (reference only).
```

---

## Quick links — preview cards

**Type:** [family](preview/type-family.html) · [display](preview/type-display.html) · [body](preview/type-body.html) · [Hebrew + Latin](preview/type-mixed-script.html)
**Colors:** [primary navy](preview/color-primary-navy.html) · [accent magenta](preview/color-accent-magenta.html) · [categorical](preview/color-categorical.html) · [neutrals](preview/color-neutrals.html) · [semantic](preview/color-semantic.html)
**Spacing:** [scale](preview/spacing-scale.html) · [radii](preview/radii.html) · [elevation](preview/elevation.html) · [backgrounds](preview/backgrounds.html)
**Components:** [buttons](preview/components-buttons.html) · [badges](preview/components-badges.html) · [pink frame](preview/components-pink-frame.html) · [cards](preview/components-cards.html) · [sidebar block](preview/components-sidebar-block.html) · [magenta badge](preview/components-magenta-badge.html) · [journey](preview/components-journey.html) · [forms](preview/components-forms.html)
**Brand:** [logo lockup](preview/brand-logo-lockup.html) · [color stripe](preview/brand-color-stripe.html) · [iconography](preview/iconography.html) · [voice & tone](preview/voice-and-tone.html)
**Sample slides:** [01 Title](slides/01-title.html) · [02 Section](slides/02-section-divider.html) · [03 Content + sidebar](slides/03-content-sidebar.html) · [04 Journey](slides/04-program-journey.html) · [05 GROWTH](slides/05-growth-model.html) · [06 Discussion](slides/06-discussion.html) · [07 Thanks](slides/07-thank-you.html) · [Full deck](slides/index.html)
