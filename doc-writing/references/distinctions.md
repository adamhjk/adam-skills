# The Critical Distinctions

**Contents:** [Tutorial vs How-to Guide](#tutorial-vs-how-to-guide) |
[Reference vs Explanation](#reference-vs-explanation) |
[Blur Risks](#the-maps-natural-affinities-blur-risks)

The most common documentation failures come from blurring the boundaries between
types. Two conflations are especially dangerous.

## Tutorial vs How-to Guide

The single most common conflation in software documentation.

### Why They Get Confused

Tutorials and how-to guides share important surface similarities. Both are
practical guides: they contain directions, set out steps, and promise that
following those steps leads to a successful conclusion. Neither makes much sense
except for the user who has their hands on the machinery, ready to do things.
Both describe ordered sequences of actions where order matters.

They are closely related — and like many close relations, easily mistaken for
one another. But they serve fundamentally different needs.

### The Core Distinction

| Tutorial                                      | How-to Guide                           |
| --------------------------------------------- | -------------------------------------- |
| Serves the user who is **at study**           | Serves the user who is **at work**     |
| Obligation: provide a **learning experience** | Obligation: help accomplish **a task** |
| **Learning-oriented**                         | **Task-oriented**                      |

### Point-by-Point Contrasts

| Tutorial                                                                                   | How-to Guide                                                                                               |
| ------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------- |
| Helps the pupil **acquire basic competence**                                               | Helps the competent user **perform a task correctly**                                                      |
| Provides a **learning experience** — what matters is what the learner does and experiences | **Directs the user's work**                                                                                |
| Follows a **carefully-managed path** with required encounters along the way                | Aims for a successful result via the safest route, but **the path can't be managed** — it's the real world |
| **Familiarises** the learner with tools, language, processes                               | Can and should **assume familiarity**                                                                      |
| Takes place in a **contrived setting** — a learning environment                            | Applies to the **real world**                                                                              |
| **Eliminates the unexpected**                                                              | Must **prepare for the unexpected**                                                                        |
| Follows a single line, **no choices or alternatives**                                      | Will typically **fork and branch**: _If this, then that_                                                   |
| **Must be safe** — always possible to start again                                          | **Cannot promise safety** — often one chance to get it right                                               |
| **Responsibility lies with the teacher**                                                   | **The user has responsibility**                                                                            |
| Learner **may not have competence to ask the right questions**                             | User is **asking the right questions**                                                                     |
| **Explicit about basic things** — where to do things, how to hold implements               | Relies on this as **implicit knowledge**                                                                   |
| **Concrete and particular** — specific, known, defined tools and conditions                | Takes a **general approach** — many things unknowable in advance                                           |
| **Teaches general skills and principles** applicable to many cases                         | User follows it to **complete a particular task**                                                          |

### "Basic" vs "Advanced" Is a Trap

A common mistake is seeing tutorials as "basic" and how-to guides as "advanced."

- How-to guides can and often should cover **basic procedures** (correct
  paperwork, disposal of materials, routine operations)
- Tutorials can present **advanced, complex** material (an experienced
  anaesthetist taking a course on difficult neonatal intubations is still in a
  _tutorial_ — a learning experience under instructors)

The difference is the need served: **the user's study** or **their work**.

### Why It Matters

A clinical manual that conflated education with practice — that tried to teach
while guiding a real-world procedure — would be a literally deadly document.

In software we get away with more, but every time we publish a tutorial or
how-to guide that doesn't understand whether it serves study or work, we cause
low-level inconvenience and unhappiness. Users who aren't brought to success
will find something else.

This conflation is particularly harmful because it risks failing newcomers we
hope to turn into committed users.

## Reference vs Explanation

Both belong to the _theory_ half of the map — neither contains steps to guide
the reader. The difference is the same axis: **acquisition** vs **application**
of skill, or **study** vs **work**.

### Quick Tests

- **If it's boring and unmemorable** — probably _reference_
- **Lists of things** (classes, methods, attributes) and **tables of
  information** — _reference_
- **If you can imagine reading it in the bath** — probably _explanation_
- **"Can you tell me more about <topic>?"** — the answer is _explanation_

### The Real Test

Is this something someone would turn to **while working** — actually executing a
task? That's **reference**.

Is this something they'd need once they've **stepped away from work** and want
to think about it? That's **explanation**.

### The Common Slip

It usually happens while writing reference that starts to become expansive.
Examples are fun to develop and can tempt you into explanation (saying _why_, or
_what if_, or how it came to be).

The result: explanatory material sprinkled into reference. Bad for the reference
(interrupted by digressions). Bad for the explanation (not allowed to develop
and do its own work).

## The Map's Natural Affinities (Blur Risks)

Each type has natural affinity with its neighbours, creating blur risk:

| Shared quality                  | Adjacent types            |
| ------------------------------- | ------------------------- |
| Guide action                    | Tutorials + How-to guides |
| Serve application of skill      | Reference + How-to guides |
| Contain propositional knowledge | Reference + Explanation   |
| Serve acquisition of skill      | Tutorials + Explanation   |

When distinctions blur, writing style and content make their way into
inappropriate places, causing structural problems that make it even harder to
maintain discipline. In the worst case: complete collapse of tutorials and
how-to guides into each other, making it impossible to meet either need.
