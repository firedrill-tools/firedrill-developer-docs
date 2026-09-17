# Firedrill documentation rules

This is a Mintlify documentation site. Pages are MDX with YAML frontmatter; site configuration lives in `docs.json`.

## Product truth

- Firedrill is a stateful simulation and testing framework for action-taking AI agents.
- Lead with the tool-first path: add or create Tools, start the synthetic environment, connect the existing agent, then add drills when behavior should become repeatable.
- Firedrill runs controlled worlds, not customer agents. Users keep their existing model, application, and runner.
- The complete individual-developer loop is local. Hosted features add managed operation, history, replay, sharing, teams, retention, and attestation.
- Never document a planned feature as available. Label release candidates, previews, and unpublished packages clearly.
- Never present an example Tool, vendor, agent type, or fixture as the product model.
- Demo delivery is v2 and must not appear as a current capability.
- Use `https://docs.firedrill.run` for published documentation links. Keep
  `https://firedrill.run` for the product site and the existing `api.`, `app.`,
  and other service subdomains for their respective products.
- Do not mention competitors, private planning, research provenance, or internal implementation discussions.

## Terminology

- **Tool**: a synthetic dependency with operations, state, schemas, and behavior.
- **World**: an isolated stateful environment in which Tools and actors interact.
- **Scenario**: reusable starting conditions such as data, faults, events, permissions, and time.
- **Drill**: an executable behavioral test for an agent.
- **Run**: one recorded execution of a drill.
- **Evidence**: the ordered record of calls, mutations, events, faults, time, assertions, and optional captures.

Capitalize **Tool** when referring to the Firedrill concept. Use “run a drill,” not “run a simulation,” in user-facing copy.

## Writing and design

- Use active voice, second person, short paragraphs, and sentence-case headings.
- Define Firedrill-specific terms before relying on them.
- Put the quickest useful path first and move advanced detail to reference pages.
- Use code that a developer can copy. Do not replace required values with unexplained placeholders.
- Use cards only for major choices, steps only for ordered workflows, and callouts only when they carry meaning.
- Keep light and dark mode readable, keyboard navigation intact, and link text descriptive.

## Verification

Run `mint validate`, the full broken-link check, `mint a11y`, and a local desktop/mobile preview before pushing.
