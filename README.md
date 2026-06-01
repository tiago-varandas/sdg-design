[README.md](https://github.com/user-attachments/files/28470450/README.md)
# SDG.design

**Open-source DESIGN.md starter kits for the 17 Sustainable Development Goals.**

Browse a goal. Download the system. Generate a product in Stitch. Launch faster.

→ **[sdg.design](https://sdgdesign.netlify.app/)** · Built for the [Google Stitch Challenge](https://stitch.withgoogle.com)

---

## What is this?

SDG.design is a community-curated registry of [DESIGN.md](https://stitch.withgoogle.com/design-md) files — one for each of the UN's 17 Sustainable Development Goals.

Each kit encodes **domain knowledge that no AI prompt can infer on its own**: field conditions for rural water workers, anxiety-responsive patterns for health apps, coercive control protections for safety tools, the despair trap in climate communication.

Paste any kit into Stitch and generate a complete, context-aware product — website, mobile app, or dashboard — in minutes.

---

## Why it exists

When you prompt Stitch with *"build a water access app"*, it generates something competent and generic. When you paste in the SDG 06 DESIGN.md, Stitch generates something that knows about:

- The **3-tap rule** for field workers with wet or gloved hands
- **7:1 contrast ratios** for sunlight legibility, not the WCAG default 4.5:1
- **Inter Mono** for all sensor data so numbers align in field conditions
- **Semantic status colors** — safe/warning/critical — that can never be used decoratively

That difference is the product.

---

## The kits

| SDG | Goal | Status | Top kit |
|-----|------|--------|---------|
| 03 | Good Health & Well-being | ✅ Ready | Community Health Worker Tool |
| 04 | Quality Education | ✅ Ready | Shared Device Literacy App |
| 05 | Gender Equality | ✅ Ready | Safety & Coercive Control Tool |
| 06 | Clean Water & Sanitation | ✅ Ready | Community Field Monitor |
| 11 | Sustainable Cities | ✅ Ready | Civic Reporting & Trust Platform |
| 13 | Climate Action | ✅ Ready | Campaign & Pledge Platform |
| 01–02, 07–10, 12, 14–17 | All others | 🔓 Open | Be the first to contribute |

---

## How to use

**Option 1 — Paste into Stitch**
1. Open any `.md` file in this repo
2. Copy the full contents
3. Go to [stitch.withgoogle.com](https://stitch.withgoogle.com)
4. Click "Start with your design" → paste into the DESIGN.md field
5. Describe your product and generate

**Option 2 — Download from SDG.design**
1. Visit [sdg.design](https://sdgdesign.netlify.app/)
2. Click any active SDG
3. Choose a kit variant
4. Click "Open in Stitch →" — the DESIGN.md copies to your clipboard automatically

**Option 3 — Use with Claude Code or Cursor**
Drop any `.md` file into your project root. Both tools will read the design tokens and apply them to generated UI.

---

## What makes these kits different

Each DESIGN.md file has two layers:

**1. Design tokens** — colors, typography, spacing, components — in the standard YAML format.

**2. Domain knowledge sections** — prose that encodes context no AI infers from a prompt:

- `## Field Conditions` — SDG 06: sunlight legibility, battery constraints, 3-tap rule
- `## Anxiety-Responsive Design` — SDG 03: the 3am test, shame as a design failure
- `## The Shared Device Problem` — SDG 04: no streak mechanics, PIN-based profiles
- `## Designing Against Coercive Control` — SDG 05: disguise mode, duress PIN, screenshot-safe screens
- `## The Trust Gap` — SDG 11: why anonymous reporting triples volume
- `## The Despair Trap` — SDG 13: why scale mismatch between data and actions causes paralysis

---

## Contribute

The 11 open SDGs need kits. So do the 6 active SDGs — every context deserves its own system.

**To submit a kit:**
1. Fork this repo
2. Create a folder: `/sdgs/[number]-[name]/[your-kit-name]/DESIGN.md`
3. Open a pull request with a description of the context your kit is optimised for
4. The community rates it — the best kit rises to the top

**Good submissions include:**
- A clear scenario (who uses this, in what context)
- Domain-specific Do's and Don'ts beyond aesthetics
- Evidence it works — a screenshot of something generated in Stitch using your kit

---

## The vision

SDG.design is the design system registry for global impact — every SDG, every scenario, rated by the builders who used them in the field.

Version 1 ships with 6 founding kits. The architecture supports unlimited community submissions. The best system for each context rises to the top. Domain expertise from NGO designers, civic technologists, and field workers — not just generalists.

---

## License

Apache 2.0 — free to use, modify, and distribute.

*Not affiliated with or endorsed by the United Nations. SDG colors used in accordance with UN guidelines for awareness purposes.*
