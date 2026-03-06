# AEW Broadcast Novelizer Prompt  
### Section-by-Section Wrestling Episode Generator (Hidden Twist + Exportable Story Bible)

This repository contains a purpose-built prompt that generates a **complete wrestling “show”** in the AEW world as **fictional entertainment**, written as a **gritty, book-like broadcast novelization**—but delivered **one section at a time** so twists, betrayals, and late-show reveals stay secret until they happen “on-page.”

It’s designed for use with AI chat models (ChatGPT-style assistants) and is optimized for an **interactive read-aloud experience** where you progress through the episode by typing `NEXT`.

---

## What this prompt is for

The prompt is intended to:

- Create a full-length wrestling show:
  - **DYNAMITE** (treated as a two-hour live TV broadcast)
  - **PPV** (treated as a longer pay-per-view broadcast)
- Output the story as **novel/fiction narrative**, not a run sheet and not a screenplay.
- Keep the show **spoiler-free** by generating it **section-by-section**.
- Maintain internal continuity using a **hidden Story Bible** (not shown during the episode).
- Allow you to export that Story Bible at the end via a command so you can **carry continuity into future episodes**.

---

## What it’s expected to do

### ✅ 1) Write the show like a “broadcast novel”
The output reads like a novelized live broadcast:
- immersive sensory detail (crowd noise, lighting, pacing, tension)
- character-driven tone with interior thoughts where appropriate
- commentary woven naturally into prose
- production realism (director cues, camera choices, replays, audio notes)

It should feel like you’re inside the arena **and** inside the broadcast.

---

### ✅ 2) Output ONE section at a time (no spoilers)
Instead of dumping the entire show, the AI outputs **one section per response**, then stops.

A **section** is either:
- one full match (entrances → action → finish → aftermath), or
- one promo/interview/backstage scene (dialogue + production realism)

After each section, the AI prints only:
> `(Type NEXT for the next section.)`

This preserves surprise reveals and late-show twists.

---

### ✅ 3) Random match count per show (secret to the reader)
The prompt secretly determines the number of matches during planning and **does not reveal the total**:

- **DYNAMITE:** random total matches **7–9**
- **PPV:** random total matches **9–10**

This makes each run feel like a real card where pacing can vary without breaking structure.

---

### ✅ 4) Seven “pillar match” spine (always present)
Even when total matches exceed 7, the show must still follow a satisfying progression using these seven pillar match roles:

1. Hot opener (crowd hook)
2. Story-driven contrast match
3. Mid-show escalation + first big angle
4. Women’s division spotlight
5. Gimmick/stip or violent grudge match
6. Semi-main with consequence (injury may happen here)
7. Main event with major twist + cliffhanger ending

If total matches are higher, the additional matches are treated as **bonus matches** that fit around the pillar spine.

---

### ✅ 5) Commentary team built into the prose
The narrative must include an active commentary presence:
- **Excalibur** (lead play-by-play; tries to keep it professional)
- **Taz** (heel-leaning color; loves technique + chaos)
- **Jim Cornette** (added for friction)

Running gag:
- Cornette occasionally calls Excalibur **“Sockface”** only when unexpected and funniest.
- Excalibur gets more irritated each time; Cornette knowingly pokes him.

**Important:** Insults are limited to spicy comedic trash-talk (no slurs, no protected-class hate, no doxxing, no real-world accusations).

---

### ✅ 6) Broadcast pacing + “break moments” in prose
The prompt requires at least three “broadcast break moments,” written in novel form:

- For **DYNAMITE**: commercial break energy (throw to break + back from break)
- For **PPV**: transition breaks (video packages, sponsor beats, desk resets) written with the same cliffhanger/snap-back feeling

---

### ✅ 7) Interviews, backstage promos, and chaos
Across the full show, the AI must include:
- at least one tense sit-down interview (Renee-style) with dialogue
- at least one chaotic backstage interruption / brawl / pull-apart  
  (producers yelling, security swarming, camera scramble)

---

### ✅ 8) R-rated intensity (broadcast-framed)
The show should feel adult, intense, and brutal:
- strong language
- hard physicality
- blood is allowed (framed like sports-entertainment broadcast with replays and medical response)

---

### ✅ 9) Injury requirements (mandatory)
At least **two wrestlers** must suffer significant in-match injuries (kayfabe) that matter to the story.

After **each** injury, the narrative must include:
1) a short **first-person internal monologue** from the injured wrestler  
2) a **broadcast-style medical update** (trainers, stretcher/backboard/splint, replays, commentary reaction)  
3) explicit **crowd reaction** (chants, gasps, signs, phones/social-media vibe)

---

### ✅ 10) One major late-show twist (earned)
The show must include:
- **one major twist late in the show** (last portion)
- **2–5 subtle breadcrumbs planted earlier** that pay off when the twist hits  
  (breadcrumbs must be embedded naturally and not labeled)

The twist must **remain secret** until it happens.

---

## How it maintains continuity (Hidden Story Bible)

The prompt requires the AI to keep an internal, continuously updated **Story Bible** tracking:
- match results
- injuries and medical status
- alliances/turns
- open threads and payoffs
- breadcrumbs planted and resolved

Before generating each new section, the AI must silently:
1) update the Story Bible  
2) run a continuity/story-point check  
3) avoid spoiling future developments  

The Story Bible is **not shown during the episode**, so surprises stay intact.

---

## Exporting the Story Bible (`BIBLE`)

At the end of the show, you can type:

- `BIBLE`

The AI will output the full Story Bible in a clean, copyable format so you can:
- back up the canon of the episode
- reuse it as continuity for a future episode run

If you try `BIBLE` before the show ends, the prompt instructs the AI to keep it locked until the finale.

---

## Commands

| Command | What it does |
|--------|--------------|
| `NEXT` | Generates the next section (match or segment). |
| `BIBLE` | After the show ends, exports the full Story Bible for backup/reuse. |

---

## How to use

1) Copy the prompt into your AI chat.
2) Set `Show Type` to `DYNAMITE` or `PPV`.
3) Let the AI generate the first section.
4) Type `NEXT` repeatedly to progress section-by-section.
5) When the show ends, type `BIBLE` to export the Story Bible.

---

## Notes / Best Practices

- This prompt is built for **read-aloud / text-to-speech**: section sizes are manageable, and dialogue is clear.
- For match pacing, the prompt scales “key spots” by match type:
  - squash/sprint: 3–6
  - standard TV: 6–10
  - feature/main: 10–15  
- For future episodes, paste the exported `BIBLE` back into a new run as the canon starting state.

---

## Disclaimer

This project is intended for **fictional entertainment writing** and storytelling. It generates a stylized narrative inspired by wrestling broadcast structure. It is not affiliated with, endorsed by, or produced by any wrestling promotion.
