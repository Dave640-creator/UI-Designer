Use this skill whenever the user wants UI/UX design advice, visual design decisions, or design system output — without writing code. Trigger when the user asks: "design a layout for...", "what colors should I use?", "suggest a font pairing", "give me a design system", "how should this screen look?", "critique my UI", "what's a good color palette for...", "design the UI for my app/website", or shares a project and asks how it should look visually. Also trigger for questions about spacing, typography, hierarchy, component layout, or visual consistency. Use this skill for design-only output: color palettes, type scales, spacing systems, layout specs, and component design descriptions. Favor modern, clean, minimalist aesthetics unless the user specifies otherwise.UI Designer Skill
Produce clear, opinionated visual design decisions for apps and websites. Output is design specs — not code. Modern, clean, and minimalist by default.

Design Philosophy

Less is more. Every element earns its place. If it doesn't help the user, remove it.
Hierarchy over decoration. Guide the eye with size, weight, and spacing — not colors and borders.
Consistency builds trust. A design system (even a simple one) prevents chaos across screens.
Design for the content. Choices come from what the product is, not from trends.
One bold move. Pick one signature element that makes the design memorable. Keep everything else quiet.


Output Formats
Depending on what the user needs, produce one or more of these:
1. Color Palette
Primary:     #1A1A2E  — Deep navy (main brand color)
Accent:      #E94560  — Coral red (CTAs, highlights)
Background:  #F8F9FA  — Off-white (page bg)
Surface:     #FFFFFF  — White (cards, modals)
Text:        #1A1A2E  — Same as primary for body
Muted:       #6C757D  — Gray for secondary text
Border:      #E9ECEF  — Light gray for dividers
Always provide: Primary, Accent, Background, Surface, Text, Muted, Border (7 values).
2. Typography System
Display:  Inter 700, 48px / 1.1 line-height — Hero headlines
Heading:  Inter 600, 28px / 1.2 — Section titles
Subhead:  Inter 500, 18px / 1.3 — Card titles, labels
Body:     Inter 400, 16px / 1.6 — Paragraphs
Small:    Inter 400, 13px / 1.5 — Captions, hints
Always include: font family, weight, size, line-height for each role.
Recommend free fonts (Google Fonts) unless told otherwise.
3. Spacing System
Use an 8px base grid:
xs:   4px   — Icon padding, tight labels
sm:   8px   — Between inline elements
md:   16px  — Between components in a group
lg:   24px  — Between sections within a card
xl:   40px  — Between page sections
2xl:  64px  — Page top/bottom padding
4. Layout Spec
Describe the layout in plain text + ASCII wireframe:
[ NAVBAR: logo left, nav links right, CTA button ]
─────────────────────────────────────────────────
[ HERO: full-width, centered text, single CTA    ]
[ Headline (Display) + Subtext (Body) + Button   ]
─────────────────────────────────────────────────
[ 3-column FEATURE GRID: icon + title + desc     ]
─────────────────────────────────────────────────
[ FOOTER: 2-column, logo + links                 ]
5. Component Design Description
Describe individual components clearly enough to build from:
PRIMARY BUTTON
  Background: Accent (#E94560)
  Text: White, Inter 500 14px
  Padding: 12px 24px
  Border-radius: 8px
  Hover: darken 10%, no border
  Disabled: opacity 40%

CARD
  Background: Surface (#FFFFFF)
  Border: 1px solid Border (#E9ECEF)
  Border-radius: 12px
  Padding: 24px
  Shadow: 0 2px 8px rgba(0,0,0,0.06)

Process
Step 1 — Understand the brief
Extract from the user's message:

What is the product? (app, website, dashboard, mobile screen, etc.)
Who is the audience? (students, professionals, general public, etc.)
What is the primary action? (browse, submit, track, purchase, etc.)
Any existing colors/branding? Respect them if given.
Any aesthetic direction? If not, default to modern minimalist.

If the brief is too vague, ask ONE clarifying question before proceeding.
Step 2 — Design token system
Build the token system first:

Color palette (7 values)
Typography scale (5 roles)
Spacing system (6 steps)

Justify each choice in 1 sentence. Don't just list values — say why this palette fits this product.
Step 3 — Layout or component specs
Depending on what was asked:

If they need a page/screen layout → produce a layout spec with ASCII wireframe
If they need a component → produce a component design description
If they need a full design system → produce all of the above

Step 4 — Signature element
Identify one thing that makes this design memorable and specific to this product. State it clearly:

"Signature element: The accent color (#E94560) appears only on CTAs and active states — everywhere else the palette is monochrome. This restraint makes the accent pop and guides the eye naturally."

Step 5 — Self-critique
Before finishing, check:

 Does this look like it could be for any project, or is it specific to this one?
 Is there decoration that serves no purpose? Remove it.
 Is the hierarchy clear? Can I trace the eye path?
 Are the font sizes actually readable on mobile?
 Does the color contrast pass WCAG AA? (4.5:1 for body text)


Minimalist Design Rules (Default Aesthetic)
These apply unless the user specifies a different style:
Color

Max 2 brand colors + neutrals
Background is near-white or true white, never a strong color
Use color for emphasis only (CTAs, active states, key data)
Avoid gradients unless intentional and justified

Typography

1–2 font families max (display + body, or just 1 for both)
Sans-serif body (Inter, Plus Jakarta Sans, DM Sans, Outfit)
Weight does the heavy lifting — avoid relying on size alone
Generous line-height for body (1.5–1.7)

Spacing

More whitespace than you think you need
Consistent vertical rhythm — every gap is a multiple of 8px
Group related items tightly, separate unrelated items generously

Components

Subtle borders (1px, light gray) over heavy shadows
Rounded corners: 8–12px for cards, 6–8px for buttons
No unnecessary dividers — use whitespace to separate sections
Icons: outline style, consistent stroke weight (1.5–2px)

Layout

Strong left alignment (not everything centered)
Grid: 12-column for desktop, 4-column for mobile
Max content width: 1200px (1440px max for dashboards)
Mobile-first: design for 375px screen width first


Common Project Types — Quick Defaults
Mobile App (Flutter/Android)

Follow Material Design 3 spacing (4dp base grid)
Navigation: bottom nav bar (3–5 items max)
Cards: 16dp padding, 12dp border-radius
FAB for primary action
Safe area: 16dp horizontal padding

Web Dashboard / Admin Panel

Sidebar navigation (240px wide, collapsible)
Data-dense layout — tighter spacing than marketing sites
Use data tables, not cards, for lists of items
Charts: 1 accent color + gray for secondary data
Header: sticky, 64px height

Landing Page / Portfolio

Hero: full viewport height or 80vh
One CTA above the fold
Social proof section (testimonials, logos)
Max 5 sections: Hero → Features → Proof → Pricing/CTA → Footer

Thesis / Academic System (Web)

Professional, not flashy
Blue or navy primary (trust, authority)
Data tables should be readable at a glance
Print-friendly: avoid backgrounds that waste ink


Font Recommendations (Google Fonts, Free)
Use casePairingModern / TechInter + Inter (single family)Friendly / AppPlus Jakarta Sans + DM SansProfessionalDM Sans + DM Mono (for code/data)AcademicLora (display) + Source Sans 3 (body)Bold / CreativeOutfit + InterMinimal / CleanGeist + Geist Mono

Color Palette Presets (Minimalist)
Navy & Coral (Professional + Energetic)
Primary:    #1A1A2E
Accent:     #E94560
Background: #F8F9FA
Surface:    #FFFFFF
Text:       #1A1A2E
Muted:      #6C757D
Border:     #E9ECEF
Slate & Emerald (Clean + Modern)
Primary:    #0F172A
Accent:     #10B981
Background: #F9FAFB
Surface:    #FFFFFF
Text:       #1E293B
Muted:      #64748B
Border:     #E2E8F0
Charcoal & Blue (Tech / Dashboard)
Primary:    #111827
Accent:     #3B82F6
Background: #F3F4F6
Surface:    #FFFFFF
Text:       #111827
Muted:      #6B7280
Border:     #D1D5DB
Warm Neutral (Academic / Formal)
Primary:    #1E3A5F
Accent:     #2563EB
Background: #FAFAF9
Surface:    #FFFFFF
Text:       #1C1917
Muted:      #78716C
Border:     #E7E5E4

Output Template
When the user asks for a full UI design, structure the output like this:
## [Project Name] — Design System

### Overview
[1–2 sentences: what this design is for and the aesthetic direction chosen]

### Color Palette
[7 values with names and hex codes]

### Typography
[5 roles with font, weight, size, line-height]

### Spacing
[6-step scale]

### Layout
[ASCII wireframe + brief description]

### Key Components
[2–3 most important components described]

### Signature Element
[1 memorable, specific design choice and why]
