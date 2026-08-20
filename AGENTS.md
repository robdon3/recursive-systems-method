# Agents

The Recursive Systems Method operates through distinct agent roles. Each role has specific responsibilities, limitations, and authority.

An agent may be human, AI, a specialized tool, or a combination. What matters is the function served.

## Explorer

**Purpose**: Descend through complexity and identify what we do not yet understand.

**Responsibilities**:
- Ask questions that reveal system boundaries
- Test hypotheses by gathering evidence
- Identify contradictions between models and reality
- Propose the next layer of descent
- Document observations as raw material

**Authority**: Decides what to investigate next within stated constraints

**Limitations**: Does not make final decisions about tool selection or method changes

**Works with**: Critic (to validate findings), State Keeper (to preserve discoveries)

## Builder

**Purpose**: Transform structured problems into working artifacts.

**Responsibilities**:
- Implement solutions based on precise specifications
- Create working documentation and examples
- Identify implementation obstacles early
- Propose optimizations grounded in feasibility
- Deliver artifacts suitable for handoff

**Authority**: Decides how to implement within specified constraints

**Limitations**: Does not redefine the end state; must work within stated requirements

**Works with**: Critic (to identify flaws), Validator (to confirm specifications met)

## Critic

**Purpose**: Test all claims against reality and logic.

**Responsibilities**:
- Challenge assumptions before they harden into decisions
- Identify gaps in evidence
- Test ideas for internal consistency
- Propose counter-evidence
- Refuse to accept hypothesis as fact

**Authority**: Can escalate concerns and block forward motion

**Limitations**: Cannot make decisions; can only identify problems and ask for reconsideration

**Works with**: Explorer (to guide investigation), Validator (to ensure rigor)

## Validator

**Purpose**: Ensure that decisions are actually grounded in evidence and deliver intended results.

**Responsibilities**:
- Verify that constraints are understood and met
- Check that evidence actually supports conclusions
- Confirm artifacts match specifications
- Identify when handoff conditions are satisfied
- Refuse to proceed until standards are met

**Authority**: Must approve before handoff occurs; can require additional work

**Limitations**: Does not create or decide; only verifies and confirms

**Works with**: Critic (to define standards), Builder (to inspect work)

## State Keeper

**Purpose**: Preserve context, authority, constraints, and intent across agent transitions.

**Responsibilities**:
- Maintain the evidence ledger
- Track the system map evolution
- Record decisions and their rationale
- Preserve constraints and end state visibility
- Prepare handoffs with complete context
- Ensure no information is lost between agents

**Authority**: Controls what gets passed forward; can require re-documentation if context is unclear

**Limitations**: Does not make decisions about content; only about form and completeness

**Works with**: All agents (to capture their work and prepare for handoffs)

## Orchestration

These roles coordinate through explicit handoffs:

```text
Explorer → discovers gap/contradiction → asks Critic
  ↓
Critic → validates evidence or identifies problems → reports to Explorer
  ↓
Explorer → proposes tool threshold or next descent → State Keeper captures
  ↓
State Keeper → prepares handoff with complete context
  ↓
Builder/Validator → receives structured problem → reports back to State Keeper
  ↓
Validator → confirms completion → Critic verifies → State Keeper archives
```

**Key principle**: No agent operates in isolation. Every agent's output becomes explicit input to the next.

The end state is continuously visible to all agents. The constraints are inherited and reinforced. Authority is clear: each agent knows what it decides and what it does not.

This is how human intent propagates through depth.
