\# {BRAND_NAME} - Claude Code Project Context

\## 🔧 Quick Customization Checklist

Before using this template, replace the following throughout this file:

\- \`{BRAND_NAME}\` → Your brand name

\- \`{BRAND_HANDLE}\` → Your social handle (e.g., "@acme.studio")

\- \`{BRAND_DOMAIN}\` → Your website

\- \`{BRAND_TAGLINE}\` → One-line description of your business

\- Color hex codes in the palette table → Replace with your brand colors

\- Font names in the typography section → Replace with your brand fonts

\- Voice rules in the Brand Voice Summary → Replace with your TOV rules

\- Language rules → Adjust language/locale rules to your audience

Then drop your own brand reference files into \`brand/\` and you're ready.

\---

\## About This Project

This project generates Instagram carousels for {BRAND_NAME} ({BRAND_DOMAIN}) - {BRAND_TAGLINE}.

\## Brand Knowledge (MUST READ before generating any content)

Always reference this file when writing or designing carousels:

\- \`brand/DESIGN.md\` - UI design system

\## Carousel Generation

Use the \`/carousel\` command to generate carousels.

See \`.claude/commands/carousel.md\` for the full pipeline.

\## Brand Voice Summary (for quick reference)

\> Replace this entire section with your own voice rules. Examples below - delete and rewrite for your brand:

\- {VOICE_PRINCIPLE_1} - e.g., "Practical authority - show, don't tell"

\- {VOICE_PRINCIPLE_2} - e.g., "Empathetic clarity - simplify without dumbing down"

\- {VOICE_PRINCIPLE_3} - e.g., "Action-forward - every post moves the reader toward doing"

\- Banned words (examples to delete/replace): "revolutionary", "game-changing", "best-in-class"

\- Language rules (if multilingual): which platforms get which language, code-mixing policy

\---

\## Visual Design System - {BRAND_NAME} Signature Carousel Style

\> The structure below is reusable - only the color hex codes and font names need to change for your brand.

{BRAND_NAME} carousels are editorial-bold, not editorial-quiet. Think: a strong dark hook that stops the scroll, light body slides that breathe, a signature accent color doing real work. Every carousel must feel unmistakably {BRAND_NAME}.

\### Brand Color Palette

\> Replace these hex codes with your own brand colors. Keep the role names (Primary dark, Signature accent, etc.) - the renderer maps them automatically.

| Role | Color Name | Hex | Usage |

|---|---|---|---|

| Primary dark | {YOUR_DARK_NAME} | \`#XXXXXX\` | Hook + CTA backgrounds, callout cards |

| Signature accent | {YOUR_ACCENT_NAME} | \`#XXXXXX\` | Inline highlights, pills, key numbers |

| Background light | {YOUR_LIGHT_NAME} | \`#XXXXXX\` | Body slide backgrounds |

| Pure | White | \`#FFFFFF\` | Dark-slide text, pure contrast |

| Body text dark | {YOUR_BODY_NAME} | \`#XXXXXX\` | Body copy on light slides |

| Secondary accent | {NAME} | \`#XXXXXX\` | Data points, secondary highlights |

| Positive tint | {NAME} | \`#XXXXXX\` | Positive data, "after" cards |

| Positive bg | {NAME} | \`#XXXXXX\` | "New way" comparison card |

| Divider accent | {NAME} | \`#XXXXXX\` | Category labels, dividers, small caps |

| Dark depth | {NAME} | \`#XXXXXX\` | Dark cards on light, muted dark accent |

| Negative / contrast | {NAME} | \`#XXXXXX\` | "Old way" cards, warnings, negative data |

| Tertiary accent | {NAME} | \`#XXXXXX\` | Optional rotation accent (use sparingly) |

DO NOT use any hex not in this list. Discipline keeps carousels recognizable.

\### Two-Theme System (the key to visual rhythm)

Every slide is either DARK or LIGHT. Mix them deliberately:

DARK theme (signature look):

\- Background: Primary dark

\- Headline: White

\- Label: Signature accent (small caps)

\- Body text: Positive bg at 85% opacity

\- Accent highlights: Signature accent background on marked words

\- Divider: Signature accent

LIGHT theme (breathing room):

\- Background: Background light

\- Headline: Primary dark

\- Label: Dark depth (small caps)

\- Body text: Body text dark

\- Accent highlights: Signature accent background on marked words

\- Divider: Divider accent

\### Mandatory Slide Rhythm Pattern

Never run more than 2 light slides in a row. Default pattern for a 6-slide carousel:

| Slide | Theme | Reason |

|---|---|---|

| 1 Hook | DARK | Stop the scroll - signature dark+accent moment |

| 2 Body | LIGHT | Breathing room, context |

| 3 Body | LIGHT | Content density |

| 4 Body | DARK | Mid-carousel re-engagement (the "key insight") |

| 5 Body | LIGHT | Final explanation |

| 6 CTA | DARK | Signature close |

For 5 slides: \`DARK → LIGHT → DARK → LIGHT → DARK\`

For 7-8 slides: insert extra LIGHT slides in the 2-3 and 5-6 positions.

\### Typography

\> Replace the font names below with your brand fonts. The renderer auto-falls-back if a font is missing.

Latin script (English, Spanish, etc.):

\- Headlines & category labels: {YOUR_DISPLAY_FONT} (brand primary)

\- Hook headline: 96-108px, Bold, tracking -1%

\- Body title: 72-80px, SemiBold, tracking -1%

\- Category label: 26px, Medium, tracking +8%, UPPERCASE

\- Body copy & pills & code: {YOUR_BODY_FONT} (secondary)

\- Body text: 34-38px, Regular, line-height 1.35

\- Pills: 28px, Medium

\- Code block: 30px, Medium (mono-spaced)

\- Counter/swipe bar: {YOUR_BODY_FONT} Medium, 24px, tracking +5%

CJK / non-Latin script (if applicable):

\- Headlines & labels: {YOUR_CJK_DISPLAY_FONT} Heavy

\- Hook: 88-96px (CJK renders visually heavier - size down ~10%)

\- Body title: 64-72px

\- Body: {YOUR_CJK_BODY_FONT} Medium / Regular, 32-36px

\- Counter/handle: {YOUR_CJK_BODY_FONT} Light, 24px

\### Strict Layout Grid

\`\`\`

┌─────────────────────────────────┐ ← 1080×1080

│ BRAND NAME NN / TT │ ← 80px top bar

│─────────────────────────────────│

│ │

│ CATEGORY LABEL │ ← 60px below bar

│ │

│ HEADLINE WITH │

│ \*ACCENT WORDS\* │ ← Display font Bold, fills width

│ │

│ ━━━━━ │ ← 80px accent divider bar

│ │

│ Content block(s) │

│ │

│─────────────────────────────────│

│ SWIPE → N / TOTAL │ ← 80px bottom bar

└─────────────────────────────────┘

\`\`\`

Non-negotiables:

1\. 96px left/right padding

2\. Divider bar is a solid rectangle, 80px × 6px, in your signature accent (dark slides) or divider accent (light slides)

3\. Top + bottom bars have 1px hairline separator (white at 15% on dark, primary dark at 10% on light)

4\. Counter format: \`01 / 06\` (zero-padded, always two digits)

5\. SWIPE indicator: localize to your primary language

6\. Headline max 4 lines. If it overflows, shorten the copy - never shrink the type.

\### Content Block Styling

\#### \`pills\` - Tool tags

\- On LIGHT slides: White pill, 2px primary-dark border, primary-dark text. Active pill = signature accent fill, primary-dark text.

\- On DARK slides: Dark pill, 2px signature-accent border (50% opacity), white text. Active pill = signature accent fill, primary-dark text.

\- Pill padding: 20px horizontal, 14px vertical. Border radius: pill-shaped.

\- Gap between pills: 16px

\#### \`comparison\` - Old vs New

\- On LIGHT slides: Negative-tint card over light bg + Positive-bg card

\- On DARK slides: Negative-tint card at 20% + Positive-tint card at 15%

\- Each card: 32px radius, 40px padding

\- Stack vertically with 24px gap

\#### \`card\` - Dark callout (only on LIGHT slides)

\- Background: Primary dark

\- Label: Signature accent, display font Medium 22px

\- Text: White, body font Regular 36px

\- Padding: 48px, Radius: 32px

\#### \`card\` variant - Light callout (only on DARK slides)

\- Background: Signature accent (10% opacity) + 1px signature-accent border

\- Label: Signature accent

\- Text: White

\#### \`code_block\` - macOS-style

\- Background: Deep variant of primary dark on BOTH themes

\- Traffic dots: actual \`#FF5F57\` / \`#FEBC2E\` / \`#28C840\`

\- Keyword color: Signature accent, body font Medium

\- Rest color: Light positive tint, body font Regular

\- Padding: 48px, Radius: 24px

\#### \`image\` - Product screenshots only

\- Rounded corners: 32px radius

\- 1px border: white at 20% on dark slides / primary-dark at 10% on light slides

\- Never fill full width - leave 96px padding consistent with text

\### Accent Highlight Rendering

Marked words (\`\*like this\*\`) get a filled signature-accent rounded rectangle behind them:

\- Rectangle: signature-accent solid fill

\- Radius: 8px

\- Padding: 8px horizontal, 4px above/below letter bounds

\- Text on top stays primary-dark on BOTH themes - pops on dark slides too

\- Max 3 highlighted phrases per slide. 1-2 is more powerful.

\### Decorative Details

1\. Slide-number badge (optional on hook/CTA): signature accent small circle with slide number

2\. Arrow glyph (→) after key phrases - signature accent on dark, divider accent on light

3\. Accent dot rows under category labels: three 8px circles, signature accent, 12px gap

4\. Oversized opening quote mark (optional) on hook quote slides - 200px, signature accent at 40% opacity, behind text

\---

\## Image Policy - Specific and Relevant, or Skip It

Golden rule: A well-designed text-only slide beats a mediocre stock image every time.

\### When to use images

Only use \`image\` field when the slide directly features a specific named product/tool and you can find its actual UI screenshot or official logo.

\### How to search for product images

1\. First: official UI screenshot

\- Search: \`"\[product name\]" official screenshot site:\[official-domain\]\`

\- Maintain a \`domains.md\` list of official sources for tools in your niche

2\. Second: dark mode screenshot

\- Search: \`"\[product name\]" dark mode UI screenshot\`

3\. Third: transparent logo

\- Search: \`"\[product name\]" logo transparent PNG official\`

4\. If nothing good found → use \`pills\` instead. Tool pill tags look professional and load reliably. Never settle for an irrelevant image.

\### Images to NEVER use

\- Stock photos with people (handshakes, laptops, headshots)

\- Abstract clichés (circuit boards, glowing brains, robot hands)

\- White-background images on concept slides - they clash with cream/colored bgs

\- Low-resolution (<1080px) or watermarked images (Getty, Shutterstock)

\- Pinterest sources (unclear copyright)

\- Any image not directly related to the slide topic

\### Image quality requirements

\- Minimum 1080px on shortest side

\- Prefer PNG (especially for logos/UI)

\- {BRAND_BACKGROUND_PREFERENCE} - pick image bg colors that complement your slide bgs

\- No text overlay duplicating slide text

\---

\## Config.json Notes

\### Do NOT add \`"colors"\` override

The render script already uses your brand theme by default. Do not add a colors block unless explicitly needed for a special variant.

\### Accent highlighting in copy

Mark 1-3 key words per slide with \`\*asterisks\*\`. Marked words get a signature-accent background highlight drawn behind them. Over-using highlights destroys the effect.

\### Label field (category tag above headline)

Always include a \`"label"\` on every slide. Examples:

\- Hook: \`"JUST LAUNCHED"\` / \`"WHY THIS MATTERS"\` / \`"THE PROBLEM"\`

\- Body: \`"WHAT IS IT"\` / \`"HOW IT WORKS"\` / \`"OLD WAY VS NEW WAY"\` / \`"KEY FEATURES"\`

\- CTA: no label needed