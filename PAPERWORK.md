# Paperwork

**AI handles the paperwork. You handle the humans.**

Paperwork builds your personal management second brain — a system of files, commands, and frameworks tailored to how *you* manage. It interviews you about your world, your rhythm, your tools, and your philosophy, then generates everything you need to run your team with AI as your copilot.

This isn't a template you fill in. It's a conversation that builds a system.

---

## How It Works

Run this skill with any AI coding agent (Claude Code, OpenClaw, Cursor, etc.). It will walk you through a conversation, then generate your management brain in the current directory.

**Time:** 15-20 minutes for the interview. Generation is instant.

**What you get:**
- A directory structure for every person you manage and every key relationship
- An instructions file (CLAUDE.md) that teaches your AI how you manage
- Slash commands personalized to your workflow and tools
- Question banks tuned to your management philosophy
- A signal framework for catching problems early
- A git repo ready to use (if you want version control)

---

## The Interview

When invoked, conduct the interview below. Be conversational, not robotic. Ask follow-ups when answers are interesting or vague. Skip questions that don't apply based on previous answers. The goal is to understand how this person actually manages — not to fill out a form.

**Important:** Don't ask all questions at once. Group them naturally. Let the conversation flow. If they give a rich answer, dig in before moving on.

### Part 1: Your World

Start here. Understand the shape of their job.

- What's your role and title?
- How many people report directly to you?
- What kind of roles do they hold? (engineers, designers, PMs, mixed?)
- Do you manage other managers, or is everyone an individual contributor?
- Any key cross-functional partners you meet with regularly? (PMs, designers, other leads)
- Do you have a manager or skip-level relationship you want to track?
- How big is the company? What stage? (startup, growth, enterprise)
- How long have you been in this role?

### Part 2: Your Rhythm

Understand their cadence and rituals.

- How often do you do 1-on-1s? (weekly, biweekly, monthly, it depends)
- How long are they typically?
- Whose agenda is it — yours, theirs, or shared?
- Do you have any recurring team rituals? (standups, retros, planning sessions, weekly updates)
- Do you write a weekly update or status report for your team or leadership?
- Do you do formal performance reviews? How often? (quarterly, biannual, annual)
- Any planning cadence? (sprints, cycles, quarters)
- What does a typical week look like for you?

### Part 3: Your Tools

Understand their ecosystem so the system integrates naturally.

- Where does your calendar live? (Google, Apple, Outlook)
- Where do your notes currently live? (nowhere, Apple Notes, Notion, Google Docs, Obsidian, scattered)
- Do you use a task manager? (Things, Todoist, Linear, Jira, Asana, pen and paper, nothing)
- Do you record meetings? (Granola, Otter, Fireflies, nothing — just pay attention)
- What does your team use for project/work tracking? (Linear, Jira, GitHub Issues, Shortcut, Asana)
- What's the team communication tool? (Slack, Teams, Discord)
- Does your team use GitHub, GitLab, or something else for code?
- Any other tools that are core to your daily work?

### Part 4: Your Philosophy

This is the most important section. Take your time here.

- What matters most to you as a manager? (If you could only do one thing well, what would it be?)
- How do you think about your role — are you more coach, shield, connector, strategist, or something else?
- When you're at your best as a manager, what does that look like?
- What signals do you watch for that tell you someone is struggling? Thriving?
- How do you think about feedback — do you give it in the moment, save it for 1-on-1s, both?
- Where do you fall on the mentorship vs autonomy spectrum? Does it depend on the person?
- How do you handle performance issues? What's your general approach?
- What's your communication style with your team? (direct, gentle, Socratic, depends)

### Part 5: Your Pain

Understand what's broken so the system solves real problems.

- What falls through the cracks most often?
- What do you wish you remembered between 1-on-1s?
- Where do you feel least prepared as a manager?
- What would make performance review season less painful?
- Is there anything about managing that you actively dread or avoid?
- If you had a perfect assistant who knew everything about your team, what would you ask them every morning?

---

## Generation

After the interview, generate the entire management brain. Don't ask for confirmation on every piece — just build it. They can adjust later. The goal is a working system they can start using immediately.

### Step 1: Create the Directory Structure

Based on the interview, create directories for every relationship type they mentioned.

```
[repo-root]/
├── CLAUDE.md                    # AI instructions (always generated)
├── people/                      # Direct reports (always generated if they have reports)
│   └── [template-person]/
│       ├── profile.md
│       ├── one-on-ones.md
│       └── feedback.md
├── journal/                     # Daily thinking and recaps (always generated)
│   └── [YYYY]/
├── references/                  # Question banks, frameworks (always generated)
│   ├── question-bank.md
│   ├── signal-framework.md
│   └── feedback-guide.md
├── [partners/]                  # Cross-functional partners (if mentioned)
│   └── [template-person]/
│       ├── profile.md
│       ├── one-on-ones.md
│       └── feedback.md
├── [leadership/]                # Upward relationships (if mentioned)
│   └── [template-person]/
│       ├── profile.md
│       ├── one-on-ones.md
│       └── feedback.md
├── [meetings/]                  # Non-1-on-1 meeting logs (if they record meetings)
│   └── [YYYY]/
├── [weeklies/]                  # Weekly updates (if they write them)
│   └── [YYYY]/
└── .claude/commands/            # Slash commands (always generated)
    ├── prep.md
    ├── log.md
    ├── health.md
    ├── think.md
    └── [additional commands based on interview]
```

**Conditional directories:**
- `partners/` — only if they mentioned cross-functional relationships
- `leadership/` — only if they want to track upward relationships
- `meetings/` — only if they record meetings or want to log non-1-on-1s
- `weeklies/` — only if they write weekly updates

**Template person directories:** Create one example directory (e.g., `people/example-person/`) with properly formatted template files. They'll duplicate this for each real person.

### Step 2: Generate CLAUDE.md

This is the brain of the system. It teaches the AI how this person manages.

Write a CLAUDE.md that includes:

**About the Manager:**
- Their role, team size, company context
- Management philosophy (in their words, refined)
- Communication style
- What they care about most

**1-on-1 Approach:**
- Cadence and duration
- Whose agenda it is
- What they want to get out of 1-on-1s

**Directory Structure:**
- Explanation of each directory and what goes where
- File formats with templates for each file type (profile.md, one-on-ones.md, feedback.md)
- Relationship types and how behavior adapts for each

**Signal Framework:**
- Red/yellow/green flags based on what they said they watch for
- Cross-referencing rules
- When to escalate

**Performance Framework:**
- How they think about performance (from the interview)
- Review cadence and approach
- How feedback gets tracked

**Tool Integrations:**
- Calendar details (which provider, how to access)
- Meeting recording tool (if any)
- Project tracking tool
- Task manager
- Communication tool
- Include MCP tool references or CLI commands where applicable

**Privacy & Sensitivity:**
- Standard guidelines about handling people data
- Adapted to their stated approach

**Git Workflow:**
- Auto-commit after logging notes
- Simple commit messages
- Main branch is fine for personal repos

### Step 3: Generate Slash Commands

Every manager gets these core commands. Adapt the implementation based on their tools and rhythm.

**Always generated:**

`/prep [name]` — Prepare for a 1-on-1.
- Read their profile, recent 1-on-1 notes, feedback log
- If they use a project tracker: pull recent activity for that person
- If they use GitHub/GitLab: pull PR/review activity
- Generate: pulse assessment, narrative summary, signals, promises made, contextual questions
- Adapt output based on relationship type (report vs partner vs leadership)

`/log [name]` — Log notes from a 1-on-1.
- If they have a meeting recorder: auto-pull and smart-merge
- If not: prompt for manual notes
- Auto-detect signals from the conversation
- Extract action items (theirs and the manager's)
- Stage the manager's commitments to the journal
- Cross-reference names mentioned to other people's feedback files
- Prepend to one-on-ones.md, commit

`/health` — Team health overview.
- Calculate meeting cadence for each person (flag overdue based on their stated cadence)
- Surface outstanding action items they owe people
- List unresolved signals
- Recommend who to prioritize

`/think [topic]` — Thinking space.
- Dump an idea, get genuine pushback
- Stress-test assumptions, explore second-order effects
- Capture refined thinking to journal
- Always generated — every manager needs a thinking space

`/review [name]` — Draft a performance review.
- Synthesize all 1-on-1 notes from the review period
- Pull feedback log entries
- Surface patterns and signals
- Generate a draft review (adapted to their review framework)
- Only generate if they do formal reviews

`/feedback [name]` — Log feedback given or received.
- Capture feedback in the moment
- Whether they gave it or received it about someone
- Log to the person's feedback.md
- Only generate as standalone if they prefer explicit feedback logging (otherwise fold into /log)

**Conditionally generated:**

`/sod` — Start of day briefing.
- Pull tasks from their task manager (if they use one)
- Check calendar for today's 1-on-1s
- Run /prep in parallel for each
- Generate a briefing
- Only if they expressed interest in daily bookends or "what would you ask your assistant every morning" resonated

`/eod` — End of day recap.
- Pull activity from project tracker
- Brain dump / reflection prompt
- Triage staged action items to task manager
- Plan tomorrow
- Only if they want daily bookends

`/sync` — Batch process meetings.
- Find all unlogged meetings from recorder
- Route 1-on-1s to people directories, others to meetings/
- Only if they use a meeting recorder

`/weekly` — Write weekly update.
- Recap the week's 1-on-1s and activity
- Draft their weekly update
- Only if they write weekly updates

`/velocity` — Team activity dashboard.
- Pull PR/commit/review activity for the team
- Flag low output or bottlenecks
- Only if the team uses GitHub/GitLab

`/new [name]` — Bootstrap a new person's directory.
- Create profile, one-on-ones, feedback files from templates
- Always generated if they manage people

`/coach [name]` — Prepare for tough feedback.
- Structure raw thoughts into talking points
- Use the feedback guide framework
- Generate opening, examples, success criteria
- Only if they expressed that feedback delivery is a pain point

### Step 4: Generate Question Banks

Create `references/question-bank.md` with questions organized by category. Base these on their stated philosophy and pain points.

**Categories to include:**
- Team dynamics & collaboration
- Workload & sustainability
- Blockers & support
- Communication & feedback
- Personal growth & learning
- Performance signals (indirect)

**For cross-functional partners (if applicable):**
- Project alignment
- Engineer/team feedback
- Process & communication
- Strategic alignment

**For leadership (if applicable):**
- Strategic context
- Feedback & growth
- Alignment & priorities
- Escalations & decisions

**Add an oddball bank** — 10-15 unexpected questions that break the routine and build real connection. These should feel authentic to the manager's personality based on the interview.

**Weight the banks** toward their stated pain points. If they said "I never know what to ask about career growth," that section gets extra depth.

### Step 5: Generate Signal Framework

Create `references/signal-framework.md` based on what they said they watch for.

Structure:
- 🚩 **Red flags** (immediate attention) — derived from their answers about struggling signals
- ⚠️ **Yellow flags** (monitor closely) — early warning signs they mentioned
- ✅ **Positive signals** (celebrate & reinforce) — what thriving looks like to them
- **Cross-referencing rules** — when someone's name comes up in another person's notes
- **Escalation triggers** — when flags become action items

### Step 6: Generate Feedback Guide

Create `references/feedback-guide.md` adapted to their feedback style.

Include:
- Their stated approach to feedback (from the interview)
- A simple framework for structuring tough conversations
- How to document feedback before and after
- Common deflection responses and how to handle them
- Templates for different feedback scenarios

### Step 7: Generate Template Files

For the example person directory, create properly formatted templates:

**profile.md:**
```markdown
# [Full Name]

**Title:** [Role/Level]
**Start Date:** [When they joined]
[Tool handle fields based on their tools — e.g., GitHub, Linear, Jira]

## Context
[Background, current projects, what they're working on]

## Working Style
[How they like to be managed, communication preferences]

## Strengths
- [Observed strengths]

## Growth Areas
- [Areas for development]

## Notes
[Personal context, interests, anything worth remembering]
```

**one-on-ones.md:**
```markdown
# 1-on-1 Notes — [Name]

[New entries go at the top]

---

## YYYY-MM-DD

**[Agenda section — adapted to their stated 1-on-1 philosophy]**

**Discussion:**
[Key points from the conversation]

**Signals:**
[Only if signals detected]

**Action items:**
- [ ] [Follow-ups]

**Notes for next time:**
[Things to remember]
```

**feedback.md:**
```markdown
# Feedback Log — [Name]

## Feedback Given

### YYYY-MM-DD — [Topic]
[What was shared, how they received it]

## Feedback Received (About Them)

### YYYY-MM-DD — From [Source]
[What was shared, context]
```

### Step 8: Initialize Git (Optional)

Ask: "Want me to initialize this as a git repo? Version control is useful for tracking changes over time, but it's not required."

If yes:
- `git init`
- Create a `.gitignore` (ignore OS files, editor files)
- Initial commit: "Initialize management brain with Paperwork"
- Ask if they want to push to GitHub/GitLab (create the repo if they confirm)

### Step 9: Onboarding Prompt

After generation, give them a clear starting path:

```
Your management brain is ready. Here's how to start using it:

1. **Right now:** Pick your 3 most important direct reports. Duplicate the
   example-person directory for each one and fill in their profile.md.
   Even partial info is fine — you'll build context over time.

2. **Before your next 1-on-1:** Run /prep [name] to see the system in action.
   It won't have much yet, but it'll start pulling from whatever you've added.

3. **After your next 1-on-1:** Run /log [name] to capture what happened.
   This is where the system starts compounding — each log makes the next
   prep better.

4. **End of your first week:** Run /health to see the big picture.

The system gets smarter the more you use it. The first week is setup.
After that, it's just part of how you manage.
```

---

## Principles

These guide every generation decision:

1. **Their system, not yours.** Every output reflects how *they* manage. Don't impose a philosophy.
2. **Start useful, grow over time.** Generate enough to be immediately usable. Don't over-engineer.
3. **Tools they have, not tools they should get.** If they don't use a meeting recorder, don't generate a /sync command. Meet them where they are.
4. **Raw over polished.** The notes and logs should be fast to capture, not pretty to read. Speed of capture > formatting.
5. **Humans over process.** The system exists to free up time for the hard, human parts of management. If a feature adds process without saving time, skip it.
6. **Private by default.** This is sensitive people data. Generate appropriate privacy guidelines and remind them.

---

## After Setup

Once the brain is built, the user works with it directly using their AI agent and the generated slash commands. Paperwork's job is done — it's a one-time bootstrap.

If they want to evolve the system later, they can run Paperwork again to add new commands, adjust their question banks, or restructure as their role changes.

---

*Built by [Jamie Wagner](https://www.linkedin.com/in/nobodyiscertain/). VP of Engineering managing 30 direct reports with AI. Figuring it out in real time and sharing what works.*

*Want help implementing your brain or adapting it as things change? [Book a coaching session.](https://everyexpert.com/nobodyiscertain)*
