# Substantive source check — paper 02

**Pass completed 18 August 2026.** Companion to
[REFERENCES.md](REFERENCES.md), which established that the works exist as
cited. This pass asks the harder question: **does each source actually say what
[POSITIONING.md](POSITIONING.md) claims it says?**

Six claims were checked against primary text. **Four hold. Two do not, and one
of those two is load-bearing.** Page-level citations for everything checked are
in §3.

**Scope, stated honestly.** Six of the twenty works in REFERENCES.md were
checked at the level of primary text: Popper (1950, Part I), Lorenz (1963),
Wolfram (2002), Grossman & Stiglitz (1980), Samuelson (1965) and Lo (2004).
Popper Part II, Laplace, Fama, Lucas, Soros, Aaronson and the whole
agency-and-influence section have **not** been checked substantively; §4 lists
them. Where a work was reached only through a secondary source or an abstract
rather than the full text, this is said in the entry.

---

## 1. Claims that do not survive the check

### 1.1 §2.4 — Popper's argument is described as logical; it is physical

The note says the predictor problem is one where "the required self-reference
generates the familiar undecidability."

Popper says the opposite, in the paper's second page:

> "The impossibility asserted is therefore a physical impossibility — that of
> successfully carrying out certain physical operations involved in obtaining
> predictions in accordance with the methods of science."
> — Popper (1950, Part I, p. 118)

He is explicit that his predictor is a *machine* — "a classical mechanical
calculating and predicting machine ... capable of being interpreted as
predictions of the positions, velocities, and masses of physical particles"
(p. 118) — and that the limit follows from what such a machine can physically
do, not from a Gödel- or Tarski-style diagonal argument. He separately
distinguishes his result from Bohr's complementarity (p. 119).

**Fix:** drop "undecidability". The argument is that a predictor embedded in the
world cannot obtain up-to-date information about its own state, because
obtaining it changes that state. That is a stronger claim for the note's
purposes than the logical gloss, because it cannot be dissolved by pointing at
formal systems that avoid self-reference.

### 1.2 §2.4 — "independent of chaos" is false for the argument Popper gives

The note says: "This argument is independent of chaos: it bites even for systems
that are perfectly stable."

The argument in Popper's §7 depends on amplification, and amplification is
introduced *because* of sensitive dependence:

> "A must, under certain circumstances, interfere strongly with B. It must do so
> because some minute differences at the instant of time t₀ may, in a mechanical
> system such as A, give rise to considerable differences at the instant of time
> t₁ ... a predictor B must be an amplifier simply because some small differences
> in the system A may become amplified in A itself in the course of time."
> — Popper (1950, Part I, p. 129)

The one-way membrane between predictor and predicted breaks down precisely when
both sides amplify. Take away sensitive dependence and the mechanism Popper
describes has nothing to work on.

Popper hedges this himself in a footnote on the same page — he believes
predictors must be amplifiers "merely as recorders of measurements", which would
make the argument independent of amplification *in the system* — but he marks it
as a belief, not a result: "it might also be shown, I believe" (p. 129 n. 1).

**Fix:** §2.4 cannot be presented as an obstruction independent of §2.2. Either
say the two are entangled, or rest the independence claim on the self-prediction
theorem in Part I §8 / Part II — which has not been read and therefore cannot
yet be leaned on. Marked outstanding in §4.

### 1.3 §3.1 — Samuelson proved a martingale property, not randomness

The note says Samuelson "proved that properly anticipated prices fluctuate
randomly." That is the title, and the title overstates the theorem.

The result is that properly anticipated prices form a **martingale** — a
restriction on the conditional mean only. A martingale is not a random walk: it
implies nothing about independence, identical distribution, or constant
variance. Lo's own history of the hypothesis puts the theorem in those terms
("In mathematical terms, prices follow martingales", Lo, *Efficient Markets
Hypothesis*, 2007 survey, p. 3) and notes that the random-walk hypothesis and
the martingale model are two *different* statistical descriptions that the early
literature ran together (pp. 3–4).

Two consequences for §3.1. First, "fluctuate randomly" cannot be used to license
the strong reading that no structure is forecastable; serial dependence in
higher moments is entirely consistent with the theorem, and volatility
forecasting lives in exactly that gap. Second, Samuelson himself did not treat
unpredictability of price changes as a good test of the theory — a point the
note should adopt rather than argue against, since it supports the paper's own
separation of P from F.

**Fix:** state the theorem as a martingale result, and say what it does and does
not restrict. The note's substantive point — that a foreseen movement is
transacted into the present price and vanishes from the future path — survives
intact. Only the word "randomly" has to go.

**Caveat on this entry.** Samuelson (1965) was reached through Lo's survey and
through the secondary literature on the martingale/random-walk distinction, not
through the *Industrial Management Review* text. The martingale characterisation
is not in dispute anywhere in that literature, but the specific caveats
Samuelson attaches in his own words have not been read at source and are not
quoted here.

---

## 2. Claims that hold

### 2.1 §2.2 — Lorenz, with one word to fix

The conclusion is Lorenz's, close to verbatim:

> "When our results concerning the instability of nonperiodic flow are applied to
> the atmosphere, which is ostensibly nonperiodic, they indicate that prediction
> of the sufficiently distant future is impossible by any method, unless the
> present conditions are known exactly."
> — Lorenz (1963), final section, p. 141

The abstract states the mechanism: bounded nonperiodic solutions are "ordinarily
unstable with respect to small modifications, so that slightly differing initial
states can evolve into considerably different states."

**One correction.** The note says prediction error "grows exponentially in the
forecast horizon." Lorenz (1963) establishes instability and divergence; the
exponential rate, and the error-doubling time that makes it quantitative, come
from Lorenz (1965) — the 28-variable study, where the figures are scaled so that
a forty-five-degree slope is a four-day doubling time, and where the time for
observational-scale errors to become intolerable is found to vary from a few
days to a few weeks depending on the circulation pattern. Cite 1963 for the
result and 1965 for the rate.

*Reached through:* the 1963 conclusion and abstract via secondary quotation; the
1965 findings via the Tellus abstract and the NOAA review of Lorenz's
predictability work. Neither full text was opened.

**New reference to add:** Lorenz, E. N. (1965). A study of the predictability of
a 28-variable atmospheric model. *Tellus*, 17(3), 321–333.
DOI 10.1111/j.2153-3490.1965.tb01424.x

### 2.2 §2.3 — Wolfram, correctly characterised and correctly hedged

Computational irreducibility is ch. 12 §6, pp. 737–750. Wolfram frames it
exactly as the note does — as the failure of the shortcut that theoretical
science normally supplies:

> "at some level almost all of them are based on finding ways to reduce the
> amount of computational work that has to be done in order to predict how some
> particular system will behave ... to derive a mathematical formula that allows
> one to determine what the outcome of the evolution of the system will be
> without explicitly having to trace its steps."
> — Wolfram (2002, p. 737)

The note's decision to treat irreducibility as suggestive rather than
load-bearing is right on the text's own terms: it rests on the Principle of
Computational Equivalence (ch. 12 §§2–4, pp. 716–734), which Wolfram presents as
a principle supported by examples, not a theorem.

**Worth adding.** Wolfram applies this apparatus to markets directly in ch. 8 §8,
"Financial Systems", pp. 429–432. The note cites Wolfram only for the general
argument and does not mention that he has already made the finance move. A
referee will.

### 2.3 §3.2 — Grossman–Stiglitz, verbatim on the note's reading

From the paper's opening paragraphs:

> "the assumptions that all markets, including that for information, are always
> in equilibrium and always perfectly arbitraged are inconsistent when arbitrage
> is costly. We propose here a model in which there is an equilibrium degree of
> disequilibrium ... In general, however, it does this imperfectly; this is
> perhaps lucky, for were it to do it perfectly, an equilibrium would not exist."
> — Grossman & Stiglitz (1980, p. 393)

The note's "self-refuting" language is a fair rendering of "an equilibrium would
not exist."

**One imprecision.** Grossman–Stiglitz is about *informational efficiency* —
whether prices aggregate private information — not about predictability. The
note slides between the two. They are related but not identical: a price system
can fail to aggregate information and still be hard to forecast. §3.2 should
either argue the bridge or narrow the claim.

### 2.4 §3.4 — Timmermann & Granger, on the note's side and stronger than quoted

The paper states the decay claim directly:

> "stable forecasting patterns are therefore unlikely to persist for long periods
> of time and will self-destruct when discovered by a large number of investors"
> — Timmermann & Granger (2004, abstract; argument developed pp. 15–27)

This is a better fit for Proposition 2 (Erosion) in §4.1 than the note currently
makes of it. §4.1 presents erosion as new; Timmermann and Granger have already
stated the mechanism. The novelty in Proposition 2 is not the erosion but the
*escalation response* — that influence architectures steer harder to restore the
edge. §4.1 should say so, or the proposition will read as a restatement.

*Reached through:* the published abstract and the paper's summary in indexing
records; the full text was not opened.

---

## 3. The §5 risk is worse than §5 says

§5 proposes to distinguish SIMEA from Lo (2004) by locating variation in "who is
steering whom, not in evolutionary fitness."

Lo's abstract undercuts the framing. The adaptive markets hypothesis is built by
"extending Herbert Simon's notion of 'satisficing' with evolutionary dynamics",
and it explicitly absorbs the behavioural anomalies — loss aversion,
overconfidence, overreaction, mental accounting — as adaptive heuristics. AMH is
therefore already a bounded-rationality framework with an evolutionary engine
bolted on, not a pure fitness story. The contrast the note wants to draw is
against a version of Lo that does not exist.

There is still a distinction available — Lo's agents adapt to an *environment*,
whereas SIMEA's are steered by an *interested party* with its own objective
function — but it has to be made on that axis, and it has to survive the
observation that a recommender system is a plausible environment. This
strengthens rather than weakens the §5 warning, and it is compounded by the
finding already in REFERENCES.md §3: Simon (1955) sits in the note's reading
list uncited, while Lo has built on him.

*Reached through:* the published abstract and the SSRN record. The full JPM text
was not opened.

---

## 4. Page-level citations established

| Claim in note | Cite as |
| --- | --- |
| §2.2 instability, no long-range prediction | Lorenz (1963), pp. 130, 141 |
| §2.2 exponential rate, doubling time | Lorenz (1965), *Tellus* 17(3), 321–333 |
| §2.3 no computational shortcut | Wolfram (2002), ch. 12 §6, pp. 737–750 |
| §2.3 irreducibility rests on PCE, not a theorem | Wolfram (2002), ch. 12 §§2–4, pp. 716–734 |
| §2.3 Wolfram's own application to markets | Wolfram (2002), ch. 8 §8, pp. 429–432 |
| §2.4 impossibility is physical, not logical | Popper (1950, I), p. 118 |
| §2.4 predictor cannot predict its own future states | Popper (1950, I), p. 118; proof §8 / Part II |
| §2.4 amplification and the one-way membrane | Popper (1950, I), p. 129 |
| §1 D and P must be separated | Popper (1950, I), pp. 121–124 |
| §3.2 equilibrium degree of disequilibrium | Grossman & Stiglitz (1980), p. 393 |
| §3.4 exploited predictability self-destructs | Timmermann & Granger (2004), pp. 15–27 |

**Precedent worth claiming rather than reinventing.** Popper's Part I already
performs the note's central distinction: he separates the *metaphysical* doctrine
of determinism, which he calls untestable (pp. 121–122), from a "finite version"
defined as predictability by scientific method (p. 124), and refutes only the
latter. That is D versus P. §1 of the note should cite it as precedent — the
separation is the paper's foundation, and it is stronger for having a canonical
source than for appearing to be new.

**A framing problem this exposes.** Popper's conclusion is *indeterminism*: he
argues classical mechanics is inconsistent with the finite deterministic
doctrine. The note's thesis is conditional — "even under full metaphysical
determinism". Those are compatible only because Popper's target is scientific
determinism rather than the metaphysical doctrine, which he holds untestable and
declines to refute. §2.4 should make that explicit; otherwise the note appears to
recruit an indeterminist to an argument that assumes determinism.

---

## 5. Still outstanding

- **Popper Part II** (*BJPS* 1(3), 173–195) and Part I §8 — the self-prediction
  proof itself. §1.2 above cannot be settled without it.
- **Laplace (1814)** — the demon passage has not been located at page level in
  either the French original or the Truscott & Emory translation. The note also
  claims Laplace "located probability in human ignorance"; unverified at source.
- **Fama (1970), Lucas (1976), Soros (1987, 2013), Aaronson (2016)** — not
  checked substantively. Aaronson is the most urgent: REFERENCES.md §3 already
  flags that §2.4 asks a hundred-page chapter to support two distinct claims
  with no page pinned to either.
- **The entire agency-and-influence section** — Hayek, Simon, Kahneman &
  Tversky, Thaler & Sunstein, Zuboff, Arthur et al. Nothing to check
  substantively while the body cites none of them. That is the backlog item
  "Cite the agency literature or drop it", and §3 above raises its priority:
  Simon is now known to be doing work inside the framework the note must
  distinguish itself from.
- **Full texts.** Only Popper Part I, Wolfram p. 737 and the Grossman–Stiglitz
  opening were read at source. Lorenz, Samuelson, Timmermann–Granger and Lo were
  reached through abstracts, publisher records or secondary quotation. Entries
  say so individually. A manuscript pass will need the full texts.
