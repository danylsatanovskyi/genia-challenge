# Personal AI Assistant (CLI)

A command-line Personal AI Assistant written in **Python 3.12** that uses the **OpenRouter API** to provide multiple interactive AI-powered capabilities through a simple menu-driven interface.

---

## Features

- **Code Explainer**
- **Language Translator**
- **Recipe Suggester**
- **Supportive Coach**
- **Mock Interviewer**
- **Debate Partner (Devil's Advocate)**

All features run locally via the command line.

---

## Technical Requirements

- Python **3.12** (latest stable recommended)
- OpenRouter API key
- Internet connection

---

## Installation

```bash
git clone https://github.com/danylsatanovskyi/genia-challenge.git
cd genia-challenge
python -m venv .venv
source .venv/Scripts/activate
pip install -r requirements.txt
```

---

## Environment Setup

```bash
cp .env.example .env
```

Edit `.env`:

```env
OPENROUTER_API_KEY=your_real_api_key_here
```

⚠️ **Never commit your `.env` file.**

---

## Running the Application

```bash
python assistant.py
```

---

## Example Usage (Feature Chats)

### 1️⃣ Code Explainer

**User**
```
**Choose an option: 1**

**Paste code to explain. Enter snippet.**

**for i in range(5):**
**    print(i)**

**DONE**
```

**Assistant**
```
This code loops from 0 to 4 and prints each number on a new line.
The range(5) function generates five values starting at 0.
```

---

### 2️⃣ Language Translator

**User**
```
**Choose an option: 2**

**Language Translator**
**Type DONE to finish entering text.**
**Type QUIT on a new line to exit.**

**Source language (e.g., English, French, Spanish) or 'auto': english**
**Target language (e.g., English, French, Spanish): french**

**Enter the text you want to translate.**
**i love you so much**

**DONE**
```

**Assistant**
```
------------------------------------------------------------
TRANSLATION
------------------------------------------------------------
je t'aime tellement
------------------------------------------------------------
```

**User**
```
**Source language (e.g., English, French, Spanish) or 'auto': spanish**
**Target language (e.g., English, French, Spanish): english**

**Enter the text you want to translate.**
**hola como estas**

**DONE**
```

**Assistant**
```
------------------------------------------------------------
TRANSLATION
------------------------------------------------------------
Hello, how are you?
------------------------------------------------------------
```

---

### 3️⃣ Recipe Suggester

**User**
```
**Choose an option: 3**

**Recipe Suggester**
**Enter ingredients (one per line). Type DONE to finish a set.**
**Type QUIT on a new line to exit.**

**Enter ingredients for this request:**
**fish and chips**

**DONE**

**Cuisine preference (optional, e.g., Italian, Asian, none): asian**
**Max cooking time (optional, e.g., 15 min, 30 min, none): 30 min**
**Dietary constraints (optional, e.g., vegetarian, halal, none): vegetarian**
```

**Assistant**
```
------------------------------------------------------------
RECIPE IDEAS
------------------------------------------------------------

### 1) Korean Gochujang Tofu "Fish" & Chips Bowl

**Why it fits:** Asian flavors (gochujang, sesame), **vegetarian** (tofu replaces fish), and ready fast with pre-cooked/oven chips.

**Ingredients used:** chips (fries). *(Fish is skipped for dietary preference.)*

**Other common ingredients:** firm tofu, nori (seaweed sheets), gochujang, soy sauce, rice vinegar (or lemon), sugar, garlic, sesame oil, scallions, sesame seeds.

**Steps (6):**
1. Pat tofu dry; cut into thick "fillet" slabs. Press a strip of nori onto each slab (use a little water to help it stick).
2. Pan-fry tofu in a little oil 3–4 min per side until golden.
3. In a bowl, mix gochujang + soy sauce + vinegar + pinch sugar + minced garlic + a few drops sesame oil.
4. Toss hot chips in a little of the sauce (or drizzle over).
5. Brush remaining sauce onto tofu and warm 30–60 sec in the pan.
6. Serve chips and tofu together; top with scallions + sesame seeds.

---

### 2) Japanese-Style Curry Chips with Crispy Tofu Katsu

**Why it fits:** Japanese curry vibe, **vegetarian**, comforting, and quick using curry roux or powder.

**Ingredients used:** chips (fries). *(Fish is skipped.)*

**Other common ingredients:** firm tofu, Japanese curry roux (or curry powder), onion (optional), vegetable stock/water, soy sauce, cornstarch/flour, breadcrumbs (optional).

**Steps (6):**
1. Heat chips (oven/air fryer) or re-crisp in a pan.
2. Slice tofu into slabs; pat dry. Coat with cornstarch (or flour), then crumbs if you have them.
3. Pan-fry tofu 3–4 min per side until crisp and golden; slice into strips.
4. Simmer curry: sauté onion (optional), add water/stock, dissolve curry roux (or stir in curry powder + a little soy).
5. Simmer 5–8 min until thick.
6. Plate chips, pour curry over, top with tofu katsu.

---

### 3) Thai-Style Sweet Chili Lime Chips + Tofu

**Why it fits:** Thai-style sweet/sour/spicy, **vegetarian**, and very fast (mostly tossing + quick fry).

**Ingredients used:** chips (fries). *(Fish is skipped.)*

**Other common ingredients:** tofu, sweet chili sauce, lime (or lemon), soy sauce, garlic, cilantro (optional), crushed peanuts (optional).

**Steps (5):**
1. Crisp chips in oven/air fryer or a hot pan.
2. Pan-fry cubed tofu in a little oil until browned.
3. Mix sweet chili sauce + lime juice + splash soy sauce + minced garlic.
4. Toss hot chips with half the sauce; toss tofu with the rest.
5. Serve together; top with cilantro/peanuts if you have them.

---

### 4) Chinese Salt-and-Pepper Chips with Seaweed Tofu

**Why it fits:** Takeout-style salt-and-pepper flavor, **vegetarian**, and cooks quickly.

**Ingredients used:** chips (fries). *(Fish is skipped.)*

**Other common ingredients:** tofu, nori (optional), garlic, scallions, chili flakes (optional), five-spice (optional), salt, black pepper.

**Steps (6):**
1. Crisp chips.
2. Cube tofu; pat dry. Pan-fry until golden on multiple sides.
3. Add minced garlic + sliced scallions to the pan for 30–60 sec.
4. Add chips and toss everything together.
5. Season generously with salt + lots of black pepper (and chili flakes/five-spice if you like).
6. Crumble a little nori over the top for a "sea" note, then serve.

If you tell me whether your "chips" are thick-cut fries, crisps (potato chips), or leftover takeaway fries, I can tailor the steps for best crunch in under 30 minutes.

------------------------------------------------------------
```

---

### 4️⃣ Supportive Coach

**User**
```
**Choose an option: 4**

**Supportive Coach (non-clinical)**
**Talk about what's on your mind. Type DONE to send a message.**
**Type QUIT on a new line to end the session.**

**ive been overwhelmed with school**
**i feel very tired**

**DONE**
```

**Assistant**
```
------------------------------------------------------------
That sounds really heavy. When school starts to feel like it's piling up from every direction, it can be exhausting and hard to know where to begin.

A few gentle things that often help in the moment:

- **Do a quick "brain dump" (5 minutes):** Write everything you're worried about—assignments, tests, emails, even small tasks. Getting it out of your head can lower the pressure.

- **Pick just one "next step":** Choose the smallest action you can do in 10–15 minutes (e.g., open the doc, outline 3 bullet points, skim the rubric). Momentum matters more than motivation.

- **Use a short reset:** Try 3 slow breaths, a glass of water, or a 2-minute stretch. It sounds simple, but it can bring your stress down enough to focus.

- **Make it easier on yourself:** If you can, aim for "good enough" on lower-stakes tasks and save your best energy for what matters most.

If it's possible, **loop someone in**—a friend/classmate, a teacher, or an academic advisor. Even just asking for an extension or clarification can lighten the load.

Two questions to help me tailor this:
1) What's overwhelming you most right now—**too many assignments, difficulty concentrating, pressure to get high grades, or something else**?
2) Do you have any **deadlines in the next 48 hours**?

------------------------------------------------------------
```

**User**
```
**i have a lot of deadlines**

**DONE**
```

**Assistant**
```
------------------------------------------------------------
That makes sense—when multiple deadlines stack up, it can feel like you're constantly behind no matter how hard you work. Let's switch into "triage" mode so you're not carrying it all at once.

### Quick triage (15 minutes)

1) **List every deadline** (even roughly): task + due date/time + how much it's worth (if you know).

2) **Mark each task with one label:**
   - **Urgent:** due in 0–2 days
   - **Soon:** due in 3–7 days
   - **Later:** 8+ days

3) For the **Urgent** ones, choose:
   - **1–2 "must-submit" items** (highest impact / strictest deadlines)
   - **1 "quick win"** (something you can finish in under 30–45 min)

### Then work in short blocks

- Do **25 minutes work + 5 minutes break** (or 15/5 if you're fried).
- Your goal for each block is a **tiny deliverable** (e.g., "write intro paragraph," "solve 3 problems," "make outline," "find 2 sources").

### If it's truly too many to finish

- **Email instructors/TAs today** with a simple note: what you're working on + ask about an **extension, partial credit, or prioritizing what matters most**. This can reduce pressure fast, even if not everyone says yes.

### Tiny stress-lowering reset (2 minutes)

Before the next block: feet on the floor, slow exhale, sip of water. You're trying to lower the "alarm" enough to think clearly.

Two quick questions so I can help you prioritize:
1) What are the **next 3 deadlines** (task + when due)?
2) About how many hours do you realistically have to work between now and the first one?

------------------------------------------------------------
```

**User**
```
**thanks!**

**DONE**
```

---

### 5️⃣ Mock Interviewer

**User**
```
**Choose an option: 5**

**Mock Interviewer**
**Answer the questions. Type DONE to submit each answer.**
**Type QUIT on a new line to end the interview.**

**Role you're interviewing for (e.g., SWE intern, analyst, none): swe**
**Focus (behavioral/technical/mixed, default=mixed): technical**
```

**Assistant**
```
------------------------------------------------------------
You're given an array of integers `nums` and an integer `k`. Return the `k` most frequent elements.

- What approach would you use, and what are the time and space complexities you're targeting?
------------------------------------------------------------
```

**User**
```
**Your answer:**
**i dont know... i didnt study ughhh**

**DONE**
```

**Assistant**
```
------------------------------------------------------------
- You were honest about uncertainty, which is good in an interview setting.
- Right now there's no structure to your response yet—let's break the problem down.
- Next time, even if unsure, try proposing a starting point (e.g., "I'd count frequencies with a hashmap").

Next question:

How would you compute the frequency of each number in `nums`, and what would the time and space complexity of that step be?
------------------------------------------------------------
```

**User**
```
**Your answer: [it continues like this]**
```

---

### 6️⃣ Debate Partner (Devil's Advocate)

**User**
```
**Choose an option: 6**

**Debate Partner (Devil's Advocate)**
**State an opinion or claim to debate. Type DONE to submit each message.**
**Type QUIT to end the debate.**

**Your initial claim:**
**messi is the best soccer player in the world**
**He beats everybody!! !!!!**

**DONE**
```

**Assistant**
```
------------------------------------------------------------
That depends on what you mean by "best," and on *when* you're evaluating it.

**If you mean peak ability (all-time/prime):**
Messi has one of the strongest cases ever—elite dribbling under pressure, chance creation, playmaking, scoring, consistency, and longevity. By many analytic measures (non-penalty goals + assists, chances created, progressive carries, etc.) across a very long span, he's extraordinary.

**If you mean best *right now* (current season, current physical level):**
that's much harder to defend, because he's not playing in a top European league anymore and isn't facing the same week-to-week level of opposition. "Best in the world" claims usually assume comparable competitive environments.

**Also, "best" can mean different roles:**
- **Most complete attacker/creator:** Messi has a strong claim historically.
- **Most dominant goal scorer right now:** you could argue for someone like Haaland (if you value finishing/volume) or other top forwards depending on form.
- **Most impactful overall in elite competitions today:** that might point to different players depending on metrics and context (minutes, league strength, Champions League performance, etc.).

So I'd challenge your claim on one key assumption: **are you saying Messi is the best *player alive*, the best *at his peak*, or the best *currently*?** And what criteria matters most to you: trophies, stats, "eye test," difficulty of competition, or all-around influence on matches?

------------------------------------------------------------
```

**User**
```
**Your response:**
**yes most ballon dors**

**DONE**
```

**Assistant**
```
------------------------------------------------------------
Most Ballon d'Ors is strong evidence of *historical greatness*, but it doesn't automatically settle "best soccer player in the world" unless you equate **best = most awarded by that specific vote**.

A few reasons the Ballon d'Or count isn't a clean proof:

- **It's a vote, not a measurement.** Media narratives, timing, and storylines matter (World Cup years, "career achievement" vibes, etc.).

- **Era and competition effects.** Messi and Ronaldo concentrated wins in a period where they were clearly the two dominant stars; other eras had more vote-splitting among multiple greats.

- **Team/context matters.** Individual awards are influenced by team trophies, teammates, and role. A defender or midfielder can be "best" in impact yet rarely win.

- **Definition mismatch.** Ballon d'Or mostly captures "most outstanding that year," not "best player overall," and definitely not "best right now."

So: **Ballon d'Ors support "Messi has the best all-time résumé,"** but they don't by themselves prove he's **currently** the best player in the world.

To pin your claim down: are you arguing
1) **Messi is the greatest of all time (GOAT)** because he has the most Ballon d'Ors, or
2) **Messi is the best player today** because he has the most Ballon d'Ors?

And would you still say "best" if another player were currently better week-to-week but had fewer career awards?

------------------------------------------------------------
```

**User**
```
**Your response: [and so on]**
```