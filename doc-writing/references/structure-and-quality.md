# Structure, Quality, and Workflow

**Contents:** [Theoretical Foundations](#theoretical-foundations) |
[The Map](#the-map) | [Quality](#quality) | [Structure](#structure) |
[Workflow](#workflow)

## Theoretical Foundations

Diataxis serves _the practitioner in a domain of skill_. A domain of skill is
defined by a craft — using a tool, a programming language, flying an aircraft,
or an entire profession.

### Two Dimensions of Craft

**Action / Cognition**: A craft contains both action (practical knowledge,
knowing _how_, what we do) and cognition (theoretical knowledge, knowing _that_,
what we think). Completely bound up with each other, but wholly distinct — two
aspects of the same thing.

**Acquisition / Application**: A practitioner's relationship with their practice
requires both acquiring and applying. Being "at work" (applying) and "at study"
(acquiring) are counterparts — distinct but bound up with each other.

These two dimensions define the complete territory of craft. There are only two
dimensions, and they define the territory — this is why there are necessarily
four quarters, not three or five. It is not an arbitrary number.

### The Map of Needs

| Need          | Addressed in  | The user             | The documentation |
| ------------- | ------------- | -------------------- | ----------------- |
| Learning      | Tutorials     | Acquires their craft | Informs action    |
| Goals         | How-to guides | Applies their craft  | Informs action    |
| Information   | Reference     | Applies their craft  | Informs cognition |
| Understanding | Explanation   | Acquires their craft | Informs cognition |

## The Map

The map places documentation types into relationships. Each occupies a space,
and boundaries highlight distinctions.

### The Problem of Structure

When documentation fails to attain good structure, it's rarely just a problem of
structure — architectural faults infect and undermine content too. Without a
clear documentation architecture, creators often try to structure work around
product features. This is rarely successful even in a single instance; across a
portfolio of documentation the results are wild inconsistency.

Any orderly attempt to organise documentation into clear content categories will
help improve it. But authors often find that content doesn't fit well within
arbitrary categories. Diataxis resolves this: its categories emerge from
systematic analysis of user needs, not arbitrary groupings.

### Expectations and Guidance

A clear advantage of the map is that it provides both clear _expectations_ (to
the reader) and _guidance_ (to the author). It's clear what the purpose of any
particular piece of content is, it specifies how it should be written, and it
shows where it should be placed.

|                      | Tutorials                     | How-to guides                  | Reference               | Explanation                        |
| -------------------- | ----------------------------- | ------------------------------ | ----------------------- | ---------------------------------- |
| What they do         | Introduce, educate, lead      | Guide                          | State, describe, inform | Explain, clarify, discuss          |
| Answers the question | "Can you teach me to...?"     | "How do I...?"                 | "What is...?"           | "Why...?"                          |
| Oriented to          | Learning                      | Goals                          | Information             | Understanding                      |
| Purpose              | Provide a learning experience | Help achieve a particular goal | Describe the machinery  | Illuminate a topic                 |
| Form                 | A lesson                      | A series of steps              | Dry description         | Discursive explanation             |
| Analogy              | Teaching a child to cook      | A recipe in a cookery book     | Info on a food packet   | Article on culinary social history |

### The Journey Around the Map

Not a literal order, but a meaningful cycle of documentation needs:

1. **Learning-oriented**: Begin by diving in to do — under guidance
2. **Goal-oriented**: Put skill to work
3. **Information-oriented**: Work calls upon knowledge not yet in our head —
   consult reference
4. **Understanding-oriented**: Away from work, reflect on practice and knowledge

Then back to the beginning — new things to grasp, or deeper penetration.

## Quality

### Functional Quality

Documentation must meet standards of accuracy, completeness, consistency,
usefulness, precision. These are independent of each other — documentation can
be accurate without being complete, or complete but useless.

Attaining functional quality means meeting high, objectively-measurable
standards in multiple independent dimensions, consistently.

### Deep Quality

Beyond functional quality:

- _Feeling good to use_
- _Having flow_
- _Fitting to human needs_
- _Being beautiful_
- _Anticipating the user_

These cannot be measured but can be clearly identified. They are
**interdependent** (having flow and anticipating the user are aspects of each
other). They are **subjective** — assessed against the human, not the world.
They are **conditional** upon functional quality — documentation will never have
deep quality without being accurate and complete.

| Functional quality          | Deep quality                        |
| --------------------------- | ----------------------------------- |
| Independent characteristics | Interdependent characteristics      |
| Objective                   | Subjective                          |
| Measured against the world  | Assessed against the human          |
| A condition of deep quality | Conditional upon functional quality |
| Aspects of constraint       | Aspects of liberation               |

Consider how we judge quality of clothing. Clothes must have _functional
quality_ (keep us warm, stand up to wear — objectively measurable). But there
are other characteristics — quality of materials, workmanship, the way it hangs
and moves — that can't simply be measured. To recognise those, you need at least
a basic eye for them. Yet even someone who can't say _what_ makes clothing
excellent still knows _that_ it is: **it feels good to wear**. Your body knows
it.

It's the same in documentation. Users may not articulate _why_ documentation is
good, but they will feel it — or feel its absence. As creators, we need a clear
understanding of what makes documentation good, so we recognise _what_ is good,
not just _that_ it is.

**Diataxis addresses deep quality** — it cannot address functional quality
directly, but it exposes lapses in it (gaps become visible when reference
mirrors code structure; removing explanation from tutorials highlights where
learners are left to fend for themselves).

### Understanding the Limits

Diataxis can never be _all_ that is required in the pursuit of deep quality. It
can _help_ attain beauty in documentation, at least in its overall form, but it
doesn't by itself _make documentation beautiful_.

Diataxis offers a set of principles — it doesn't offer a formula. It cannot
offer a short-cut to success, bypassing the skills and insights of disciplines
such as user experience, interaction design, or visual design.

Using Diataxis does not guarantee deep quality. But it _can_ lay down conditions
for the _possibility_ of deep quality in documentation.

## Structure

### Basic Structure

```
Home                      <- landing page
    Tutorial              <- landing page
        Part 1
        Part 2
    How-to guides         <- landing page
        Install
        Deploy
        Scale
    Reference             <- landing page
        CLI
        API
    Explanation           <- landing page
        Best practices
        Security overview
```

Landing pages contain overviews of contents within. Each section's landing page
describes what it has to offer, providing context.

Even very large documentation sets can use this structure effectively, though
after a while some grouping of content within sections may be wise. Add another
layer of hierarchy when needed:

```
Home                      <- landing page
    Tutorial              <- landing page
        Part 1
        Part 2
    How-to guides         <- landing page
        Install           <- landing page
            Local installation
            Docker
            Virtual machine
            Linux container
        Deploy
        Scale
    Reference             <- landing page
        CLI
        API
    Explanation           <- landing page
        Best practices
        Security overview
```

### Contents Pages

Lists longer than ~7 items need breaking up. Landing page content should read
like an overview — introduce items with headings and snippets of text, don't
just present bare lists. **Author for a human user, not to fulfil a scheme.**

### Complex Hierarchies

When Diataxis meets another structure (topic areas, different user types,
different deployment targets), the result can be complex. Key principles:

- Diataxis is not four boxes — it identifies four _kinds_. There need not be
  simply four divisions in the hierarchy.
- **Diataxis is underpinned by attention to user needs** — let that direct you.
  Document the product _as it is for the user_.
- If the product is effectively three different products for three different
  users, let that be the starting point.
- Documentation should be as complex as it needs to be. Complex structures can
  be straightforward to navigate if they are logical and fit user needs.

## Workflow

### Use Diataxis as a Guide, Not a Plan

The structure is not a plan to complete. It's a guide — a map to check you're in
the right place going in the right direction. It provides tools to assess
documentation, identify problems, and judge what to do.

### Don't Worry About Structure

**Don't spend energy getting structure correct.** If you follow Diataxis
prompts, documentation will assume the structure — because it has been improved.
Structure is not imposed to improve; it emerges from improvement.

**Do not create empty structures** for tutorials/how-to/reference/explanation
with nothing in them. That's horrible.

Make changes where you see opportunities. At a certain point, changes will
demand moving material under Diataxis headings — that is how top-level structure
forms. **Diataxis changes structure from the inside.**

### Work One Step at a Time

Whatever the state of existing documentation — even a complete mess — it's
always possible to improve iteratively. Every step in the right direction is
worth publishing immediately. Don't try to work on the big picture.

If you're tidying up a huge mess, the temptation is to tear it all down and
start again. Avoid it. It isn't necessary to seek out things to improve.
Instead, apply Diataxis to whatever is right in front of you.

### The Iterative Cycle

1. **Choose something** — any piece, even at random. Don't go looking for
   problems. Just look at what you have right in front of you: the file you're
   in, the last page you read — it doesn't matter.
2. **Assess it** — preferably small (a paragraph, a sentence). Challenge it:
   _What user need is this? How well does it serve that need? What can be added,
   moved, removed, changed? Do its language and logic meet the requirements of
   this mode of documentation?_
3. **Decide** — what single next action will produce an immediate improvement?
4. **Do it** — complete that action and consider it done. Publish it.

Repeat. This keeps work flowing toward the desired end without needing a plan.

### Organic Growth

Good documentation develops like a living organism — well-formed growth at the
cellular level, not structure imposed from above. Like a plant: **never
finished** (always can develop further) but **always complete** (useful,
appropriate to its stage, structurally healthy, ready for the next stage).
