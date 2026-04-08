# Writing How-to Guides

**Contents:** [Addressed to Problems](#how-to-guides-addressed-to-problems) |
[What They Are Not](#what-how-to-guides-are-not) |
[Key Principles](#key-principles) | [Language Patterns](#language-patterns) |
[Food Analogy](#the-food-analogy-a-recipe)

How-to guides are **directions** that guide the reader through a problem or
towards a result. How-to guides are **goal-oriented**.

A how-to guide helps the user get something done, correctly and safely. It
guides the user's _action_ and is concerned with _work_ — navigating from one
side to the other of a real-world problem-field.

Examples: _How to calibrate the radar array; How to use fixtures in pytest; How
to configure reconnection back-off policies._ Not: _How to build a web
application_ — that's not a specific goal, it's a vastly open-ended sphere.

The list of how-to guides frames what your product can actually _do_. A rich
list is an encouraging suggestion of capabilities. Well-written how-to guides
are likely the most-read sections of documentation.

## How-to Guides Addressed to Problems

**Write from the perspective of the user, not of the machinery.** Every how-to
guide should answer to a human project — show what the human needs to do, with
tools at hand, to obtain the result they need.

This contrasts with a common anti-pattern: guides defined by operations that can
be performed with a tool or system. This offers little value — it's focused on
the tool, on taking the machinery through its motions.

This is a distinction of _meaningfulness_. Meaning comes from purpose and need.
There is no purpose or need in the functionality of a machine — merely causes
and effects, inputs and outputs.

Consider:

- "To shut off the flow of water, turn the tap clockwise."
- "To deploy the desired database configuration, select the appropriate options
  and press **Deploy**."

These _look_ like guidance but are not. They represent mostly useless
information that anyone with basic competence should know. What the user needs:

- How much water to run, and how vigorously, for a certain purpose
- What database configuration options align with particular real-world needs

**How-to guides are about goals, projects, and problems, not about tools.**
Tools appear as incidental bit-players, means to the user's end. Sometimes a
guide concentrates on a particular tool when a goal aligns closely with it. Just
as often, a guide cuts across different tools or parts of a system, joined by
something a human needs to get done.

## What How-to Guides Are Not

**Wholly distinct from tutorials.** They are often confused, but the user needs
they serve are quite different. This conflation is at the root of many
documentation difficulties. See [distinctions.md](distinctions.md) for the full
contrast.

Not merely procedural guides. Real-world problems don't always offer linear
solutions. Sequences sometimes fork and overlap, with multiple entry and exit
points. A how-to guide often needs the user to rely on their judgement.

## Key Principles

A how-to guide is concerned with work — a task or problem, with a practical
goal. _Maintain focus on that goal._

How-to characteristics:

- Focused on tasks or problems
- Assume the user knows what they want to achieve
- Action and only action
- No digression, explanation, teaching

Anything else dilutes useful power. Temptations are to explain or provide
reference for completeness — neither is part of guiding work. If important, link
to them.

### Address Real-World Complexity

**A how-to guide needs to be adaptable to real-world use-cases.** One useless
for any purpose except exactly the narrow case you addressed is rarely valuable.
You can't address every possible case, so remain open to the range of
possibilities in a way that lets the user adapt your guidance.

### Omit the Unnecessary

**Practical usability is more helpful than completeness.** A how-to guide does
not need to be complete end-to-end (unlike a tutorial). It should start and end
in some reasonable, meaningful place, and require the reader to join it to their
own work.

### Provide a Set of Instructions

A how-to guide describes an _executable solution_ to a real-world problem. It's
a contract: if you're facing this situation, work through it by taking these
steps. Steps are in the form of _actions_.

"Actions" includes physical acts but also thinking and judgement — solving a
problem involves thinking it through. Address how the user thinks as well as
what the user does.

### Describe a Logical Sequence

The fundamental structure is a _sequence_ implying logical ordering in time.
Sometimes ordering is imposed by dependencies. Sometimes it's more subtle — one
operation might set up the user's environment or thinking to benefit the next.

### Seek Flow

Ground sequences in the patterns of the _user's_ activities and thinking for
smooth progress.

Consider: What are you asking the user to think about? How will thinking flow
from subject to subject? How long must the user hold thoughts open before
resolving them in action? If you require jumping back to earlier concerns, is
that avoidable?

A how-to guide has pace and rhythm. Badly-judged pace or disrupted rhythm damage
flow.

At its best, how-to documentation _anticipates_ the user — the documentation
equivalent of a helper who has the tool you were about to reach for, ready to
place it in your hand.

### Pay Attention to Naming

**Choose titles that say exactly what a how-to guide shows.**

- Good: _How to integrate application performance monitoring_
- Bad: _Integrating application performance monitoring_ (maybe it's about
  whether you should, not how)
- Very bad: _Application performance monitoring_ (could be how, whether, or just
  what it is)

Search engines appreciate good titles just as much as humans.

## Language Patterns

| Pattern                                                      | Purpose                                  |
| ------------------------------------------------------------ | ---------------------------------------- |
| _This guide shows you how to..._                             | Describe the problem or task clearly     |
| _If you want x, do y. To achieve w, do z._                   | Conditional imperatives                  |
| _Refer to the x reference guide for a full list of options._ | Don't pollute with every possible option |

## The Food Analogy: A Recipe

A recipe clearly defines what will be achieved and addresses a specific question
(_How do I make...?_ or _What can I make with...?_).

It's not the recipe's responsibility to _teach_ you. A professional chef who
created the recipe may still follow it to ensure correctness.

Following a recipe **requires at least basic competence**. Someone who has never
cooked should not be expected to follow one with success — a recipe is not a
substitute for a cooking lesson.

Someone expecting a recipe who gets a cooking lesson instead will be
disappointed and annoyed. While it's interesting to read about a dish's context
or history, you don't want that while trying to make it. A good recipe follows a
well-established format that excludes both teaching and discussion and focuses
only on **how** to make the dish.
