# Claude Setup Playbook

Version 2.0.0 · 2026-09-05
Prepared by RG Advisors

This is the order to set up Claude so it is actually useful, and the reasoning behind the order. It goes with `self-interview-claude.md`, which does most of the work for you, and `tune-up-claude.md`, which you will not need for a month.

**If you only read one paragraph:** open Claude, start a new conversation outside any project, paste in the whole of `self-interview-claude.md`, and answer its questions. About thirty minutes. It fixes one privacy setting with you, asks what the tool is for in your work, and writes your instruction files. Come back here afterward for stages 3 to 6, which are the part the interview cannot do for you.

Under two hours, and you can do all of it today. One sitting, start to finish.

**There is nothing to prepare and nothing to answer here.** This is not a worksheet. The interview asks every question that needs asking, most of them as options you pick rather than answers you compose, and it writes the files for you.

---

## The thesis: most people do this backwards

The common sequence is to connect every data source on day one, ask a few broad questions, get generic answers, and conclude the tool is mid.

The tool was fine. It had no idea who you were.

Claude starts every conversation knowing nothing about your firm, your deals, your vocabulary, your standards, or what you have already decided. Connecting it to more data does not fix that. It gives a stranger more filing cabinets.

The correct order is instructions first, access second, automation third. Each stage is only worth doing once the previous one is real.

| Stage | What you configure | Time |
|---|---|---|
| 0 | Account and plan hygiene | 15 min |
| 1 | Personal instructions (how Claude talks to you) | the interview, |
| 2 | Context file (who you are, how the business works) | 30 min for both |
| 3 | Projects (one per durable workstream) | 20 min |
| 4 | Connectors and data access | 20 min |
| 5 | Skills (repeatable procedures) | later, see below |
| 6 | Maintenance loop | 10 min a month |

Stages 0 through 4 are today, in order, in one sitting. Stages 1 and 2 are both handled by the interview in a single pass.

Stage 5 is the exception, and it is the one everybody wants to start with. It does not wait on a calendar. It waits on you having used the thing enough to know what you actually repeat, which is a different kind of readiness than time passing.

---

## Stage 0: account and plan hygiene

Do this before a single real document goes in.

1. **Confirm you are on commercial terms.** Consumer plans and business plans have different data handling. On a personal plan the training and retention controls sit with the individual user, there is no owner, no central billing, and nothing to deactivate when someone leaves. If client or deal material is going to touch it, it belongs on a plan where the organization holds the controls.
2. **Name an owner.** One person who can add and remove seats. On a team of three this feels like ceremony. It is the difference between offboarding taking five minutes and taking a lawyer.
3. **Walk the organization settings once, with the defaults visible.** Look specifically for anything that retains conversation content for feedback or quality review, and decide it deliberately rather than inheriting it. Turn off what you do not want before the first real file is read, not after. On a personal plan there is no organization to walk; the one setting that matters is the training toggle, and the interview's first step is to turn it off with you.
4. **Decide what is out of bounds entirely.** Some categories should never enter any AI tool: credentials and API keys, anything under an NDA that restricts machine processing, personnel and payroll files, resident or applicant records. Write the list down now. It is the shortest and most useful governance document you will ever produce.

Settings interfaces change. Verify the current labels in the product rather than trusting a screenshot in a document.

---

## Stage 1: personal instructions

This is the short block that applies to every conversation you have, on any topic. It answers one question: how should Claude talk to you.

The interview writes it, mostly from options you pick. What follows is so you recognize what you are looking at when it hands you the file.

Keep it under about 20 lines. It loads on every single turn, so every line is paying rent.

What belongs here:

- **Register and length.** Direct and short by default, or thorough and structured. Say which.
- **Formatting rules you actually care about.** Bullet density, tables, headers, whether you hate em dashes, whether emojis are acceptable. Small, but you will notice these on every output for years.
- **The role.** This is the highest-leverage line in the whole file. "Assistant" produces a tool that waits for orders. "Advisor who challenges my thinking and names the risk I am not seeing" produces something different from the same model. Pick deliberately.
- **The lane.** What this tool is for in your work: building finished work, creative exploration, checking, or writing in your voice. If you run a second AI tool, which one owns what. Two tools with no written lane end up doing the same job badly, and this is the line that prevents it.
- **Pushback tolerance.** Whether you want disagreement surfaced or work delivered. If you want to be told you are wrong, you have to say so, in writing, once.
- **How you input.** If you dictate, say so. Dictated text has run-ons and false starts, and Claude should read through them rather than mirror them back.

What does not belong here: anything about a specific deal, project, or entity. That is stage 2.

---

## Stage 2: the context file

This is the durable document describing who you are and how your business works. In a browser or desktop project it goes in the project instructions. In a folder-based tool it is a file named `CLAUDE.md` at the root of the folder. Same content, different surface.

The interview writes this. What matters is understanding what makes one good, because you will be editing it for years.

**Three layers, and they age at different speeds.**

| Layer | Contents | Changes |
|---|---|---|
| Identity | Who you are, the entities, roles, credentials | Yearly |
| Operating rules | Standards, boundaries, what never mixes, vocabulary | Rarely |
| Current focus | Active priorities, what is live right now | Monthly |

Keep them in separate sections and label the third one with a date. A stale current-focus section is worse than none, because it steers confidently toward last quarter.

**The rule that governs every line: if it does not change what Claude does, cut it.**

This is the single most useful editing test. "We value quality and integrity" changes nothing. "Never present a projection without naming the assumption it turns on" changes something. Aspirational language is free to write and costs you on every turn forever.

**Describe intent and conventions, never inventory.**

Do not list the files in a folder. The list goes stale the day you add a file, it burns context on every load, and it is unnecessary because Claude can look. Describe what the folder is for and how things are named. Then new files are handled correctly without anyone updating anything.

**Explain why, not how loud.**

"CRITICAL: YOU MUST NEVER EDIT THE SUBMISSION WORKBOOK" is weaker than "Never write to an agency submission workbook. A tool that can open a file can usually save it, and a saved workbook with silently broken validation looks identical to a correct one until the agency opens it." The second one holds up in situations the first one did not anticipate, because the reasoning transfers.

**Pointers, not copies.**

One fact lives in one place. If a standard is written down somewhere, point at it. Copying it into the instruction file creates two versions that will disagree within a quarter, and you will not know which one is being followed.

**Date it.** Put `Last updated:` at the top. In eight months you will need to know whether to trust it.

Target length: about 150 lines. If you are past 250, the fix is almost never trimming words. It is that reference material belongs in an attached document that gets read when relevant, not in the always-loaded instruction.

---

## Stage 3: projects

A project is a container with its own instructions and its own attached documents. It is the right unit for a durable workstream, not for a task.

- **One project per thing that has a lifespan of months.** A deal. A property. A recurring report. A function of the business.
- **Not one project per question.** That is what a normal conversation is for.
- **Attach the reference material to the project rather than pasting it into the instructions.** Attachments get read when relevant. Instructions get read always. That difference is the whole design.
- **Project instructions layer on top of your personal ones.** They do not replace them. So the project only needs what is specific to it, which is usually much shorter than people expect.

The failure mode is a project per week, each one starting from nothing. If you find yourself re-explaining the same background in a new project, that background belonged in the parent context file.

---

## Stage 4: connectors and data access

Only now. Instructions before access, because a connected tool that does not know your standards produces confident work in the wrong shape, and reviewing that costs more than doing it yourself.

- **Connect from a normal user account, never an administrator account.** These tools generally see exactly what the signed-in person sees. If the signed-in person is an admin, that is a much larger surface with no corresponding benefit.
- **Least privilege is not a slogan here, it is the entire security model.** If the permission structure in your file system is already correct, connecting AI adds no new exposure. If it is not, AI does not create the problem, it makes the problem legible by surfacing files nobody had browsed to in three years.
- **Anything that must never be reachable goes in a separate container, not a subfolder.** A subfolder depends on someone remembering a rule. A separate site or drive that the connected account is not a member of depends on nothing.
- **Test the boundary once, deliberately.** Ask for something it should not be able to see. Confirm it cannot. Write down the date you confirmed it.

---

## Stage 5: skills

A skill is a written procedure Claude follows the same way every time. It is the highest-value thing in the system and the most commonly attempted too early.

**The trigger is a list, not a date.** Before you have run a procedure several times for real, you do not know which parts of it are the procedure and which parts were that one deal. A skill built from imagination encodes the workflow you assume rather than the one you run. It produces one plausible answer shape and then quietly produces the wrong thing when the inputs change.

So the readiness test is simple: can you name three things you have now done more than twice, the same way each time. When you can, you are ready. That might be next week or next month depending on your volume.

The sequence that works:

1. Do the work manually with Claude. Keep a running list of anything you did more than twice.
2. Pick the most repeated one. Run it once more, deliberately, in small steps.
3. Ask Claude to document the decision logic behind what just happened, as if teaching another practitioner. Not the output. The reasoning.
4. Build the skill from that documented process, with the explicit instruction to build from the process and not from the sample output.

Step 3 is the one people skip, and skipping it is what produces a skill that reproduces one answer instead of a way of thinking.

The list starts today. The interview captures the first version of it.

---

## Stage 6: the maintenance loop

Instruction files are not written. They are accumulated.

- **Keep a corrections note.** Every time you correct Claude on something that was not a one-off, write the correction down. Once a month, fold the list into the instruction file. This is where the genuinely good instructions come from. Nobody writes them on day one, because on day one you do not yet know what gets misread.
- **Write the lesson into the file, not just into your head.** A correction that lives only in a conversation dies when that conversation ends.
- **Re-read the whole file quarterly.** Delete what is no longer true. Update the date. The current-focus section will be wrong; that is expected, which is why it is dated and separate.
- **When output quality drops, check the instructions before blaming the model.** The usual cause is a stale current-focus section or a rule that was written for a situation that no longer exists.

`tune-up-claude.md` runs this for you, the same way the interview did. Paste it into a new conversation in about a month with your file handy. It asks what you have been fixing, writes the actual rules from your answers, shows you each one before it goes in, cuts what has gone dead, and hands back the complete revised file.

You are not expected to know how to phrase a rule. Describing the problem is your half of that; the wording is its half.

---

## What this is not

This covers one person and their working context. It does not cover firm-wide file architecture, classification tiers, permission design, incident response, or an AI use policy. Those are separate documents and they are a separate conversation. If several people are about to work in shared files, that conversation should happen before, not after.

---

## Run the interview

Open a new Claude conversation, outside any project. Paste the entire contents of `self-interview-claude.md`. Nothing to prepare, nothing to look up first.

Most of what it asks comes as options you pick. The handful of open questions are the ones only you can answer, and talking through them out loud is fine, dictation included. It will read past the run-ons and pull out what matters. You are not drafting anything; it does the writing.

About 30 minutes, and it produces three things: your personal instruction block, your context file, and a card telling you exactly where to put each one. Each comes out as a single copy-paste block.

Do it in one sitting. The interview builds on your earlier answers, so restarting means repeating yourself.
