# The Recursive Systems Method

A method for thinking, investigating, building, and orchestrating with AI.

The Recursive Systems Method begins with a desired end state and recursively
descends through the systems preventing that state from being true.

Each descent produces evidence.

Each discovery changes the map.

The end state remains visible throughout.

The process continues until the problem becomes sufficiently structured to
cross a **Tool Threshold**: the point at which a specialized tool, agent, model,
or human capability becomes the appropriate next intelligence to receive it.

The work is then handed off without losing state, evidence, constraints, or
intent.

## The Core Loop

```text
                      END STATE
                          ▲
                          │
                  continuously retained
                          │
BEGIN → OBSERVE → DESCEND → DISCOVER
  ▲                           │
  │                           ▼
  │                      REINTERPRET
  │                           │
  │                           ▼
  └──── SYNTHESIZE ←── DESCEND AGAIN
                          │
                          ▼
                   TOOL THRESHOLD
                          │
                          ▼
                       HANDOFF
                          │
                          ▼
                   NEW CAPABILITY
                          │
                          └────→ END STATE
```

This is not a circle.

It is a spiral.

The system may return to the same question repeatedly, but each return occurs
with greater resolution.

## First Principle

> Begin with what should be true. Descend until you discover why it is not
> true. Let each discovery revise the map without surrendering the end state.
> Continue until the problem crosses a tool threshold. Hand it to the right
> intelligence, preserve what it learns, and climb back toward the whole.

## Evidence Discipline

Every serious investigation separates:

- **Known** — directly demonstrated
- **Inferred** — strongly supported by evidence
- **Hypothesized** — plausible but untested
- **Unknown** — information still required
- **Disproved** — explanations contradicted by evidence

A hypothesis does not become a fact because it is useful, exciting, or likely.

## The Tool Threshold

A Tool Threshold occurs when a problem has become the right shape for another
tool.

```text
Vague problem
    ↓
exploration
    ↓
system boundaries identified
    ↓
specific artifacts / interfaces / questions
    ↓
---------------------
    TOOL THRESHOLD
---------------------
    ↓
specialized intelligence
```

Tool choice is therefore not merely a prerequisite to reasoning.

**Tool selection can itself be an output of reasoning.**

## Human and Machine Roles

The human retains:

- intent
- end-state judgment
- tradeoffs
- consequential decisions
- interpretation of what matters

AI and other tools provide:

- local expertise
- exploration
- implementation
- testing
- criticism
- documentation
- state preservation

The objective is not to remove the human from the system.

It is to increase the depth through which human intent can propagate.

## Case Study 001

The first live case study is the reverse engineering of an Anker A8392 USB-C
dock.

The initial objective was simple:

> Make three physical monitors behave as one logical display through one cable.

The investigation descended through:

```text
user requirement
→ macOS display behavior
→ MST
→ USB-C / DisplayPort Alt Mode
→ dock controller
→ firmware package
→ Synaptics VMM
→ ViewExpand
→ HID transport
→ DisplayPort AUX
→ GPU-specific Windows APIs
→ binary reverse engineering
```

The important artifact is not merely whether the dock is ultimately modified.

The case records how an initially vague physical goal became a precise
technical investigation and how the appropriate tools changed as the problem
changed shape.

## Status

This method is being developed through use.

The framework should evolve when real projects expose weaknesses in it.

When the system fails to preserve something important, the response should not
only be to remember better next time.

**The missing behavior should be encoded into the system.**

## Development Philosophy

> We do not invent this methodology in isolation and then try to use it. We build it by extracting rules from actual work.

The case studies in this repository are not examples we add later. They are the fossil record of the method being born.

Every time a project exposes a flaw—poor state retention, bad evidence discipline, premature tool selection, agent duplication, unclear authority—we modify the framework itself.

The repository evolves as:

```text
your way of thinking
        ↓
explicit principles
        ↓
files and schemas
        ↓
agent instructions
        ↓
software
        ↓
orchestration environment
```
