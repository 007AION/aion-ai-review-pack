# AI Fast Collaboration Channel Protocol v0.1

## Purpose
Define how 007 and external audit-side AI (such as 都水监) use a shared Discord channel for rapid coordination without turning chat into the formal governance store.

## Why this exists
The fast loop exists to reduce human relay burden while preserving:
- formal GitHub closure
- auditability
- low token waste
- protection of sensitive project information

## Channel role
This channel is a **fast coordination layer**, not the formal source of truth.

Use it for:
- short questions
- short challenge / response loops
- routing discussion
- deciding which issue should receive the next formal write-back
- identifying ambiguity before formal issue updates

Do not use it as:
- the only closure location
- the only record for high-risk decisions
- a dump for long execution logs
- a place to share sensitive business or credential information

## What this protocol defines
1. channel purpose
2. allowed and forbidden information classes
3. what must return to GitHub
4. how 007 and external AI should talk
5. how to reduce token waste
6. how to protect sensitive operational context

---

## Information boundary model

### Allowed to discuss openly with external audit AI
- organization structure
- role model
- boundaries and permission concepts
- workflow rules
- issue templates
- audit methods
- closure methods
- blocker taxonomy
- risk classification logic
- governance methods
- standards, checklists, and review criteria

### Restricted / do not share in fast collaboration channel
- tokens, keys, secrets, credentials
- actual permission grants or privileged account details
- customer identity or customer data
- business model internals beyond abstract governance relevance
- pricing, revenue, sales conversion, or internal commercial metrics
- private deployment details unless abstracted
- sensitive environment topology
- exact operational weaknesses that would materially increase attack surface

### Safe sharing rule
If a point can be abstracted without losing governance value, abstract it.

---

## Interaction rules

### Rule 1: Short-message discipline
Messages should be short, pointed, and linked to a concrete issue or standard where possible.

### Rule 2: One discussion, one anchor
When possible, tie a discussion to:
- issue number
- file path
- standard name

### Rule 3: Discord for compression, GitHub for fixation
If a useful conclusion emerges, it must be written back to GitHub when it affects:
- rules
- issue direction
- audit judgment
- closure conditions
- follow-up task creation

### Rule 4: No hidden side-channel governance
Chat may clarify. Chat may challenge. Chat may accelerate. But chat must not silently become the only place where governance changes occur.

### Rule 5: Sensitive-context minimization
Do not paste more sensitive operational context than is needed to ask the question.

---

## Token economy rules for the fast loop
1. prefer short prompts over long replays
2. reference file names and issue numbers instead of pasting large documents
3. ask one sharp question at a time where possible
4. use GitHub links as the deep context layer
5. summarize before expanding

---

## Recommended operating pattern
1. identify issue or ambiguity
2. ask short question in Discord channel
3. receive challenge / audit feedback
4. decide next GitHub target
5. write back to GitHub
6. if needed, summarize result back in Discord in one or two lines

---

## Red-line rule
External audit AI may help judge roles, rules, methods, workflow, and structure.
External audit AI must not be given unrestricted access to secrets, commercial internals, or privileged operational controls merely for convenience.

---

## Practical benefit
This protocol exists to create:
- less human copy-paste
- faster AI-to-AI challenge loops
- better governance without chat sprawl
- safer external collaboration
