# Writing Tutorials

**Contents:** [The Tutorial as a Lesson](#the-tutorial-as-a-lesson) |
[Key Principles](#key-principles) | [Language Patterns](#language-patterns) |
[Food Analogy](#the-food-analogy-teaching-a-child-to-cook)

A tutorial is a **lesson** — a learning experience under the guidance of a
tutor. It is always **learning-oriented**.

The student learns by doing something meaningful toward an achievable goal. What
the student _does_ is not necessarily what they _learn_. Through doing, they
acquire facts, understanding, familiarity with tools, workflows, concepts,
commands, and how things relate to each other.

## The Tutorial as a Lesson

A lesson entails a relationship between teacher and pupil. Learning takes place
as the pupil applies themself to tasks under the instructor's guidance.

A good lesson gives the learner confidence by showing them they can be
successful.

### Obligations of the Teacher

Nearly all responsibility falls on the teacher: what the pupil will learn, what
they will do, and their success. The pupil's only responsibility is to be
attentive and follow directions.

The exercise must be:

- **Meaningful** — the pupil has a sense of achievement
- **Successful** — the pupil can complete it
- **Logical** — the path makes sense
- **Usefully complete** — the pupil encounters all actions, concepts, and tools
  they need

### The Special Difficulty

In documentation, the instructor is condemned to be absent. The instructor must
find a way to be present through written instruction alone. A teacher who's
there can rescue a learner when things go wrong; in a tutorial, you can't do
that. The tutorial must be so well constructed that things _can't_ go wrong.

### The Problem of Tutorials

Tutorials are rarely done well, partly because they are genuinely difficult to
do well, and partly because they are not well understood. Many products lack
good tutorials or lack tutorials completely; tutorials are often conflated with
how-to guides.

Writing and maintaining tutorials consumes a remarkable amount of effort. Unlike
other documentation where changes can generally be made discretely, in tutorials
— where the end-to-end learning journey must make sense — changes often cascade
through the entire story. The product itself evolves rapidly, meaning all that
work needs to be done again to ensure the tutorial still performs its required
functions.

Tutorials also carry the additional complication of the distinction between
_what is to be learned_ and _what is to be done_. The creator must have a good
sense of what the user must learn, and when, and must also devise a meaningful
learning journey that delivers all of that.

## Key Principles

A tutorial is a pedagogical problem. The first rule of teaching: **don't try to
teach.** Provide the learner with an experience that allows them to learn. If
you give in to the anxiety to impart knowledge by telling and explaining, you
jeopardise the learning experience.

Anti-pedagogical temptations to resist:

- Abstraction, generalisation
- Explanation
- Choices
- Information

### Show the Learner Where They'll Be Going

Allow the learner to form an idea of what they will achieve from the start.

Good: _In this tutorial we will create and deploy a scalable web application.
Along the way we will encounter containerisation tools and services._

Bad: _In this tutorial you will learn..._ — this is presumptuous.

### Deliver Visible Results Early and Often

Understanding comes from connecting causes and effects. Let the learner see
results rapidly and repeatedly. Every step should produce a comprehensible
result, however small.

### Maintain a Narrative of the Expected

At every step, the user experiences anxiety: will this produce the correct
result? Keep providing feedback that they are on the right path.

- "You will notice that ..."
- "After a few moments, the server responds with ..."
- Show actual example output or exact expected output
- Flag likely signs of going wrong: "If the output doesn't show ..., you have
  probably forgotten to ..."
- Prepare for surprises: "The command will probably return several hundred lines
  of logs in your terminal."

### Point Out What the Learner Should Notice

A learner is typically too focused on what they are doing to notice signs in
their environment unless prompted. Close the loops of learning by pointing
things out in passing. This can be as simple as noting how a command line prompt
changes.

### Target the Feeling of Doing

The accomplished practitioner experiences a _feeling of doing_ — joined-up
purpose, action, thinking, and result. As skill develops, it flows in a
confident rhythm and becomes a kind of pleasure.

Ensure the tutorial's tasks tie together purpose and action to become a cradle
for this feeling.

### Encourage and Permit Repetition

Learners return to and repeat exercises that give them success. Repetition
establishes the feeling of doing. Try to make steps repeatable. Watching users,
you may be amazed how often they choose to repeat a step just to see the same
thing happen again.

### Ruthlessly Minimise Explanation

A tutorial is not the place for explanation. The user is focused on following
directions and getting results. Explanation distracts attention and blocks
learning.

Sufficient: _We're using HTTPS because it's more secure._ Then link to an
in-depth article for when the user is ready.

Explanation is only pertinent at the moment the _user_ wants it — not when the
author decides.

### Focus on the Concrete

The student is in the moment, composed of concrete things. Focus on _this_
problem, _this_ action, _this_ result. Lead from step to concrete step.

Our minds perceive general patterns from concrete examples spectacularly well.
All learning moves from the concrete and particular toward the general and
abstract. The latter _will_ emerge from the former.

### Ignore Options and Alternatives

Guide the learner to a successful conclusion. Ignore diversions — different
options, different ways to use the API, different approaches. Guidance must
remain focused on reaching the conclusion. Everything else can wait.

### Aspire to Perfect Reliability

A tutorial must inspire confidence. Confidence is built layer by layer and
easily shaken. When the user follows directions and doesn't get expected
results, they lose confidence in the tutorial, the tutor, and themselves.

The tutorial ought to work for every user, every time. Rely on users to discover
flaws through extensive testing and observation.

## Language Patterns

| Pattern                                                              | Purpose                                                      |
| -------------------------------------------------------------------- | ------------------------------------------------------------ |
| _We ..._                                                             | First-person plural affirms the teacher-learner relationship |
| _In this tutorial, we will ..._                                      | Describe what the learner will accomplish                    |
| _First, do x. Now, do y. Now that you have done y, do z._            | No room for ambiguity or doubt                               |
| _We must always do x before y because... (see Explanation for more)_ | Minimal explanation in basic language, link to more          |
| _The output should look something like ..._                          | Clear expectations                                           |
| _Notice that ... Remember that ... Let's check ..._                  | Clues to confirm they're on track                            |
| _You have built a secure, three-layer hylomorphic stasis engine..._  | Describe and mildly admire what they accomplished            |

## The Food Analogy: Teaching a Child to Cook

It doesn't matter what the child makes or how correctly they do it. The value
lies in what the child _gains_, not what they produce. Success is when the child
acquires the knowledge and skills you hoped to impart.

The lesson might be framed around preparing a dish, but what we need the child
to learn is: _that we wash hands before handling food; how to hold a knife; why
the oil must be hot; what this utensil is called; how to time and measure
things._ The child learns by working alongside you — through activities, not
from things you say or show.

If the lesson ends early but the child achieved something and enjoyed it, it
laid down something that can be returned to and built upon.
