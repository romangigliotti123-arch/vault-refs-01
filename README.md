# Roblox reference screenshots (vault-refs)

308 frames from 31 popular, high-polish Roblox games (37 folders; phone captures are separate `-mobile` folders), indexed by screen type (HUD, shop, popup, world, lighting, VFX, mobile layout, onboarding, typography) and by quality tag. They are visual-quality references: an AI agent (or a person) compares screenshots of their own game with what good looks like and writes concrete differences.

**Third-party content.** Every image is a frame captured from a public gameplay video of someone else's Roblox game. Nothing here is original work of this repository's owner and no licence is granted: see [NOTICE.md](NOTICE.md) for the credits (game names, video creators), the rights position and how to ask for removal.

Part of the Roblox Dev Mastery Vault (https://github.com/romangigliotti123-arch/vault-kit-01). Built and maintained by Roman (GitHub: romangigliotti123-arch). The vault's setup and `/vault-update` fetch this repository automatically into `~/.claude/claude-kit/roblox-reference/` and point the visual-QA step at it (`claude-kit/tools/refs-sync.py`); by hand: `git clone https://github.com/romangigliotti123-arch/vault-refs-01.git` and open `INDEX.md`.

Files: `INDEX.md` (one line per image: path | game | category | why it is good | tags), `NOTICE.md`, `RESEARCH-best-looking.md` (how the games were chosen), `img/<game>/<nn>-<category>.jpg`.

## Usage and sources

Frames from gameplay footage of popular, high-polish Roblox games, so an agent can compare its own game's screenshots against what good looks like.
Third-party content: for visual comparison and study only (see NOTICE.md). Never copy, trace or re-create these frames in your own game and never ship them with it.

Location: this folder (INDEX.md, README.md, NOTICE.md, img/<game>/<nn>-<category>.jpg). Images are JPEG, width <= 1280.

## How to use
1. Take a screenshot of your own game for the screen you want to judge (HUD, shop, popup, world, lighting, VFX, ...).
2. Read INDEX.md. Grep it by category or rubric tag, e.g. `grep "| menu-shop-inventory |" INDEX.md` or `grep "effects-juice" INDEX.md`.
3. Read 3-6 matching images (mix games; prefer the genre closest to yours: tower-defense-simulator for tower defence, fisch/adopt-me for collecting, pet-simulator-99/bubble-gum-simulator-infinity/steal-a-brainrot for simulators, dress-to-impress/sols-rng/rivals for UI standouts).
4. Compare side by side and write a list of CONCRETE differences: panel style consistency (one corner radius/stroke/font), spacing and overlap, text size at phone width, icon style, colour palette count, lighting/atmosphere, model detail vs bare primitives, VFX and feedback on actions.
5. Fix the differences, re-screenshot, repeat. Each INDEX line says WHY the frame is good; use that as the checklist. Do not copy art or layouts exactly; transfer the principle.

Caveats: all frames come from compressed YouTube video (some 720p). Some games are good only for certain things (see the WHY text, e.g. Blox Fruits HUD text is tiny and dense: use it for VFX/world, not HUD).

## Source videos (attribution; YouTube, all downloaded to a temp folder and deleted after frame extraction)
| game folder | video |
|---|---|
| tower-defense-simulator | https://www.youtube.com/watch?v=LItbo4W3Kw4 (YTDa_corgi, Molten mode, mobile layout) and https://www.youtube.com/watch?v=e6c95H9dUI8 (Halo854, Fallen mode, farm map) |
| fisch | https://www.youtube.com/watch?v=ENfvAH3pCKY (PixelPlayss) |
| pet-simulator-99 | https://www.youtube.com/watch?v=hKdUr4K5c5Q (NightFoxx) |
| adopt-me | https://www.youtube.com/watch?v=PYhugUSKMEM (Riivv3r, Halloween) and https://www.youtube.com/watch?v=atwFjJkawLg (glossie gaming) |
| sols-rng | https://www.youtube.com/watch?v=8ye9KOQWWnE (BachaBlox) |
| bubble-gum-simulator-infinity | https://www.youtube.com/watch?v=nB8OqCIhAos (DinozaurPlays) |
| steal-a-brainrot | https://www.youtube.com/watch?v=vej_kxQwQHE (SkellyPlays) |
| rivals | https://www.youtube.com/watch?v=1OOfL2QjI-0 (Viecti) |
| the-forge | https://www.youtube.com/watch?v=OCyjo7JvaWs (Sebbyastian) |
| dress-to-impress | https://www.youtube.com/watch?v=qkh85RlPZAQ (raspberry, no commentary) |
| grow-a-garden | https://www.youtube.com/watch?v=38P9CZ3givU (Maizen) |
| 99-nights-in-the-forest | https://www.youtube.com/watch?v=f0GlAQWguQw (Roblox Journey) |
| blox-fruits | https://www.youtube.com/watch?v=a4kPP5w4_8U (ZillasPlays) |
| plants-vs-brainrots | https://www.youtube.com/watch?v=VSrzi2VZC6U (Bloxoonrob Plays) |

## Not covered
No frames were kept for Anime-style tower defence (All Star TD looked weak), Escape Tsunami, Bee Swarm, or Dress to Impress's main runway beyond the one video. Add more with the same method (yt-dlp video-only, ffmpeg frames, contact sheet, keep ~8-12 per game).


## Source videos, batch 2 (best-looking research, see RESEARCH-best-looking.md; YouTube, downloaded video-only to a temp folder, deleted after frame extraction)
| game folder | video |
|---|---|
| animal-hospital | https://www.youtube.com/watch?v=W3EFyj7-DFo (TheKacperosEN, walkthrough) |
| ttk | https://www.youtube.com/watch?v=Nwt9fDZvCXE (Shlermski, no commentary) |
| piggy-intercity | https://www.youtube.com/watch?v=8HJyBdrYKRY (Aquapines, part 1) |
| scrapbook-saga | https://www.youtube.com/watch?v=3PQyD6ptiYU (Faded-B, dev battle footage; small creator caption) |
| hellreaver-arena | https://www.youtube.com/watch?v=aGZxfh9bE_8 (Oscar) |
| doors | https://www.youtube.com/watch?v=fbBHD-8cz4Q (FRIM GAMER; faint channel watermark) |
| creatures-of-sonaria | https://www.youtube.com/watch?v=RN18J8AyEn4 (Koopekool) |
| frontlines | https://www.youtube.com/watch?v=Wo6Uhk5Y83I (GameGodzilla1, PC 4K) |
| tower-defense-x | https://www.youtube.com/watch?v=v1UrlqXblyQ (RogueOrdinary, Halloween 2026 run) |
| anime-vanguards | https://www.youtube.com/watch?v=WBxH7vj_V1c (Bcordepic; window capture, taskbar cropped out) |
| jujutsu-shenanigans | https://www.youtube.com/watch?v=NbkLRK4tIpY (FloatyZone; VFX frames only, game is visually plain) |
| fish-it | https://www.youtube.com/watch?v=grs_0-bE6Wc (mayrushart; burned-in creator captions; genre-pattern frames only) |

Batch 2 caveats: footage for these games has no phone-view or portrait video, so mobile-layout is still thin. Frames from TTK, Hellreaver Arena, Frontlines are realistic-style references; Animal Hospital, Piggy: Intercity, Scrapbook Saga and Doors are the best UI/typography/character references.


## Source videos, batch 3 (mobile-layout, onboarding, new games; YouTube, section-downloaded video-only to a temp folder, deleted after frame extraction)
| folder | video |
|---|---|
| rivals-mobile | https://www.youtube.com/watch?v=ZsYA86F6jJk (GodlyWiz, Rivals mobile, 1150x720 source) |
| doors-mobile | https://www.youtube.com/watch?v=7vK3sAcK26E (TapGameplay, Doors mobile walkthrough) |
| sonaria-mobile | https://www.youtube.com/watch?v=PR8fbpfGNNw (chewwy, Creatures of Sonaria on mobile, 1280x592 source; frames without captions only) |
| grow-a-garden-mobile + grow-a-garden/08-11-onboarding | https://www.youtube.com/watch?v=ci21QFQhm-g (GrowAGardenGameplays, iPad Pro, no commentary) and https://www.youtube.com/watch?v=iyf-VkIqg-U (IZHARPOZO, Android phone, no commentary) |
| fisch-mobile | https://www.youtube.com/watch?v=tR8ZcdXyLPY (GuideStream, phone; faint @Guidestream watermark) |
| fisch/11-18 (onboarding, shop) | https://www.youtube.com/watch?v=lDH_7vc9XzA (KaosBlox, Noob to Pro Ep. 1; fresh account tutorial) |
| 99-nights-in-the-forest-mobile + 99-nights-in-the-forest/07-09 | https://www.youtube.com/watch?v=HPngEkBt1VE (TapGameplay, 99 Nights mobile) |
| tower-defense-x/11-14 | https://www.youtube.com/watch?v=rZG70YTKPT4 (Mr. Donut, F2P series part 1; edited video, only clean frames kept) |
| dandys-world | https://www.youtube.com/watch?v=1HRt_HtX9Pc (chomp, alpha-era, no commentary) and https://www.youtube.com/watch?v=UJf8slwBxuY (CIPHER TE ROBLOX, small corner logo in frame 05) |
| forsaken | https://www.youtube.com/watch?v=oQYyzr5aEDs (Bloxoonrob Plays, no commentary) |
| guts-blackpowder | https://www.youtube.com/watch?v=5g8d8PIGkEk (EpicDino, campaign maps, no commentary; very dark/foggy game) |
| livetopia | https://www.youtube.com/watch?v=Otum_HPRaZI (Game Infinity, 4K house tour, no commentary) |
| deepwoken | https://www.youtube.com/watch?v=j0exlAkG7gM (ItzPinguh, Trial of One, no commentary; small UI text) |

Batch 3 notes: tried and rejected (face-cam, hand-cam, meme edits or only lobby footage): Frontlines mobile AwfRhAFa5No (hand-cam overlay + HDR), Fisch mobile TS2clWXqVhk (face-cam), Anime Vanguards AlBUy76oBnI (lobby menus only, nothing new), Guts hT6kzlwF2sI (streamer face-cam), Dead Rails P1RFjxLIFig (lobby waiting only). Dandy's World and Guts & Blackpowder footage is dark; use for card/typography/atmosphere, not general brightness. Folders named <game>-mobile hold phone/tablet touch-HUD frames of games that also have a PC folder.
