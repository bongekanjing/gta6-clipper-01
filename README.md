# GTA 6 Clipper — Vice City Speedboat Short

Entry for make.fun's `gta6-clipper-01` bounty: clip GTA 6 for the most
YouTube views. Places go by the video's views; the top 20 share $500.

## The clip

A 30-second vertical Short cut from GTA 6 open-world gameplay
(`GTA 6 Open World Gameplay on PS5 Slim`, Testing Games):
a speedboat run across the bay toward the Vice City skyline, 598–628s
of the source video. It opens mid-motion — wake, speed, sun on the
water, skyline ahead — because the first seconds decide whether a
viewer stays.

The last 8 seconds carry make.fun's pitch on screen:

> Make clips like this with AI and earn money on make.fun
> make.fun/bounty/gta6-clipper-01

The rendered clip is `clip/gta6-vice-city-boat-short.mp4`
(1080x1920, 30s, H.264 + AAC). It was cut and rendered with ffmpeg
in the agent session that built this entry: trimmed to the moment,
blur-filled to vertical 9:16, hook text up top for the first 4 seconds,
pitch text over the last 8.

## The video

`VIDEO.json` at the repository root names the video's address on
YouTube. The video is published public as a Short, its description
carrying the bounty's line and the entrant's play code:

> Made by my AI agent for a $500 bounty on make.fun, where you can earn
> money making clips with AI: https://make.fun/bounty/gta6-clipper-01

## The program

`main.ts` (Node 22, standard library only) copies `VIDEO.json` to
`/output/VIDEO.json`. That is all it has to do — the house reads the
video itself through the YouTube Data API and ranks the entry by its
views.

Run it the way the grader does:

```
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Upload notes

See `UPLOAD.md` for the clip's title, description and upload steps.
