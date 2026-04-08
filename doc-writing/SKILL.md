---
name: doc-writing
description: >
  Write and structure documentation using the Diataxis framework. Diataxis
  identifies four kinds of documentation — tutorials, how-to guides, reference,
  and explanation — each serving a distinct user need and requiring a distinct
  writing approach. Use this skill when: (1) writing new documentation of any
  kind, (2) restructuring or improving existing documentation, (3) reviewing
  documentation for quality, (4) deciding what type of documentation to write,
  (5) the user asks to "write docs", "add documentation", "document this", or
  mentions tutorials, how-to guides, reference docs, or explanation pages.
---

# Diataxis Documentation Framework

Diataxis identifies four kinds of documentation that serve four different user
needs. Each has a distinct purpose and must be written in a distinct way.

There are exactly four kinds — not three or five — because they emerge from two
independent dimensions of craft (action/cognition and acquisition/application).
Two dimensions with two values each yield exactly four quarters. This is a
complete map of the territory: there is no other documentation need to cover.

## The Compass: Identify the Type First

Before writing, determine the documentation type using two questions:

| If the content...     | ...and serves the user's...      | ...then it belongs to... |
| --------------------- | -------------------------------- | ------------------------ |
| Informs **action**    | **Acquisition** of skill (study) | **Tutorial**             |
| Informs **action**    | **Application** of skill (work)  | **How-to guide**         |
| Informs **cognition** | **Application** of skill (work)  | **Reference**            |
| Informs **cognition** | **Acquisition** of skill (study) | **Explanation**          |

Apply these questions flexibly:

- _action_: practical steps, doing
- _cognition_: theoretical/propositional knowledge, thinking
- _acquisition_: study
- _application_: work

Apply at any scale — individual sentences or entire documents.

## The Four Types at a Glance

|                 | Tutorial                      | How-to guide           | Reference              | Explanation                  |
| --------------- | ----------------------------- | ---------------------- | ---------------------- | ---------------------------- |
| **Purpose**     | Provide a learning experience | Help achieve a goal    | Describe the machinery | Illuminate a topic           |
| **Answers**     | "Can you teach me to...?"     | "How do I...?"         | "What is...?"          | "Why...?"                    |
| **Oriented to** | Learning                      | Goals                  | Information            | Understanding                |
| **Form**        | A lesson                      | A series of steps      | Dry description        | Discursive discussion        |
| **Reader**      | Beginner under guidance       | Competent user at work | Competent user at work | Anyone seeking understanding |

## Universal Rule: No Editorialising

This applies to **all four documentation types**, no exceptions. No marketing in
documentation, ever. No selling, ever. Never pitch, hype, or tell the reader how
to feel. Statements like "This is the real power of X", "No YAML by hand!", "The
beautiful thing about this approach", or "You'll love how easy this is" are
marketing copy and must never appear in any documentation page — tutorials,
how-to guides, reference, or explanation. If the product is good, the
documentation proves it by being clear and useful, not by making claims.

## Writing Rules per Type

### Tutorial

Read [references/tutorials.md](references/tutorials.md) for full guidance.

- Use **"we"** — first-person plural throughout
- **Don't try to teach** — provide experiences that allow learning
- Show where they're going at the start; deliver results early and often
- Maintain a narrative of the expected ("You will notice that...")
- **Ruthlessly minimise explanation** — if a sentence explains _how_ or _why_
  something works rather than telling the reader what to _do_ or _notice_, cut
  it or link to an Explanation page. One-line noticing prompts ("Notice the
  `CLAUDE.md` file — this is what lets Claude Code work with swamp
  automatically.") are fine; multi-sentence explanations of internals are not.
- **Stay on the focused path** — end at the accomplishment. Don't add "Try
  something more interesting" or "You could also..." sections that open choices.
  If the reader wants to explore, they will. The tutorial's job is to deliver
  one complete, successful experience.
- Focus on the concrete; ignore options and alternatives
- **Show expected output at every step** — every command or agent interaction
  should show what the reader will see. Missing output is where confidence
  breaks down.
- Aspire to perfect reliability — must work every time
- **"What we will build" describes what we _do_, not what we _learn_** — say
  what we will produce, not "along the way we will see how X works." Describing
  what the reader will learn is presumptuous.

Language: _"In this tutorial, we will... First, do x. Now, do y. The output
should look something like... Notice that... You have built..."_

### How-to Guide

Read [references/how-to-guides.md](references/how-to-guides.md) for full
guidance.

- Write from the **user's perspective**, not the machinery's
- Address real-world goals and problems, not tool operations
- Assume competence — the user knows what they want
- **Action and only action** — no digression, explanation, or teaching
- Adaptable to real-world variation; omit the unnecessary
- Seek flow — anticipate the user's thinking and pace
- Title must say exactly what the guide shows

Language: _"This guide shows you how to... If you want x, do y. To achieve w, do
z. Refer to the x reference guide for a full list of options."_

### Reference

Read [references/reference.md](references/reference.md) for full guidance.

- **Describe and only describe** — neutral, austere, authoritative
- No doubt, no ambiguity, no opinion
- Structure mirrors the structure of the thing it describes
- Adopt standard, consistent patterns
- Provide examples to illustrate without explaining

Language: _"X inherits Y's defaults. It's available as `Z`. Sub-commands are: a,
b, c. You must use a. You must not apply b unless c. Never d."_

### Explanation

Read [references/explanation.md](references/explanation.md) for full guidance.

- **Make connections** — weave a web of understanding
- Provide context: _why_ things are so — design decisions, history, constraints
- Talk _about_ the subject (titles should work with an implicit "About...")
- Admit opinion, perspective, and alternatives
- Keep closely bounded — resist absorbing instruction or description

Language: _"The reason for x is because historically, y... W is better than z,
because... Some users prefer w. This can be a good approach, but..."_

## Guarding the Boundaries

The most common documentation failure is blurring types. Read
[references/distinctions.md](references/distinctions.md) when the type is
ambiguous or you suspect conflation.

**Most dangerous conflation**: Tutorial vs how-to guide. They look similar (both
have steps) but serve opposite needs — study vs work. A tutorial that tries to
be a how-to guide fails both.

**Subtle conflation**: Reference that drifts into explanation. Examples are fun
to develop and tempt you into saying _why_ — keep reference neutral and link to
explanation instead.

### Blur Risks by Adjacency

| Shared quality          | Types that blur         |
| ----------------------- | ----------------------- |
| Guide action            | Tutorial + How-to       |
| Serve work              | Reference + How-to      |
| Propositional knowledge | Reference + Explanation |
| Serve study             | Tutorial + Explanation  |

## Structuring Documentation

Read [references/structure-and-quality.md](references/structure-and-quality.md)
for the full map theory, quality framework, complex hierarchies, and workflow.
The map provides both clear _expectations_ to the reader and _guidance_ to the
author — it's clear what the purpose of any piece of content is, how it should
be written, and where it should be placed.

Key principles:

- **Don't create empty four-section structures.** Structure emerges from
  improvement, not the other way around.
- Landing pages should read like overviews with context, not bare lists.
- Keep lists under ~7 items; break up longer ones.
- For complex products (multiple user types, deployment targets), let user needs
  drive structure — Diataxis is an approach, not four boxes.
- **Work iteratively**: choose something, assess it against Diataxis, make one
  improvement, publish. Repeat.

## Workflow When Writing

1. **Identify the type** using the compass
2. **Read the relevant reference file** for that type's full guidance
3. **Consult [distinctions.md](references/distinctions.md)** if the type is
   ambiguous
4. **If the doc involves swamp commands**, set up a sandbox and run them (see
   below)
5. **Write in the correct voice and form** for that type, using real output from
   the sandbox
6. **Self-check**: Does any sentence belong to a different type? Move it or link
   to it.
7. **Title check**: Does the title clearly signal the type?
   - Tutorial: _"Getting started with X"_, _"Your first Y"_
   - How-to: _"How to configure X"_, _"Troubleshooting Y"_
   - Reference: _"X API"_, _"Configuration options"_
   - Explanation: _"About X"_, _"Why we use Y"_, _"Understanding Z"_

## Manual Page SEO Rules

Every manual page in `content/manual/` must follow these rules for search engine
optimization:

- **No `# heading` in markdown body** — the route template renders its own
  `<h1>` from the frontmatter `title` field. Including a `# Title` in the
  markdown produces duplicate `<h1>` elements on the page, which violates the
  single-`<h1>` SEO guideline. Start the markdown body directly with content or
  `##` subheadings.
- **Frontmatter `description`** — every page must have a `description` field
  (150-160 characters, unique per page). This becomes the `<meta description>`
  tag. Write it as a compelling summary with relevant keywords.
- **Frontmatter `title`** — keep under 60 characters. It renders as
  `{title} - Manual - Swamp Club` in the `<title>` tag.
- **Sitemap inclusion** — manual pages are automatically added to
  `routes/sitemap.xml.ts` via `loadManualPages()`. No manual sitemap entry
  needed.
- **BreadcrumbList JSON-LD** — the manual page route automatically emits
  `BreadcrumbList` structured data (Manual > Category > Page). No action needed
  per page.

## Swamp Sandbox: Verify Commands Before Writing

When writing or updating documentation that includes swamp commands, **run those
commands for real** and use the actual output in the docs. Never guess or
fabricate command output.

### Setup

1. **Check for swamp**: Run `which swamp`. If found, use it. If not, install it:

   ```bash
   curl -fsSL https://swamp.club/install.sh | sh
   ```

2. **Create a temporary repo**: Every doc-writing session that involves swamp
   commands should use a fresh temp directory:

   ```bash
   SWAMP_SANDBOX=$(mktemp -d)
   cd "$SWAMP_SANDBOX"
   swamp repo init
   ```

3. **Run the tutorial/guide steps** in this sandbox directory, capturing real
   output.

4. **Use the real output** in code blocks in the documentation. Copy it verbatim
   — don't clean it up, paraphrase it, or truncate it unless the output is very
   long (in which case truncate with `...` and note what was removed).

5. **Clean up** when done:

   ```bash
   rm -rf "$SWAMP_SANDBOX"
   ```

### When to use the sandbox

- **Always** when writing a new tutorial or how-to guide that includes swamp
  commands
- **Always** when updating docs after a swamp version change
- **Always** when a doc references specific command output, flags, file
  structures, or error messages
- **Not needed** for explanation pages that discuss concepts without showing
  commands

### What to capture

- The exact command run (including flags)
- The full output (or a representative excerpt with `...` for very long output)
- Any files or directories created (use `ls` or `cat` to show them)
- Error output if documenting error cases

If a command's output includes timestamps, UUIDs, or paths that will differ
between runs, the doc should say "You will see output like:" rather than "The
output will be:" — and it's fine to replace volatile values with placeholders
like `...` in the example.

### Tmux sandbox (for interactive tools like Claude Code)

When a tutorial involves Claude Code or other interactive tools, use a tmux
session to control the flow and capture output. This lets you launch Claude
Code, send it prompts, wait for responses, and capture exactly what appears on
screen.

**Setup:**

```bash
# Create sandbox directory
SWAMP_SANDBOX=$(mktemp -d)

# Start a tmux session
tmux new-session -d -s docs-sandbox -x 120 -y 40
tmux send-keys -t docs-sandbox "cd $SWAMP_SANDBOX" Enter
```

**Sending commands and capturing output:**

```bash
# Send a command
tmux send-keys -t docs-sandbox 'swamp repo init' Enter

# Wait for command to finish (poll for expected output)
# Then capture the pane content
tmux capture-pane -t docs-sandbox -p
```

**Waiting for output:** Poll `tmux capture-pane -t docs-sandbox -p` in a loop
checking for expected text (a prompt character, a known output line, etc.)
rather than using fixed sleeps. For example, wait for the `$` prompt to reappear
after sending a command:

```bash
# Wait up to 15 seconds for the shell prompt to return
for i in $(seq 1 30); do
  if tmux capture-pane -t docs-sandbox -p | grep -q '^\$'; then
    break
  fi
  sleep 0.5
done
tmux capture-pane -t docs-sandbox -p
```

**Launching Claude Code in the session:**

```bash
# Start Claude Code
tmux send-keys -t docs-sandbox 'claude' Enter

# Wait for Claude Code to be ready (look for the input prompt)
# Then send a prompt
tmux send-keys -t docs-sandbox 'Create a command/shell model called hello-world that echoes "Hello from the swamp!"' Enter

# Wait for Claude Code to finish (poll for its idle indicator)
# Capture the output
tmux capture-pane -t docs-sandbox -p

# Exit Claude Code
tmux send-keys -t docs-sandbox '/exit' Enter
```

**Cleanup:**

```bash
tmux kill-session -t docs-sandbox
rm -rf "$SWAMP_SANDBOX"
```

**When to use tmux vs direct Bash:**

- Use **direct Bash** (the basic sandbox above) for simple CLI commands like
  `swamp model method run`, `swamp data query`, etc. It's simpler and faster.
- Use **tmux** when the tutorial involves Claude Code, interactive prompts, or
  multi-step flows where you need to see the terminal as the user would.
- You can **mix both** — use tmux for the Claude Code steps and direct Bash for
  the CLI steps in the same tutorial.
