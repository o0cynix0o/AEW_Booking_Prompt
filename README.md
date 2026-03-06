# AEW Dynamite Novelizer Prompt (Section-by-Section + Hidden Story Bible)

This repository contains a single, purpose-built prompt designed to generate a **complete, TV-ready, two-hour episode of AEW Dynamite** as **fictional entertainment**, written as a **gritty, book-like “broadcast novelization”**—but delivered **one section at a time** to preserve surprises and twists.

The prompt is intended for use with an AI text model (e.g., ChatGPT-style assistants) and is optimized for an **interactive reading experience** where you reveal the episode progressively by typing `NEXT`.

---

## What this prompt is for

The prompt is built to:

- **Book a full two-hour AEW Dynamite episode** in a way that feels like real weekly wrestling TV.
- Present the show as a **novel/fiction narrative**, not a script, not a run sheet, and not a timestamped format.
- Deliver the story **section-by-section**, so you can read/listen to it in chunks and keep major angles secret until they happen.
- Maintain a **hidden internal continuity system (“Story Bible”)** while you progress through the episode, so events remain consistent and story threads pay off properly.
- Enable exporting that Story Bible at the very end with the command `BIBLE`, so you can carry continuity into a future episode.

---

## What it’s expected to do

Across the full run of the episode, the AI is expected to produce:

### ✅ A complete Dynamite episode written as a novel
The output should read like an immersive broadcast novelization:
- sensory detail (crowd noise, lights, pacing)
- character-driven tone
- interior thoughts when required
- commentary woven naturally into prose
- production realism (truck cues, camera callouts, replays)

### ✅ Exactly 7 matches total
Each match must include in narrative form:
- entrances (arena feel)
- commentary beats integrated into the prose
- **8–15 key spots** (scaled by match importance)
- finish + winner
- aftermath angle that continues the “TV show”

At least **2 matches must advance larger story threads** (not just “great match” filler).

### ✅ TV realism, even in book form
The episode must include:
- **at least 3 commercial break moments**, written as “throw to break / back from break”
- interviews and backstage promos throughout
- at least one tense sit-down interview (Renee-style)
- at least one chaotic backstage interruption / pull-apart

### ✅ R-rated broadcast vibe (within rules)
- strong language and adult intensity
- brutal physicality and blood (framed like a wrestling broadcast)
- no slurs, protected-class hate, doxxing, or real-world accusations

### ✅ Injury and perspective requirements
At least **two wrestlers** must suffer significant in-match injuries (kayfabe) that matter to the story.

After **each** injury, the narrative must include:
1) a short **first-person internal monologue** from the injured wrestler  
2) a broadcast-style **medical update** (trainers, stretcher/backboard, replays, commentary reaction)  
3) explicit **crowd reaction** (chants, gasps, signs, phones/social-media vibe)

### ✅ Commentary team dynamic
The narrative must include:
- Excalibur (lead play-by-play)
- Taz (heel-leaning color)
- Jim Cornette (added for friction)

Running gag:
- Cornette occasionally calls Excalibur **“Sockface”** at the funniest possible moments.
- Excalibur’s irritation escalates over time; Cornette knows exactly what he’s doing.

### ✅ One major twist late in the show
- Must occur in the last ~30 minutes.
- Must recontextualize something earlier.
- Must have **2–5 breadcrumbs** planted earlier (embedded naturally, not labeled).

### ✅ Cliffhanger ending + next-week tease
The final section ends on a cliffhanger and includes a “next week” tease written like the narrator is still in the aftermath.

---

## How it does that (the core mechanisms)

### 1) Section-by-section delivery (no spoilers)
Instead of printing the entire show at once, the AI outputs **one section per response**:
- a full match **or**
- a promo/interview/backstage scene

After each section, the AI stops and prints only:
> `(Type NEXT for the next section.)`

This keeps twists and major angles secret until they happen “on-page.”

### 2) Backend Story Bible (hidden continuity engine)
The prompt requires the AI to maintain a hidden internal “Story Bible” while writing, tracking:
- match results
- injuries and medical status
- alliances/turns
- open story threads
- breadcrumbs and payoffs

Before generating each new section, the AI must silently:
1) update the Story Bible  
2) run a continuity/story-point check  
3) avoid spoiling future developments  

The Story Bible is **not displayed during the episode** so surprise moments remain intact.

### 3) Exportable Story Bible at the end (`BIBLE`)
The prompt includes a command:

- `BIBLE` — **only after the final section**, output the full Story Bible in a clean, copyable format.

This allows you to:
- back up the full episode continuity
- reuse it as the canon starting point for the next “episode” you generate

If the user requests `BIBLE` before the end, the AI should respond that the Bible is locked until the finale and prompt the user to continue with `NEXT`.

---

## How to use

1) Copy the prompt text into your AI chat.
2) Let it generate the first section.
3) Type `NEXT` to continue section-by-section.
4) Continue until the episode ends.
5) When the AI says the episode is over, type `BIBLE` to export the Story Bible.

---

## Commands

| Command | What it does |
|--------|--------------|
| `NEXT` | Generates the next section (match or segment). |
| `BIBLE` | After the episode ends, exports the full Story Bible for backup/reuse. |

---

## Notes & recommended usage

- This prompt is ideal for **text-to-speech listening** because it outputs in manageable chunks and uses clear dialogue.
- If you want to carry continuity into a sequel episode, save the exported `BIBLE` and paste it into the next run as the “previously on / canon state.”

---

## Disclaimer

This prompt is for **fictional entertainment writing**. It is intended to simulate the tone and structure of wrestling television in narrative form.
