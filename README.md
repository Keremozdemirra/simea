# SIMEA — Systemic Influence Model of Economic Agency

Classical economics modelled the agent as a rational utility-maximiser.
Behavioural economics kept the maximiser and added the ways it fails. SIMEA
proposes a different starting point: the agent is a **decision-subject**,
embedded in and steered by systems — algorithms, platforms, recommender
architectures, social infrastructure — rather than an optimiser operating on
its own preferences.

The framework introduces three constructs:

| Construct | Symbol | What it measures |
| --- | --- | --- |
| Influence Gradient | *IG* | The pull external systems exert on an agent's choice |
| Autonomy Threshold | *AT* | How much of the decision remains the agent's own |
| Systemic Entropy | *SE* | The disorder of the choice environment the agent sits in |

and a welfare function that weights utility by autonomy and by the diversity of
choices actually available, rather than by realised consumption alone.

This repository is the working home of that programme: the papers, the models
that test them, and the open problems.

## Contents

| | | Status |
| --- | --- | --- |
| [01 — SIMEA framework](papers/01-simea-framework) | The original statement of the model, its constructs and its welfare function | Draft |
| [02 — Determinism and predictability](papers/02-determinism-and-predictability) | If determinism holds, does it follow that financial futures are predictable? Argues that it does not, and that predictability is instead a function of autonomy | Positioning note; [bibliography verified](papers/02-determinism-and-predictability/REFERENCES.md), [sources checked in part](papers/02-determinism-and-predictability/SOURCE-CHECK.md) |

`models/` holds the computational work supporting the papers. Empty until
paper 02 reaches the simulation stage.

## The through-line

The framework and the second paper are the same argument approached from
opposite ends.

SIMEA says decisions are generated externally to a measurable degree. Paper 02
takes that seriously and asks what it implies for forecasting: if behaviour is
steered, it is more predictable, and predictability stops being a fixed property
of a market and becomes a coordinate that moves with autonomy. Systemic
influence buys forecastability, and it pays for it in agency.

That trade is the subject of the programme.

## Open problems

1. **Operationalising *AT*.** The Autonomy Threshold is a construct, not yet an
   instrument. Most of the empirical work in paper 02 is blocked on it.
2. **Aggregation.** Individually steered agents may still aggregate to an
   unpredictable price. Whether the trade-off survives aggregation is unresolved
   and may bound the whole claim.
3. **Distinguishing SIMEA from adaptive-markets accounts.** Both make efficiency
   variable. The obvious contrast — steering versus evolutionary fitness — does
   not hold, because Lo's adaptive markets hypothesis is itself built on Simon's
   bounded rationality. What remains is that Lo's agents adapt to an
   environment while SIMEA's are steered by an interested party, and that has to
   be made sharp enough to be tested.

## Status and how to read this

Everything here is work in progress and is published in that state
deliberately. Drafts carry their own limitations sections, and the positioning
note for paper 02 includes an explicit list of what would sink its argument.
Citations in working documents are marked where they have not yet been verified
against the original sources. Paper 02's bibliography has been through a
verification pass and lives in
[REFERENCES.md](papers/02-determinism-and-predictability/REFERENCES.md); that
pass confirmed the works exist as cited. A second pass,
[SOURCE-CHECK.md](papers/02-determinism-and-predictability/SOURCE-CHECK.md),
asks whether each source says what the note claims it says. Six of the twenty
works have been through it; two claims failed and are corrected in the note.
Fourteen remain unchecked, and the file says which.

Corrections and objections are welcome via issues.

## Licence

Written material CC BY 4.0; code MIT. See [LICENSE](LICENSE).
