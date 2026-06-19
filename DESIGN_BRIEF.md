# Design brief: aarushiguptamemorial.org

A project prompt for a design deliberation. Read it whole before proposing anything.
The goal of this conversation is to **deliberate on the design**, not to ship code.
Propose directions, show trade-offs, push back where you see a better path.

---

## 1. What this is, in one line

A website in memory of Aarushi Gupta, who died at 21, and a quiet front door to the
family-funded scholarship created in her name. One domain, two things held together.

## 2. The single most important principle

This is a memorial, but it must **burst with life, like she did**. The default memorial
site is muted, grey, somber, and a little self-pitying. This is the opposite of that.
Color, warmth, her face, light. She was 21 and full of life; the page should feel like
that, not like a tombstone.

Two failure modes to avoid in equal measure:

- **Somber and grey.** The generic "in loving memory" template. Emotionally dead.
- **Generic warmth.** Stock adjectives ("she was kind and bright") and pretty layout
  with nothing specific in it. A trained eye reads generic affect as absence of feeling.

The cure for both is **specificity**. One true, small, concrete thing about her lands
harder than any amount of sentiment. The design has to make room for the specific and
refuse to fill space with the generic. Do not dumb anything down to be "relatable":
emotional resonance comes from precision, not from lowering the register.

## 3. The two things the site holds

- **The memorial.** Who Aarushi was. The heart of the site. For the people who loved her.
- **The fund.** The Aarushi Gupta Memorial Education Fund, which gives scholarships.
  It exists because of her, and reads as a continuation of who she was, not as a campaign.

The fund must never overpower the memorial on the front page. She comes first; the fund
is what her family does in her name.

## 4. Audience

Weighted, in order:

1. **People who knew her** (family, friends, her wide circle). The site is a place they
   can return to.
2. **Students and institutions** who might benefit from the fund. They need clear,
   practical information on a separate page, not a sales pitch.

A potential donor is **not** an audience. See the next point.

## 5. Non-negotiable stance: we give, we do not ask

The family funds this themselves. **There is no donate button, and there never will be.**
No fundraising language, no pledge bar, no "support us." The site exists to *give*
scholarships, not to *take* donations. The fund page literally says: "We give. We do not
ask." Design accordingly. Nothing should make a visitor feel solicited.

## 6. Structure (six pages)

| Page | Path | What it does |
|------|------|--------------|
| Landing | `/` | Her, immediately, alive. Photo-led. Three soft paths underneath. |
| Her | `/aarushi` | "In all her glory." Photo-led, the page that bursts. The emotional centre. |
| Fund | `/fund` | The Aarushi Gupta Memorial Education Fund. The family's words, what it offers. |
| Apply | `/apply` | The scholarship program: eligibility, support, how to apply, deadlines. Practical. |
| Family | `/family` | The people who carry her forward. Quiet, warm. |
| Reach | `/reach` | Contact. One email. An invitation to share a memory. |

## 7. Visual direction (current working register, open to challenge)

The current build uses:

- **Warm cream** background (`#FBF6EB`), not white. Off the institutional palette entirely.
- **Color photographs**, never greyscale. Her face does the visual work.
- **One vibrant accent.** Currently a warm coral (`#E27D5A`), a placeholder. The open
  question is whether there is a color that was *hers*, and how saturated it should be.
- **Soft serif body** (Lora) and an **elegant serif display** (Cormorant Garamond).
- **Generous white space.** "Bursting with life" is color and warmth and her, breathing.
  It is not visual loudness or clutter.
- **No iconography, no stock graphics, no decorative motifs.** Photography only.

Treat all of the above as a strong starting point, not a locked decision. If you can argue
a better palette, type pairing, or photographic treatment that serves the principle in
section 2, make the case.

## 8. Real content you are designing around

**The fund.** The Aarushi Gupta Memorial Education Fund runs the Aarushi Gupta Memorial
Scholarship Program. It supports deserving, meritorious students pursuing higher education
without financial constraint. Eligibility: academic excellence, leadership, competitive
superiority, and genuine financial need. Support takes four forms: tuition fee assistance,
stipend, mentorship, and assistance for domestic and international academic competitions.

**How students apply.** Through their institution. A student raises it with their
institution's head, the institution shortlists, and forwards candidates to the Fund.
Deadlines: tuition and mentorship by 31 August 2026 for this year; competition assistance
and stipends are accepted year-round.

**The family's own words** (from their tribute card, use faithfully, do not rewrite into
generic copy): "Aarushi's life was marked by compassion, and a deep appreciation for
learning and personal growth. While her time with us was far too short, her values
continue to inspire those who knew and loved her. As a family, we wish to create a
meaningful and lasting tribute that would carry her legacy forward by supporting students
seeking financial help to fulfil their educational journeys."

**The people.** Parents: Dr. Anshul Gupta and Dr. Ruchi Gupta. Her older brother: Dhruv
Gupta (building this site). Her grandparents. Her father's brother, his wife, and their
children, the cousins she grew up beside and was very close to.

**Photography.** A color photograph of Aarushi exists and is currently the hero: she is
smiling, in front of a brightly painted wall. It was cropped from a family-made tribute
card, so it is low resolution for now; a higher-resolution original is expected. More
photographs will come from the family.

**Still to come from the family:** her years (birth and the year), one true line about her
for the landing, the themes and photographs for the "Her" page, a line in each family
member's own voice, and the scholarship brochure and application form as downloadable files.

## 9. Hard constraints

- **No em dashes anywhere.** Not in copy, not in design mockup text. Use commas, colons,
  semicolons, or periods. This is a firm house rule.
- **No donate flow of any kind** (see section 5).
- **Do not publish any personal email address.** All contact routes through
  `contact@aarushiguptamemorial.org`. (The family's scholarship emails use a personal
  address; it stays off the public site.)
- **Faithfulness.** Invent nothing about Aarushi. No fabricated dates, quotes, or details.
  Where content is missing, the design must hold an honest, dignified empty state, never a
  generated stand-in.
- **Accessibility.** Real alt text on every photograph. Any motion must respect
  `prefers-reduced-motion`. Legible contrast on the warm palette.
- **Hosting reality.** Static site, GitHub Pages, custom domain at the apex. Plain HTML
  and Tailwind. No heavy framework, no build that a small static host cannot serve.
  Google Workspace runs `contact@`, so email must keep working (DNS MX preserved).

## 10. Current state

A working skeleton exists: six HTML pages, Tailwind, the visual register above, her
cropped photograph wired into the landing and the "Her" page, the tribute card featured on
the Fund page, the Apply page populated from the real scholarship details, and honest
placeholders everywhere content is still pending. The skeleton builds and renders. We are
not redesigning from zero; we are deliberating on how to make it land.

## 11. What we want to deliberate with you

Bring point-of-view on these. Disagree with our defaults where warranted.

1. **Her color.** Is there one signature color the whole site should carry, and how
   vibrant? How do we choose it so it feels like hers and not arbitrary?
2. **The landing.** Lead with her photograph alone (current), the family tribute card, or
   a composition of both? What is the first thing a stranger should feel in half a second?
3. **The "Her" page, the one that must burst.** Themes (things she loved, the people she
   made laugh, small adventures, her own words) versus a gallery versus a timeline.
   Chronology ends in her death and pulls the page down; how do we structure for life
   instead? How much photography, how treated (full bleed, framed, grid)?
4. **Motion.** Appetite for subtle, tasteful animation that adds life without ever
   feeling gimmicky, versus none. If yes, where, and how restrained?
5. **Typography.** Confirm Cormorant Garamond plus Lora, or propose a pairing that better
   serves "alive, warm, specific, not institutional."
6. **Giving, not asking, made visual.** How do the Fund and Apply pages feel generous and
   open rather than transactional, while staying genuinely useful to a student?
7. **Holding two audiences.** How the memorial and the fund coexist without the fund
   intruding on the grief, and without the grief burying the practical information a
   student needs.
8. **Mobile.** Most visitors who knew her will arrive on a phone. What is the mobile-first
   experience, especially for the photo-led pages?
9. **Cultural register.** An Indian family. Any design cues that would feel warm and true
   rather than generic, without tipping into stereotype.

## 12. Deliverable from this deliberation

A clear design direction: palette, type, the landing and "Her" page compositions, the
photographic treatment, the motion stance, and how the six pages hang together, with the
reasoning tied back to the principle in section 2. Mockups or annotated wireframes welcome.
Hold every choice against one test: would someone who loved Aarushi feel her here, or feel
a template?
