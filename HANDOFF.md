# Handoff prompt

Paste this into a fresh session to take over the production.

```
You're taking over a film production. The project is in
/home/jade/Documents/halys-video. Read PLAN.md in full first, then
inputs/Halys lyrics.md and inputs/Halys Suno prompt.md, and listen to the
structure of inputs/Halys (trailer version, -2 st).wav by analysing it.

WHAT WE'RE MAKING
A two-minute photoreal theatrical trailer for a feature film that doesn't
exist, cut to that track. The film is about the Battle of the Halys
(28 May 585 BC): Lydians and Medes, six years into a war, stop fighting
when a total solar eclipse arrives mid-battle, and go home. It should feel
like the trailer for a Christopher Nolan film somewhere between The
Odyssey, Tenet and Inception, paced as though the full film exists. The
core idea is that every "effect" is a real eclipse phenomenon photographed
straight: to men who didn't know it was coming, a real eclipse is a
science-fiction event.

The finished piece is a 1920x1080 video the length of the track (121.8 s),
with the song untouched, a light sound-design layer under it, and an end
card with the title HALYS and credits.

WHAT'S SETTLED
PLAN.md sections 1 to 5 record the vision and the decisions I agreed in an
earlier conversation: fully photoreal, no on-screen lyrics, no Jade or
simulation or coda, Thales shown calculating and never explaining, home
shown only before and after the eclipse, the frame opening at totality,
the palindrome structure. Treat these as settled. Don't reopen them or
offer alternatives. If research or production shows one of them can't
work, tell me what you found and what you'd do instead, and wait.

WHAT TO DRAW ON
- An earlier attempt at a longer version of this song is at
  https://github.com/jadeqwang/halys-music-video, branch
  claude/halys-music-video-fxr5i7. Its look and structure are abandoned
  (PLAN.md section 9 says what's kept). What's worth harvesting is its
  research (production/RESEARCH.md, FACTCHECK.md, HISTORY.md,
  research/THALES_METHOD.md), its character and costume boards
  (media/chars, media/boards), its audio tooling (tools/audio: beat grid,
  word alignment) and its generation tooling and model schemas (tools/,
  production/TOOLING.md, production/PLATES.md, which includes notes on how
  the video model behaved). Check its facts before relying on them; I have
  not re-derived the eclipse geometry.
- My shipped videos are in /home/jade/Documents/1-music-shipped. Read
  holdfire's CLAUDE.md, README and docs for how I like a production run,
  and use its end card as the model for the HALYS title and credits card.
- I don't know which image and video models or credentials are available
  on this machine right now. Find out early and tell me.

HOW I WANT IT MADE
Every shot is staged or modelled before it goes to a video model: a locked
still or blocked 3D or composited frame that fixes composition, lens,
light, costume and action, so the video model is animating a decision and
not making one. Models are chosen by bake-off: run the same staged shot
through the candidates and pick on the result. Bake off a small set of
shots that covers the hard cases (a crowd battle, a hero face in close-up,
the low sun on a long lens with silhouettes, the slow-motion falling
sword, Thales's hands at work) before generating anything in bulk.

Cuts lock to the music. Run word-level alignment and a beat grid on the
trailer track before writing the shot list; the timings in PLAN.md
section 8 are approximate.

Accuracy matters to me more than drama. Costume, arms, tools, architecture
and the sky should be right for 585 BC, with sources, and where the
evidence is thin I want that said plainly. Both armies get equal dignity
and neither is a villain. The battle is shown through impact, dust and
exhaustion, without gore. Notes I've given on earlier work, which still
apply: men are caught mid-action when they look up, never standing in a
row; bronze was precious, so weapons are let go and fall, never thrown;
when I give a note, take it literally.

No real studio marks and no real director's name appear anywhere. The
credits say honestly what was generated and with what.

THE ORDER OF WORK
PLAN.md section 7 has the sequence. In outline:
1. The Thales research in section 6 (launch the subagent with that brief,
   then check its citations yourself before trusting it).
2. Track alignment and beat grid.
3. Remaining fact checks: eclipse geometry at the river, Lydian and Median
   dress and arms, the houses for the departure and the return.
4. The shot-by-shot list, each shot with its timing against the grid, its
   staging spec, and which earlier shot it mirrors in the palindrome.
5. Staging, then bake-offs.
6. An animatic of staged stills against the track.
7. Full generation, edit, grade, sound layer, title and credits card.
8. A small low-resolution preview of the whole thing before any full-size
   render.

WHERE TO STOP FOR ME
Work through research, alignment and fact checks without checking in.
Stop and show me at these points, and wait for my answer:
- after the research and fact checks, with what they change in the plan
- after the shot list is written, before any staging
- before any paid generation: tell me the models, the expected spend for
  the bake-off and for the full run, and get my go-ahead; log every paid
  call and its cost as you go
- after the bake-offs, with the candidates side by side and your pick
- after the animatic
- after the low-resolution preview, before the full-size render

At each stop, tell me what you did, what you verified and what you
didn't, and what is still weak. If a shot isn't working after a few
attempts, say so and propose a different shot, don't keep spending on it.

Keep PLAN.md current as decisions change, and keep the project in a state
where another session could pick it up from the files alone. Don't commit
or push anything unless I ask.
```
