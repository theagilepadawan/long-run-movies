# The Long Run — intro and joggers transition

Status: preproduction only. No animated clips have been generated, approved, exported, or integrated. Runway's callable tools were absent from the previous chat's complete tool list, including after the user re-enabled the connection. The underlying app-loading cause was not visible to the agent; there was no Runway API request or credit charge from that work. Recheck the tools in the new chat.

Start with [NEXT-CHAT.md](NEXT-CHAT.md) for the user's requested deliverables and the exact continuation point.

The user requested two films:

- A roughly 8–12 second Lower Manhattan introduction to Nicolai, ending with **THE LONG RUN** and a natural handoff into Opening Bell.
- A roughly 6–8 second transition **after Midtown completion and before Central Park**: the office host presents a shoebox, Nicolai discovers his Park trainers, changes shoes, tightens the laces, tests them, and jogs into the Park.

The new user request governs these films. The earlier handoff's six-scene slate is background material and does not authorize generating the other proposed scenes.

## Prepared material

- `reference-analysis.md`: observed visual treatment of the supplied Fanthomas opening and the adaptation boundaries.
- `shot-plan.md`: a 10.5 second intro and an 8 second shoe transition, including image-to-video motion briefs and editorial transitions. These are production targets, not claims about supported Runway generation durations.
- `references/style-analysis/reference-01.jpg` and `reference-02.jpg`: one-second visual sampling of the user's full approximately 32 second reference video, ordered left-to-right, top-to-bottom. These are inspection sheets, not production frames.
- `storyboards/intro-reference-v001.png`: preliminary Lower Manhattan composition from the image-generation tool.
- `storyboards/joggers-reveal-reference-v001.png`: preliminary office gift-reveal composition from the image-generation tool. This depicts the open-box reveal, not the closed-box opening frame.
- `reference-record.json`: source and generated-frame provenance, measured image sizes and hashes.
- `references/style/Fanthomas-opening.mp4`: the original uploaded animation reference, copied byte for byte.
- `references/source-photos/nicolai-user-reference.png`: Nicolai's supplied likeness photograph from the handoff.
- `references/characters/`, `references/locations/`, `references/gameplay/` and `references/branding/`: the relevant native assets, exact Park footwear atlases, gameplay captures and official branding, copied byte for byte from the handoff.

The two generated stills are **unapproved**. Compare Nicolai's face with the original photograph and native sprites, the host with her native art, and the generated shoes with the exact Park atlas before using either as a production reference. The gift-frame footwear is a conceptual depiction; exact sneaker silhouette and sole profile require another fidelity pass. Do not claim these stills establish animation quality, facial stability through motion, or an exact match to the source shoe design.

## Source authority

The relevant references are committed directly under this folder, so they are available in a fresh checkout. These paths are relative to `production/`:

| Use | Committed reference |
|---|---|
| Nicolai's actual photograph | `references/source-photos/nicolai-user-reference.png` |
| Current Nicolai pose and costume | `references/characters/nicolai-idle.png`, `nicolai-run.png`, `nicolai-formal-atlas.webp` |
| Exact Park footwear | `references/characters/nicolai-park-atlas.webp`, `nicolai-park-flip-atlas.webp` |
| Office host's native character art | `references/characters/office-host-native.png` |
| 505 entrance | `references/locations/505-fifth-native.png` |
| Lower Manhattan and Park | `references/locations/lower-manhattan-wtc.webp`, `central-park-bow-bridge.webp` |
| Actual game composition | `references/gameplay/` |
| Official logo, symbol and fonts | `references/branding/` |

The office host image is generated production art from the handoff, not an original photograph. The original host photographs were not included in that package.

The complete untouched game handoff is committed as `../The-Long-Run-Cutscene-Handoff.zip`. For its source, audio and full documentation, extract it from the repository root with `unzip -n The-Long-Run-Cutscene-Handoff.zip`; `-n` preserves existing extracted files. The following original paths are relative to the resulting `The-Long-Run-Cutscene-Handoff/` directory:

- Nicolai face: `references/source-photos/nicolai-user-reference.png`.
- Nicolai clothes/proportions/formal footwear: `references/characters/nicolai-idle.png`, `nicolai-run.png` and `game/assets/original-27.webp`.
- Exact Park trainers: `game/assets/original-17.webp` and `original-18.webp`. `game/scripts/park-shoes.js` describes navy knit uppers, a white collar and a white midsole. Do not replace them with a generic tennis shoe or a branded alternative.
- Office host: `references/office-host/host-native-source.png`.
- Office architecture: `references/locations/midtown-505-native-source.png`.
- Entry/exit composition: `references/gameplay/downtown-gameplay.png`, `office-gameplay.png`, `central-park-gameplay.png`, and the original approved Park paintings.
- Official NBIM lockup: `game/assets/original-08.svg`; symbol: `original-09.svg`. Preserve their vectors and clear space in postproduction.
- Exact type: packaged Norges Bank WOFF2 fonts (`original-02` through `original-06`).

## Remaining production

Once Runway tools are actually available, inspect their schemas, supported model names, image-reference controls, durations, output sizes and audio behavior. Do not assume an API, supported parameter or model. Prepare individual shot start frames, beginning with a short identity/action proof; do not send a multi-frame contact sheet or full sprite atlas as the scene to animate.

After animation, review the whole clips for likeness drift, foot contact, shoe continuity, fingers, stable doors and frame-to-frame clothing consistency. Deliver clean picture, a review mix, audio stems, first/last frames, posters, contact sheets and actual generation provenance. Add exact title/logo typography in post. Integration into the game remains a separate change: this task has not modified the source or its chapter behavior.
