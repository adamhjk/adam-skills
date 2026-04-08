# Writing Reference

Reference guides are **technical descriptions** of the machinery and how to
operate it. Reference material is **information-oriented**.

Reference contains _propositional or theoretical knowledge_ that a user looks to
in their _work_. Its only purpose is to describe, as succinctly as possible, in
an orderly way.

Content of tutorials and how-to guides is led by user needs. Reference material
is led by the product it describes.

For software: reference describes APIs, classes, functions, and how to use them.

Users need reference because they need truth and certainty — firm platforms on
which to stand while they work. Good technical reference is essential for user
confidence.

## Reference as Description

Reference describes the machinery. It should be **austere**. One hardly _reads_
reference material; one _consults_ it.

There should be no doubt or ambiguity. It should be wholly authoritative.

Reference is like a map: it tells you what you need to know about the territory
without having to go check the territory yourself.

Although reference should not attempt to show how to perform tasks, it can and
often needs to include a description of how something works or the correct way
to use it.

Some reference (such as API documentation) can be generated automatically by the
software, which is a powerful way of ensuring faithful accuracy. But
auto-generated reference alone is not sufficient documentation.

## Key Principles

### Describe and Only Describe

_Neutral description_ is the key imperative. It's one of the hardest things to
do — describing neutrally is not a natural way of communicating. What's natural
is to explain, instruct, discuss, opine. All of these run counter to reference's
demands of accuracy, precision, completeness, and clarity.

It can be tempting to introduce instruction and explanation because description
seems too inadequate. Instead, link to how-to guides, explanation, and
tutorials.

Style and form:

- Austere and uncompromising
- Neutrality, objectivity, factuality
- Structured according to the structure of the machinery itself

### Adopt Standard Patterns

**Reference is useful when it is consistent.** Standard patterns allow effective
use. Place the material where users expect to find it, in a format they're
familiar with.

There are many opportunities to delight readers with extensive vocabulary and
multiple styles. Reference is definitely not one of them.

### Respect the Structure of the Machinery

**The structure of the documentation should mirror the structure of the
product**, so the user can work through them at the same time — just as a map
corresponds to territory.

This doesn't mean forcing documentation into unnatural structure. The logical,
conceptual arrangement of and relations within the code should help make sense
of the documentation.

### Provide Examples

**Examples** illustrate reference while avoiding distraction. An example of
usage of a command can succinctly illustrate it and its context without falling
into the trap of trying to explain or instruct.

## Language Patterns

| Pattern                                                                                                                    | Purpose                                                                          |
| -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| _Django's default logging configuration inherits Python's defaults. It's available as `django.utils.log.DEFAULT_LOGGING`._ | State facts about machinery and behaviour                                        |
| _Sub-commands are: a, b, c, d, e, f._                                                                                      | List commands, options, operations, features, flags, limitations, error messages |
| _You must use a. You must not apply b unless c. Never d._                                                                  | Provide warnings where appropriate                                               |

## The Food Analogy: Information on a Packet

When looking for information — relevant facts — you do not want opinions,
speculation, instructions, or interpretation. You expect information presented
in standard ways so you can find nutritional properties, storage instructions,
or ingredients quickly and reliably.

_May contain traces of wheat. Net weight: 1000g._

You would not expect recipes or marketing claims mixed with this information —
that could be literally dangerous. The way reference material is presented on
food products is so important it's usually governed by law. The same seriousness
should apply to all reference documentation.
