# Current Redesign

_Started 2026-05-07 11:30 UTC_

---

## User

we need to redesign this
check it out. don't design right now

## Assistant

I took a look at the wireframe for the Bitshala site. Here's what I see:

**Current structure:**
- Hero with dark photo bg + orange accent, dual CTAs ("Join our community" / "Explore study cohorts")
- "So, what do you folks do at Bitshala?" — mission blurb + supporter/affiliate logo strips
- "Bitcoin seems really technical..." — 6-card grid of activities (Latest in Bitcoin Tech, Reading Club, Bitcoin PR Review Club, Bengaluru BITDEVS, Bitcoin Study Cohorts, Bitshala Fellowship)
- Testimonials — 3-column wall of quotes from community members
- "And, if I wanted to start my Bitcoin dev journey..." — 5-step orange journey section (Discord → club activities → fellow devs → Fellowship → Bitspace)
- "It's not just about learning; it's about growing together" — closing pitch + big orange CTA card
- Footer

**What stands out as redesign opportunities:**
1. **Hero feels generic** — heavy dark photo overlay + orange wash is a common Bitcoin-org trope. Could be more distinctive to Bitshala specifically.
2. **Two competing logo strips** ("Supported by" + "In collaboration with") sit in identical orange bands — visually noisy, hierarchy unclear.
3. **6-card activities grid** — all cards weigh the same, but Fellowship (paid) and BITDEVS (in-person) are very different commitments than Reading Club. Worth differentiating.
4. **Testimonial wall** is dense and unscannable — 3 columns of similar-length paragraphs.
5. **Orange "journey" section** is the strongest idea on the page (a clear linear path), but it's buried below testimonials and visually disconnected from the activities grid above — they're really the same content twice.
6. **Two big CTAs at the end** ("Take the first step" card + footer) repeat the hero CTA — feels redundant.
7. **Color usage** — orange is doing a LOT of work (hero accent, both logo bands, journey section, final CTA). Could use more restraint or more variation.
8. **Type hierarchy** is flat — section headers, body, and card titles don't have enough size contrast.

**Before I design, a few things I'd want to know:**
- Is there an existing brand kit (logo files, exact orange, typefaces) or should I treat this as an open canvas grounded in what's on the current site?
- Who's the primary audience — total Bitcoin newcomers, devs already comfortable with code, or both equally?
- Is the "journey" (Discord → activities → Fellowship → Bitspace) the *real* spine of what Bitshala offers? If so, I'd consider making it the organizing structure of the whole page rather than a section.
- Any activities/programs missing from the wireframe, or any being deprecated?
- Desktop-only redesign, or should I plan mobile breakpoints too?
- Tone preference — keep the warm/grassroots feel, push more technical/serious, or something else?

Let me know and I'll put together a few directions.

## User

logo and font

total Bitcoin newcomers, devs already comfortable with code, audience is both equally

i'll be sharing a wireframes try to make it like that

## Assistant

Got the fonts (Satoshi + Apfel Grotezk) — those are great choices, very different from the generic web stack. I don't see a logo file attached yet though, just the two font families.

A few things before I start designing:

1. **Logo** — could you attach the Bitshala logo file (SVG ideally, or PNG)?
2. **Wireframes** — you mentioned you'll share wireframes. I'll wait for those before designing so I match the layout you have in mind.
3. **Brand orange** — do you have an exact hex for the Bitshala orange, or should I pull it from the existing screenshot?
4. **Font roles** — Apfel Grotezk has a strong display character (especially Fett/Satt weights). My instinct: Apfel Grotezk for headlines/display, Satoshi for body and UI. Sound right, or do you want them used differently?

Drop the logo + wireframes when you're ready and I'll get started.

## User

Visual Style: A high-contrast, "Neo-Brutalist" academic aesthetic. The design should feel tactile, using a "Paper & Glass" layering system.

Color Palette: > * Primary: Deep Ink Black and a vibrant, "Electric" Bitcoin Orange.

Background: A warm, grainy cream-parchment texture (replacing the flat off-white) to give it a traditional "Pathshala" feel.

Typography: > * Headlines: Use an ultra-bold, condensed sans-serif (like the "FUTURE" text in the reference) with tight kerning.

Secondary Text: A clean, high-readability monospace font to lean into the "coder/technical" side of Bitcoin.

UI Elements (The FinFLO Influence):

Layering: Elements should look like physical cards dropped onto the page. Use heavy, soft-drop shadows and slight rotations (1-2 degrees) to make the tree "leaves" and the staircase "blocks" look like physical objects.

3D Metaphors: Instead of a flat 2D tree, the "Bitshala Tree" should be a high-detail 3D isometric illustration or a stylized clay-render. The "Stairs" should have a thick 3D depth, looking like concrete blocks with orange neon lighting embedded in the edges.

Grain & Noise: Apply a subtle film grain/noise overlay across the entire site to remove the "digital" flatness and make it feel more "authentic" and human.

Interactive Details: > * Buttons and cards should have a "pressed" state where the shadows disappear, mimicking a physical button.

Use "Sticker" or "Stamp" elements (like the orange 'plus' signs in the reference) as decorative anchors for the Indian map and event icons.


this is the aesthetic. don't use any mascot

## Assistant

_[tool: snip]_

Got it — locked in the aesthetic direction:

**Bitshala Neo-Brutalist / Pathshala**
- **Colors:** Deep ink black, electric Bitcoin orange, warm grainy cream-parchment background
- **Type:** Apfel Grotezk (ultra-bold, condensed) for headlines with tight kerning; mono for secondary/technical text; Satoshi for body
- **Surfaces:** Paper-and-glass layering — physical cards with heavy soft drop shadows, slight 1–2° rotations, pressed states on click
- **Texture:** Film grain/noise overlay across the whole page
- **3D moments:** Bitshala "Tree" as isometric/clay render; "Stairs" as concrete blocks with orange neon edges
- **Stickers:** Orange "+" stamps as decorative anchors (Indian map, event icons)
- **No mascot.** Got it — placeholders for any 3D illustrations rather than fake AI-generated characters.

A few quick questions before I build, then I'll wait for your wireframes:

1. **Logo** — still need the Bitshala logo file. Attach SVG/PNG when you can. I'll use a typeset placeholder until then.
2. **Wireframes** — you mentioned you'd share new wireframes. Should I:
   - (a) wait for the new wireframes before designing, or
   - (b) start now using the existing site's structure (hero → mission → activities grid → testimonials → 5-step journey → CTA → footer) reinterpreted in this new aesthetic?
3. **3D illustrations** — for the Tree and Stairs, you want me to leave clearly-marked placeholder slots (so you can drop in real renders later) rather than attempting them in CSS/SVG, right? That's my plan since you said no mascot and the brief specifies "clay-render" / "isometric" — those need real 3D, not faked.
4. **Indian map** — should this be a literal element on the page (for BITDEVS chapters / community locations)? If so, should I leave a placeholder for it too, or attempt a minimal SVG outline?

Drop the wireframes + logo when ready and I'll start building.

## User

here is the wireframe

## Assistant

I can read the wireframe now. Here's my understanding of the new structure:

1. **Hero** — "A PARTSHALA OF BITCOIN" big condensed display type
2. **"So what actually is Bitshala"** — the **Bitshala Tree**: a tree illustration with floating "leaf" cards (each card = an activity/program). This replaces the old 6-card grid.
3. **"How Bitshala is able to do all this"** — Trusted by + Collaboration partner strips (two horizontal logo bars)
4. **"How can you start your journey"** — the **Staircase**: stepped blocks (clubs → cohorts → fellowship → start your own → join us in upcoming events). This is the journey section, now visualized as physical stairs with orange neon edges.
5. **"People who worked with us / Wall of Love"** — testimonial grid, ~6 cards, slight rotations, paper aesthetic
6. **"Our gallery"** — photo gallery row of community/event images with rotated cards
7. **Footer**

A few last questions before I build:

1. **Tree leaves** — each leaf card holds one activity. From the existing site that's: Latest in Bitcoin Tech, Reading Club, PR Review Club, Bengaluru BITDEVS, Study Cohorts, Fellowship. So 6 leaves on the tree. Sound right?
2. **Staircase steps** — wireframe shows ~5 steps. My read: Discord → Club Activities → Hands-on Cohorts → Fellowship → Bitspace/Real-World. Confirm or adjust?
3. **Tree + Stairs as 3D placeholders** — you said no mascot, but the brief calls for clay-render tree and concrete-block stairs. I'll leave clearly-labeled placeholder slots for real 3D renders, with the activity cards/labels overlaid on top in HTML so the content is still real and editable. OK?
4. **Logo** — still need it. I'll typeset "BITSHALA" in Apfel Grotezk Fett as a placeholder.
5. **Gallery photos** — drop placeholder image slots so you can fill them with real photos? (Using `image_slot.js` so you can drag-and-drop them in.)

Confirm these and drop the logo when you can — then I'll build.

## User

1. yes
2. Staircase steps — wireframe shows ~5 steps. My read: Discord → Club Activities → Hands-on Cohorts → Events → Fellowship → starter grant
3. do the rendering then make it 3D
4. okay 
5. Gallery - make a placeholder

## Assistant

_[tool: snip]_

_[tool: update_todos]_

_[tool: list_files]_

Logo's there. Let me check it and set up.

_[tool: view_image]_

_[tool: image_metadata]_

Tree mark is the actual logo. Setting up.

_[tool: copy_files]_

_[tool: copy_starter_component]_

Now let me build the design. I'll plan the structure carefully — this is a single long landing page in the neo-brutalist Pathshala aesthetic.

**Design system commitment:**
- **Colors**: `#0A0908` ink black, `#FF6B1A` electric Bitcoin orange, `#F4ECDD` cream parchment
- **Fonts**: Apfel Grotezk Fett (display, ultra-bold condensed), JetBrains Mono (mono — Apfel doesn't ship mono so pairing with a system mono via Google Fonts), Satoshi (body)
- **Layering**: Cards with heavy soft shadows + 1–2° rotations, pressed states
- **Texture**: SVG noise grain overlay
- **3D moments**: Tree as stylized clay-render via layered SVG/CSS (since I can't use real 3D); Stairs as isometric concrete blocks with neon orange edges

Let me build it in pieces. Main file + a few component scripts.

_[tool: write_file]_

_[tool: snip]_

Now the Tree component as a separate file (it's the most complex piece — a 3D-feeling stylized clay-render done with layered SVG):

_[tool: write_file]_

Now let me build the main HTML file with all sections.

_[tool: write_file]_

_[tool: snip]_

_[tool: done]_

_[tool: fork_verifier_agent]_

Built **Bitshala.html** — neo-brutalist Pathshala aesthetic per your brief.

**What's in it:**
- **Hero** — "A Pathshala For Bitcoin" in Apfel Grotezk Fett, tight kerning, mono meta strip, grid background, big BTC watermark
- **Tree section** — stylized clay-render SVG tree (warm orange foliage, dark trunk, ground shadow) with 6 tiltable activity "leaf" cards floating around the canopy
- **Partners** — two logo strips (dark + cream) for "Trusted by" / "In collaboration"
- **Staircase** — 6 ascending concrete blocks with neon-orange edges on a black ink background, top step in solid orange
- **Wall of Love** — 8 quote cards in a masonry grid, mixed cream/dark/orange, decorative `+` stamps
- **Gallery** — 5 tilted `image-slot` placeholders you can drag photos into
- **Footer** — big condensed CTA, link columns, mono fine print

**Aesthetic details:**
- Cream parchment base + SVG noise grain overlay (mix-blend multiply)
- Cards have hard offset shadows + 1–2° rotations + pressed states (shadow disappears on `:active`)
- Orange `+` and circular "SINCE 2023" stamps as decorative anchors
- Apfel Grotezk display / Satoshi body / JetBrains Mono for technical bits

**Caveats:**
- Logo placeholder uses your uploaded PNG (which has the old "Bitshala A Pathshala for Bitcoin" wordmark baked in) — if you want just the tree mark, send an SVG/transparent crop and I'll swap it
- The tree is SVG-rendered "clay" — looks 3D-ish but isn't a real 3D render. If you want full clay/isometric fidelity, that needs a real render dropped in (I left the SVG so you can swap `assets/tree.svg` for an exported render anytime)
- Activity descriptions and testimonial copy are placeholders in your voice — swap real ones in
- Partner logo names are guesses based on the existing site — replace with the real logo files

## User

Verifier agent check completed

## Assistant

Three real bugs from the verifier — fixing.

_[tool: str_replace_edit]_

Now fix the tree SVG rendering by inlining it, and fix the staircase overlap.

_[tool: read_file]_

Inlining tree SVG into the HTML and fixing the staircase layout.

_[tool: run_script]_

Now the staircase. The blocks are 360px wide and only stride 110px, so they pile on top. I'll restructure so each step has enough horizontal stride that the text column is readable, while keeping the rising staircase look. I'll narrow each step, increase the stride, and let later steps tuck behind earlier ones (front-to-back z-index) — that's how real stairs read.

_[tool: str_replace_edit]_

_[tool: snip]_

_[tool: str_replace_edit]_

_[tool: done]_

_[tool: fork_verifier_agent]_

Fixed all three verifier issues:
1. Leaf cards — reset link styling (color + text-decoration)
2. Tree SVG — inlined into the HTML so it renders reliably
3. Staircase — narrowed steps to 230px and increased stride to 200px so each step's content is fully readable; wrapped in a 1280px track that scrolls horizontally on smaller screens

