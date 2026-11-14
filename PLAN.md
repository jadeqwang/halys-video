# HALYS — theatrical trailer: plan

Status: vision agreed in conversation on 2026-11-14. The shot-by-shot list is **not** written yet.
It waits on two things: the Thales research below (section 6) and word-level alignment of the track (section 7).

## 1. What this is

A two-minute theatrical trailer for a feature film that does not exist, about the Battle of the Halys
(28 May 585 BC): Lydians and Medes, six years into a war, stop fighting when a total solar eclipse arrives
mid-battle, and go home.

- **Track:** `inputs/Halys (trailer version, -2 st).wav`, 121.8 s, B minor, about 72 BPM half-time.
- **Lyrics and song notes:** `inputs/Halys lyrics.md`, `inputs/Halys Suno prompt.md`.
- **Cinematography target:** a Christopher Nolan film, somewhere between *The Odyssey*, *Tenet* and *Inception*.
  His name, and any real studio's marks, never appear on screen.

## 2. The idea

**Every "effect" in this film is a real eclipse phenomenon, photographed straight.**
To men in 585 BC who did not know what was coming, a real eclipse is a science-fiction event. Nothing is added.
The phenomena we use, all real:

- shadows sharpen and colour drains to pewter
- crescent suns project through wicker shields and leaves
- shadow bands crawl across the ground
- birds go to roost, horses balk, the air cools
- the Moon's shadow arrives from the horizon as a wall of darkness
- stars and Jupiter appear in daytime
- sunset colour glows on all 360° of the horizon
- the diamond ring at the end of totality

## 3. Locked decisions

| Topic | Decision |
|---|---|
| Look | Fully photoreal, large-format. No blended art styles. |
| On-screen lyrics | None. The vocal plays as the trailer's cover song. Lyrics go in closed captions. |
| Jade, the simulation, any coda | Out. |
| Ending | The title **HALYS**, with credits on the card in the manner of `1-music-shipped/holdfire`. |
| Thales | Shown **calculating**, never telling, never addressing anyone, never looking up in triumph. No legible method on screen. |
| Home | Shown only before and after the eclipse, never during it (see section 5). No Aryenis. |
| Production method | Every shot is staged or modelled first, then handed to video models. Models are chosen by bake-off. |

## 4. Look and grammar

- **Camera:** wide lenses close to faces, handheld; long-lens shots of the low sun through heat shimmer with
  small silhouettes; aerials for scale; grain, real dust, real bronze. One slow-motion passage only (the break).
- **Frame:** letterboxed scope until totality. The frame opens to full 16:9 height when the shadow hits and
  never closes again.
- **Colour, following the real light:**

| Phase | Palette |
|---|---|
| Day | Amber dust and the red river |
| Strange light | Desaturated silver |
| Totality | Steel-blue night, orange horizon ring, pearl corona |
| Return | Clean white-gold |

- **The three borrowings:**
  - *Odyssey*: the spine is homecoming, not battle. The men are exhausted. "Go home to the ones you love" is the film.
  - *Tenet*: the song is a palindrome ("Daylight turned to shade" / "Shadow turned to day"). The trailer hinges
    at totality, and second-half shots answer first-half shots in reverse order. The last shot resolves the first.
  - *Inception*: time dilates and the film cross-cuts under one shadow. One sword falling in extreme slow
    motion spans the break.
- **Text:** a few trailer cards at most, then the title card with credits.
- **Sound:** the song is untouched. The ticking pulse in the break gets a diegetic source: pebbles clicking down
  one at a time under Thales's hand (pending the research in section 6).

## 5. People

- **A Lydian and a Mede,** mirrored, each carrying a token of home. Costume tells the sides apart, never faces.
  Both armies get equal dignity; there are no villains.
- **Thales,** about 40, working. His last beat: he makes one more mark, then notices the light on his work has changed.
- **Home, split across the hinge.** We see the Lydian leave and the Mede come home, and the viewer completes
  the other half of each. The two houses must look clearly different. If this confuses in the animatic, fall
  back to one household.
- **The six years are visible in a child:** a toddler held at the departure, an eight-year-old in the doorway
  at the return.
- **One woman's face, held once,** at the departure. The voice is not hers. Nobody on screen sings or narrates.

## 6. Research task: Thales at work (launch a subagent)

**Why:** Thales must be shown calculating, in a real place, with real tools. The first sketch of this scene
had him writing on clay with a water clock nearby; both were wrong or doubtful. Nothing in his scene gets
staged until this research is back.

**How to launch:** start one fresh general-purpose agent (it needs web search and fetch) with the brief below
as its prompt. Run it in the background. It writes one file and reports back a short summary.

**The brief (paste as the prompt):**

> You are researching for a photoreal film trailer about the eclipse of 28 May 585 BC. One short scene shows
> Thales of Miletus, aged about 40, working out that the eclipse is coming. The director's rule is that he is
> shown *calculating*, never explaining. We need to know what that work would physically have looked like, and
> what the room or courtyard around him would have looked like, well enough to build the set and props.
> Accuracy matters more than drama: where the evidence is thin, say so.
>
> **Start here.** An earlier project already researched the prediction itself. Read these first, treat them
> as a starting point to check, not as settled:
> `production/research/THALES_METHOD.md`, `production/HISTORY.md` and `production/FACTCHECK.md` on the branch
> `claude/halys-music-video-fxr5i7` of `https://github.com/jadeqwang/halys-music-video`.
> Its conclusion was that the forecast is corroborated but the method is unknown, and that Herodotus 1.74
> says only that he named the year.
>
> **Question A: the calculation.** What would an Ionian Greek around 600–585 BC actually have done to work on
> a problem like this?
> 1. What do the ancient sources credit Thales with (Herodotus, Diogenes Laertius, Eudemus via later writers,
>    and others), and what do modern historians of astronomy think he could really have done? Cover the main
>    positions, including the view that the prediction is legend.
> 2. What knowledge could have reached Miletus from Babylon and Egypt by then (eclipse records, period
>    relations, lunar month counting), and by what route?
> 3. What would the working itself have consisted of: counting months, tallying, observing the Moon, shadow
>    measurements, drawn figures? What is plausible, what is attested only later, what is anachronistic?
> 4. How were numbers written and reckoned in archaic Ionia? Tally strokes, pebbles, any numeral system
>    actually attested by 585 BC, and what letter forms and writing direction were in use in Miletus.
>
> **Question B: the tools and surfaces.** For each of these, say whether it is attested for archaic Ionia,
> plausible, or wrong, and describe what it looked like (materials, size, how it was held and used): wax
> tablets and styluses, dust or sand boards and drawing on the ground, cord and peg for circles, pebbles for
> counting, a shadow stick or gnomon, potsherds, leather, papyrus, lead sheets, clay tablets, water clocks,
> lamps, and anything we have not thought of. We specifically need a sound source for a steady ticking: is
> placing pebbles one at a time defensible, and is there a better one?
>
> **Question C: the environment.** What did Miletus look like around 600–585 BC, before its destruction in
> 494 BC, and what would a prosperous Milesian's house and courtyard have looked like?
> 1. Architecture and materials: walls, roofs, floors, courtyard layout, doors, windows, what the
>    excavations of archaic Miletus show.
> 2. Furniture and household objects: stools, tables, chests, pottery styles in use (name the wares),
>    lamps, storage, textiles.
> 3. Clothing, hair and beard for a Milesian man of about 40 of his standing, and for anyone else who might
>    be in the house.
> 4. The setting outside: harbour, coastline, vegetation, the light and the night sky he would have worked
>    under, and where he could have watched the horizon.
> 5. What he would have seen from Miletus on the day: how deep the eclipse was there, at what time, and
>    how high the sun stood. Give the source or the computation.
>
> **Question D: what to avoid.** List the common anachronisms in depictions of Thales and early Greek
> science (for example white marble temples, togas, armillary spheres, scrolls everywhere, old-sage
> beards, Classical-period architecture) so the art department can rule them out.
>
> **Deliverable.** Write one file, `docs/research/THALES.md`, in the project at
> `/home/jade/Documents/halys-video`. Structure it as: a one-page summary of what to put on screen;
> then sections A to D. Mark every claim as **attested**, **plausible** or **speculative**, and cite the
> ancient source or the modern scholarship (author, title, year, and a link where one exists) for each.
> Where scholars disagree, give both sides. Include links to museum objects or excavation photographs
> that could serve as visual reference for props and set. Finish with a list of open questions you could
> not settle. Do not write a shot list or a scene; that is someone else's job.
>
> Report back in under 300 words: the three or four findings that most change how the scene should look,
> and anything in the earlier project's research that you found to be wrong.

**After it returns:** read `docs/research/THALES.md`, correct section 5 and the sound note in section 4 of
this plan if needed, then write Thales's shots.

## 7. Next steps, in order

1. Launch the Thales research (section 6).
2. Run word-level alignment and a beat grid on the trailer track, so every cut locks to a real beat or
   syllable. The timings in section 8 are read off the loudness curve only.
3. Check the remaining facts the pictures depend on: the eclipse geometry at the river (taken so far from the
   earlier project's `production/RESEARCH.md`, not re-derived) and Lydian and Median dress and arms.
4. Write the shot-by-shot list, with a staging spec for every shot.
5. Stage or model the shots, then run bake-offs on a small set covering the hard cases: a crowd battle,
   a hero face, the low sun on a long lens, the slow-motion sword.
6. Animatic against the track, then full generation, edit, sound layer, title and credits card.

## 8. Shape against the track (approximate, ±1 s)

| Time | Music | Picture |
|---|---|---|
| 0:00–0:08 | Harp, drone | Cold open: Thales at work, a year earlier |
| 0:08–0:27 | Hushed verse | The departure from home; the war, tactile and tired, in low gold light |
| 0:27–0:37 | Pre-chorus | The light goes strange; men notice one by one, still fighting |
| 0:37–1:02 | Chorus 1, braam | The shadow wall hits, the frame opens, a comrade's arm stops a strike, the fighting stops in a wave |
| 1:03–1:08 | Break: held note, ticking | The falling sword in slow motion; ten thousand men silent |
| 1:08–1:29 | Build | Cross-cutting accelerates; the palindrome starts running back; Thales notices the light |
| 1:29–1:30 | Silence | Black, then the diamond ring on "a sudden spark" |
| 1:30–1:50 | Final chorus, key change | Light slams back; bronze let go; enemies pass each other in the river; the return home |
| 1:50–1:56 | Climax chant | Fastest cutting; each hit is a weapon landing on stone |
| 1:56–end | Three hits, silence, minor chord | Three images cut to black (the kings' oath among them); the title and credits card |

## 9. Kept from the earlier attempt

- The eclipse geometry: sunset totality, the sun low over the river's vanishing point, the armies mirrored on
  the two banks.
- The eclipse as a clock: the bite grows through the first act.
- The director's corrections: men look up mid-action; bronze is precious, so it is dropped, never thrown;
  a comrade's arm-pull stops the strike.
- Crescent suns through wicker shields; Jupiter beside the black sun; the blood oath of Herodotus 1.74.
- The eclipse always looks like a real eclipse.

Left behind: the five art worlds, the history montage, the terminal and wink, on-screen lyrics and HUD,
and the painted and line-art renderers.
