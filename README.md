# AEW Broadcast Novelizer Prompt  
### Section-by-Section Wrestling Show Generator (TTS Chunking + Hidden Twist + Exportable Story Bible)

This repository contains a single, long-form prompt designed to generate a **complete wrestling show in the AEW world** as **fictional entertainment**, written as a **gritty, book-like broadcast novelization**—but delivered in **small, text-to-speech-friendly chunks** so it can be read aloud smoothly and **without spoiling twists**.

The prompt is intended for use with AI chat models (ChatGPT-style assistants). It creates an **interactive “listen/read” experience** where you advance playback with `NEXT READ`, and only generate new story sections with `NEXT`.

---

## What this prompt is for

This prompt is built to:

- Generate a full, TV-realistic wrestling show as narrative fiction:
  - **DYNAMITE**: treated as a **two-hour live TV broadcast**
  - **PPV**: treated as a **longer pay-per-view broadcast** (not forced into two hours)
- Write the output as a **novel/fiction narrative**, not a run sheet and not a screenplay.
- Keep major angles and the late-show twist **secret** by revealing the show **progressively**.
- Provide a **two-layer control system**:
  - **Playback control** (`NEXT READ`) for read-aloud chunking
  - **Story control** (`NEXT`) for moving to the next match/segment
- Maintain internal continuity using a **hidden Story Bible** and export it at the end via `BIBLE`.

---

## Key features

### 1) Novelized broadcast style (not a script)
The show is written like a gritty live-broadcast novelization, including:
- sensory arena detail (crowd noise, lights, tension)
- character-driven narration and interior thoughts (when required)
- commentary woven naturally into prose
- production realism (director cues, camera movement, replays, audio notes)

---

### 2) Spoiler-safe delivery (no outlines, no future card reveals)
The AI is instructed to plan the entire show internally but:
- **never reveal the outline**
- **never reveal the full match card**
- **never hint at future surprises**
- keep the **twist secret** until it happens “on-page” late in the show

---

### 3) Two-layer navigation: `NEXT` vs `NEXT READ`
This prompt separates **creating story** from **reading story**:

- `NEXT`  
  Generates **new story content** by creating the next “section” (a match or a segment).  
  Use this only after the current section is fully read out.

- `NEXT READ`  
  Continues **playback only** of the already-written section.  
  It must **not** create new story content or add new details.

This prevents accidental spoilers and supports a clean read-aloud experience.

---

### 4) Text-to-Speech chunking rules (immersion-friendly)
The output is chunked into small read-aloud segments:

- Target size: **~5 minutes of read-aloud** per response
- Hard limits:
  - **3,500 characters max** (including spaces)
  - **10 paragraphs max**
- Splitting rules:
  - do not split mid-sentence unless absolutely necessary
  - prefer splitting at natural breath points, dialogue lines, or decisive action beats
- The prompt tracks chunk numbers **silently** (no visible “### segment X” labels)
- Every chunk ends with exactly:
  > `(Reply NEXT READ for the next 5-minute segment.)`

When a section ends, the final chunk also includes:
> `—End of this section. Reply NEXT to continue the episode.—`

---

### 5) Random match count per show (kept secret)
Each run chooses a total match count once during planning:

- **DYNAMITE:** random **7–9 matches**
- **PPV:** random **9–10 matches**
- The chosen number is **not revealed** to the user.

Even if the show has more than seven matches, it must still follow a seven-match “pillar spine” for pacing (see below).

---

### 6) “Pillar match spine” (always present)
No matter the match count, the show includes a satisfying seven-part progression:

1. Hot opener (crowd hook)
2. Story-driven contrast
3. Mid-show escalation + first big angle
4. Women’s division spotlight
5. Gimmick/stip or violent grudge
6. Semi-main with consequence (injury can occur here)
7. Main event with major twist + cliffhanger ending

Extra matches (if any) are “bonus matches” that fit around the spine without breaking pacing.

---

### 7) Mandatory TV realism requirements
Across the full show, the prompt requires:
- at least **three break moments** written in prose  
  - Dynamite: commercial break energy  
  - PPV: transition breaks (video packages / sponsor beats / resets)
- at least one **tense sit-down interview** (Renee-style)
- at least one **chaotic backstage brawl/pull-apart**
- production truck flavor (director cues, camera calls, replay decisions)
- crowd POV cutaways (signs, chants, phone videos, shifting loyalties)

---

### 8) Commentary team baked into the prose
The narrative must include:
- **Excalibur** (lead play-by-play)
- **Taz** (heel-leaning color)
- **Jim Cornette** (friction + arguments)

Running gag:
- Cornette occasionally calls Excalibur **“Sockface”** only when it’s funniest.
- Excalibur grows more irritated each time; Cornette knows he’s pushing buttons.

**Safety/quality rule:** trash-talk only — no slurs, protected-class hate, doxxing, or real-world accusations.

---

### 9) Injury system (mandatory) + visceral broadcast framing
At least **two wrestlers** must suffer significant in-match injuries (kayfabe) that matter to the story.

After each injury, the narrative must include:
1) a short **first-person internal monologue** from the injured wrestler  
2) a **broadcast-style medical update** (trainers, stretcher/backboard, replay notes, commentary reaction)  
3) explicit **crowd reaction** (chants, gasps, signs, phones/social-media vibe)

---

### 10) Late-show twist (earned)
The show includes:
- **one major twist late in the show**
- **2–5 subtle breadcrumbs** planted earlier that pay off at the twist  
  (breadcrumbs must be embedded naturally and not labeled)

---

## Continuity system: Hidden Story Bible + export (`BIBLE`)
The prompt forces the AI to maintain an internal “Story Bible” tracking:
- match results
- injuries and medical status
- alliances/turns
- open threads and payoffs
- breadcrumbs planted and resolved

This is **hidden during playback** to preserve immersion and surprises.

After the show ends, you can type:

- `BIBLE`  
  Exports the full Story Bible in a clean, copyable format so you can reuse continuity in future runs.

---

## How to use

1) Copy/paste the full prompt into your AI chat.
2) Choose a show type:
   - `Show Type: [DYNAMITE]` or `Show Type: [PPV]`
3) The AI outputs the first playback chunk of the first section.
4) Use:
   - `NEXT READ` to keep listening/reading the current section
   - `NEXT` only when the section has ended to generate the next one
5) At the end of the show, type `BIBLE` to export continuity.

---

## Commands (quick reference)

| Command | Purpose |
|--------|---------|
| `NEXT READ` | Continue playback of the already-written current section (no new story). |
| `NEXT` | Generate the next section (new match/segment). |
| `BIBLE` | After the finale, export the Story Bible for backup/reuse. |

---

## Disclaimer

This project is intended for **fictional entertainment writing** that emulates the structure and feel of professional wrestling broadcasts in narrative form.  
It is **not affiliated with or endorsed by** any wrestling promotion.
