# Determinism and the Predictability of Financial Futures

**Research positioning note — working document**
Kerem Özdemir · August 2026

---

## 1. The question, stated precisely

The intuition to be examined:

> If determinism is true — if every decision is in principle knowable — then the
> financial future is predictable.

Stated this way the claim is an inference from a metaphysical premise to an
epistemic conclusion. The premise concerns what *is fixed*; the conclusion
concerns what *can be known*. The whole research programme lives in the gap
between those two, and the first task of the paper is to show that the gap does
not close.

Three distinct claims must be kept apart, because the literature routinely
conflates them:

| Claim | Type | Content |
| --- | --- | --- |
| **D — Determinism** | Metaphysical | The state of the system at *t* fixes its state at *t+1*. |
| **P — Predictability in principle** | Epistemic | An agent with sufficient information could derive *t+1* from *t*. |
| **F — Forecastability in practice** | Practical | An agent embedded in the system can produce useful forecasts. |

D → P → F is the intuitive chain. **Both arrows fail**, and the second fails for
reasons specific to markets rather than for generic reasons about knowledge.

The thesis of this paper is stronger than the standard sceptical position:

> **Even under full metaphysical determinism, financial markets are
> unpredictable in principle — not merely in practice.** The obstruction is
> structural, not a shortfall of data or computing power.

And then the SIMEA-specific claim, which is where the contribution sits:

> **Predictability is not a fixed property of a market. It is a variable, and it
> moves inversely with autonomy.** Systemic influence purchases forecastability
> at the price of agency.

---

## 2. Why D → P fails

### 2.1 The Laplacean baseline

Laplace's demon (Laplace, 1814) is the clean statement of D → P: an intellect
knowing all forces and all positions, and vast enough to analyse them, would
have nothing uncertain, and the future would be present before its eyes. The
paper should open here, because the demon is exactly the position the naïve
version of the question assumes, and every subsequent argument is a limitation
on it.

Note what Laplace already conceded: the demon requires *vastness*. He located
probability in human ignorance, not in the world.

### 2.2 Sensitive dependence (chaos)

Lorenz (1963, pp. 130, 141) established that a fully deterministic system of
three ordinary differential equations produces bounded nonperiodic trajectories
that are unstable under arbitrarily small modifications of the initial state,
and concluded that "prediction of the sufficiently distant future is impossible
by any method, unless the present conditions are known exactly" (p. 141). With
finite measurement precision — and measurement precision is always finite —
predictability collapses at a finite horizon. Determinism is untouched.

The *rate* is a separate citation: Lorenz (1963) shows instability, not an
exponent. Lorenz (1965) supplies the quantitative version, with error-doubling
times on the order of days and a predictability horizon that varies with the
circulation pattern. Cite 1963 for the result and 1965 for the rate.

For the paper, the relevant move is that this is not an argument about
complexity or about markets being "messy." It is a proof that D does not imply
P even for a three-variable system that a first-year student can write down.

### 2.3 Computational irreducibility

Wolfram (2002, ch. 12 §6, pp. 737–750) argues that for a broad class of
deterministic systems there exists no computational shortcut to the state at
step *n*: the fastest way to know the outcome is to run the system. If a market
is computationally irreducible in this sense, then the cheapest complete
forecast of tomorrow costs one day. Wolfram makes the move to markets himself in
ch. 8 §8, pp. 429–432, and the paper should engage that rather than leave a
referee to find it.

This argument is weaker than the chaos argument — irreducibility rests on the
Principle of Computational Equivalence (ch. 12 §§2–4, pp. 716–734), which
Wolfram presents as a principle supported by examples rather than a theorem —
and the
paper should present it as suggestive rather than load-bearing. It earns its
place because it survives the objection "but with enough compute": no amount of
compute buys a shortcut that does not exist.

### 2.4 Self-prediction

Popper (1950, Part I) argued that a predictor which is part of the system it
predicts cannot in general predict that system: it cannot obtain up-to-date
information about its own state, because obtaining it alters that state, and so
"no member of such a society can fully predict the future states of that
society, or those of any of its members" (p. 118).

Two things about this argument are easy to get wrong and were got wrong in
earlier drafts of this note.

*It is a physical claim, not a logical one.* Popper is explicit: "The
impossibility asserted is therefore a physical impossibility — that of
successfully carrying out certain physical operations involved in obtaining
predictions in accordance with the methods of science" (p. 118). His predictor
is a machine subject to mechanics, not a formal system, and he separates the
result from Bohr's complementarity (p. 119). Reading it as an undecidability
result invites the objection that formal systems can be built to avoid
self-reference, which is not the obstruction he identifies.

*It is not independent of §2.2.* The mechanism is the breakdown of a "one-way
membrane" between predictor and predicted, and that breakdown requires both
sides to amplify: "a predictor B must be an amplifier simply because some small
differences in the system A may become amplified in A itself in the course of
time" (p. 129). Sensitive dependence is doing work here. Popper suspects the
amplification requirement holds for recording alone and would then be
independent — but marks it as a belief, not a result (p. 129 n. 1). The claim of
independence rests on the self-prediction theorem of §8 and Part II, which this
note has not yet read.

One further caution about recruiting Popper. His conclusion is *indeterminism*:
classical mechanics, he argues, is inconsistent with the finite deterministic
doctrine. That is compatible with this paper's conditional thesis only because
his target is scientific determinism — determinism read as predictability by the
methods of science (p. 124) — and not the metaphysical doctrine, which he holds
untestable and declines to refute (pp. 121–122). That separation is precisely
the D/P distinction of §1, and §1 should cite it as precedent rather than
present it as new.

Aaronson (2013) revisits related territory from computational complexity, and
is worth reading for the care with which he separates what indeterminism could
and could not buy. The paper should avoid leaning on quantum indeterminacy —
it is a common move and a weak one, since decoherence at the scale of an order
book makes it irrelevant, and because indeterminism would *reduce*
predictability rather than rescue agency.

---

## 3. Why P → F fails specifically in finance

Sections 2.2–2.4 are general limits on knowledge. Finance has its own, sharper
obstruction, and this is where the paper stops being philosophy of science and
becomes economics.

### 3.1 A forecast, once acted on, alters what it forecasts

Samuelson (1965) proved that properly anticipated prices form a **martingale**:
if a price movement is foreseen, it is transacted immediately, and the
foreseeable component vanishes from the future path into the present price.
Predictability in markets is *self-consuming* in a way that predictability of
the weather is not. Knowing tomorrow's rainfall does not change tomorrow's
rainfall.

The paper's title says "fluctuate randomly" and the paper should not repeat it.
A martingale restricts the conditional mean and nothing else — not independence,
not identical distribution, not constant variance. Volatility is forecastable
inside the theorem, and a great deal of quantitative finance lives in exactly
that gap. Stating the result as a martingale property is also the honest
version: Samuelson did not regard the unpredictability of price changes as a
good test of the theory, which is a point on this paper's side, since it is the
P/F distinction of §1 arriving sixty years early.

This is the single most important structural point in the paper. It converts
the question from "can we know enough?" to "can a fact about the future survive
being known?"

### 3.2 The impossibility of informationally efficient markets

Grossman and Stiglitz (1980, p. 393) close the loop. If prices fully reflected
all information, no agent would have an incentive to bear the cost of acquiring
information; but then no one would acquire it, and prices could not reflect it.
What the market settles at instead is "an equilibrium degree of disequilibrium",
in which prices aggregate private information only partially — "this is perhaps
lucky, for were it to do it perfectly, an equilibrium would not exist."

Note the gap the paper has to bridge rather than step over. Grossman–Stiglitz is
a result about *informational efficiency*, not about forecastability: a price
system can fail to aggregate information and still be hard to predict. The
argument that perfect informational efficiency is self-refuting does not by
itself deliver the claim that perfect predictability is self-refuting. Either
that bridge is built or the section narrows its claim.

Fama (1970) provides the efficient-markets framing that Grossman–Stiglitz
undercuts, and should be treated as the position being qualified rather than a
straw man.

### 3.3 Reflexivity

Soros (1987; and the more careful statement in Soros, 2013) generalises this:
participants' beliefs about the market are part of the market, so the object of
knowledge is altered by the act of knowing it. Popper's "Oedipus effect" (Popper,
1957) is the same structure — the prophecy that causes its own fulfilment or
its own defeat.

The reflexivity literature is the natural home for this paper, but it is also
notoriously loose. The contribution below is an attempt to make one part of it
measurable.

### 3.4 Model dependence

The Lucas critique (Lucas, 1976) shows that a relationship estimated under one
policy regime cannot be assumed to survive a change in that regime, because the
agents whose behaviour generated the relationship will re-optimise. Any
forecasting model that succeeds becomes part of the environment its subjects
respond to.

Timmermann and Granger (2004) work through the practical consequence: stable
forecasting patterns "will self-destruct when discovered by a large number of
investors", so a forecasting edge is a depreciating asset. Proposition 2 in §4.1
must be stated against this, not alongside it — the erosion mechanism is already
theirs, and what is left to claim is the escalation response.

---

## 4. Where SIMEA enters

Sections 2 and 3 are established results. Assembled well they make a good
literature review, not a new paper. The contribution has to come from somewhere
else.

SIMEA supplies it. If economic agents are decision-subjects steered by systems
rather than autonomous optimisers — the core claim of the framework — then the
degree to which behaviour is *generated externally* varies across agents,
markets and time. And externally generated behaviour is, by construction, more
predictable than autonomously generated behaviour: it is a function of an input
the modeller can in principle observe.

This yields the central proposition:

> **Proposition 1 (Autonomy–predictability trade-off).** The forecastability of
> an agent's decisions is decreasing in the Autonomy Threshold *AT* and
> increasing in the magnitude of the Influence Gradient *IG*.

Predictability stops being a property of markets and becomes a *coordinate*:
markets slide along an axis between "deterministic and forecastable" and "free
and unforecastable," and SIMEA's influence variables set the position.

This reframes the original question. The interesting answer to "if determinism
is true, is the financial future predictable?" is not yes or no. It is:

> Predictability was never the consequence of determinism. It is the consequence
> of *influence*. A world can be fully deterministic and unforecastable; a world
> can be indeterministic in its foundations and highly forecastable at the level
> where the steering happens.

### 4.1 The self-defeating loop

Proposition 1 is not the end of the argument, because Section 3.1 has not gone
away.

> **Proposition 2 (Erosion).** Predictability generated by systemic influence is
> arbitraged away once identified, which pushes influence architectures to
> escalate — to steer harder in order to restore an edge that their own success
> destroyed.

This gives the paper a dynamic rather than a static conclusion, and it is
falsifiable in a way most reflexivity writing is not. It also connects to
SIMEA's welfare function: if the equilibrium of this loop is escalating
influence, then autonomy is consumed as a byproduct of the search for
forecastability, and the welfare cost is not incidental but systematic.

### 4.2 What this predicts

| # | Proposition | Where to look |
| --- | --- | --- |
| 3 | Flow segments with high algorithmic mediation are more forecastable than low-mediation segments, controlling for liquidity | Retail app order flow, robo-advised rebalancing, passive index flows vs discretionary institutional flow |
| 4 | Forecastability of a mediated segment decays after the mediation mechanism becomes publicly known | Event studies around disclosure of recommender or flow-payment arrangements |
| 5 | Rising influence intensity coincides with falling cross-sectional dispersion of individual decisions | Dispersion of retail holdings and trade timing over the platform era |
| 6 | The autonomy-weighted welfare measure diverges from realised utility precisely where forecastability is highest | SIMEA welfare function applied to high- and low-mediation cohorts |

Propositions 3–5 are testable with data that exists. Proposition 6 is where the
normative payload sits and is the harder one.

---

## 5. What could sink the argument

Written honestly, this section is what makes the paper credible.

- **The trade-off may be trivially true.** "Behaviour caused by an observable
  input is easier to predict" risks being definitional. The paper must specify
  *IG* and *AT* so that Proposition 1 could come out false — otherwise it is not
  a finding.
- **Aggregation may dissolve the effect.** Individually predictable agents can
  aggregate to an unpredictable price if the influence is heterogeneous. The
  claim may hold at the level of flows and fail at the level of prices, which
  would be a real result but a narrower one than it first appears.
- **Measuring autonomy is unsolved.** *AT* is currently a construct, not an
  instrument. Without an operational measure Propositions 3–5 cannot be taken to
  data, and building that measure may be a paper of its own.
- **Adaptive markets may already cover this, and the planned escape does not
  work.** Lo (2004) frames efficiency as varying with the ecology of
  participants. The distinction previously proposed here — that SIMEA locates
  variation in *who is steering whom* rather than in evolutionary fitness —
  contrasts against a version of Lo that does not exist: AMH is built by
  extending Simon's satisficing with evolutionary dynamics, and absorbs the
  behavioural anomalies as adaptive heuristics. It is already a
  bounded-rationality framework. A distinction is still available — Lo's agents
  adapt to an *environment*, SIMEA's are steered by an *interested party* with
  its own objective function — but it must be made on that axis and must survive
  the reply that a recommender system is a plausible environment. If it cannot,
  the contribution collapses into an existing framework.
- **Determinism may be doing no work at all.** A reasonable referee will ask
  whether the metaphysical premise is load-bearing or decorative. One honest
  answer is that it is a framing device — the paper's real subject is the
  structure of predictability — and it may be cleaner to say so than to defend a
  metaphysical commitment the argument does not need.

---

## 6. Proposed structure

1. **Introduction** — the Laplacean intuition and why it is intuitive
2. **Three concepts, not one** — D, P, F separated
3. **General limits** — chaos, irreducibility, self-prediction
4. **The finance-specific limit** — self-consuming predictability; Samuelson,
   Grossman–Stiglitz, reflexivity, Lucas
5. **Interim conclusion** — determinism does not deliver predictability, and
   nothing else will either
6. **Predictability as a variable** — SIMEA; Propositions 1 and 2
7. **Empirical implications** — Propositions 3–6 and identification strategy
8. **Limitations** — Section 5 above, unabridged
9. **Welfare and policy** — autonomy as the quantity being consumed
10. **Conclusion**

Sections 1–5 are a literature review with a sharp edge. Sections 6–7 are the
contribution. Section 8 is what separates this from a blog post.

---

## 7. Reading list

**Determinism and prediction**

- Laplace, P.-S. (1814). *Essai philosophique sur les probabilités.*
- Lorenz, E. N. (1963). Deterministic nonperiodic flow. *Journal of the Atmospheric Sciences*, 20(2).
- Popper, K. (1950). Indeterminism in quantum physics and in classical physics. *British Journal for the Philosophy of Science*, 1(2–3).
- Popper, K. (1957). *The Poverty of Historicism.* — the Oedipus effect
- Wolfram, S. (2002). *A New Kind of Science.* — computational irreducibility
- Aaronson, S. (2013). The ghost in the quantum Turing machine.

**Markets, information and reflexivity**

- Samuelson, P. (1965). Proof that properly anticipated prices fluctuate randomly. *Industrial Management Review*, 6.
- Fama, E. (1970). Efficient capital markets. *Journal of Finance*, 25(2).
- Grossman, S. & Stiglitz, J. (1980). On the impossibility of informationally efficient markets. *American Economic Review*, 70(3).
- Lucas, R. (1976). Econometric policy evaluation: a critique.
- Soros, G. (2013). Fallibility, reflexivity, and the human uncertainty principle. *Journal of Economic Methodology*, 20(4).
- Timmermann, A. & Granger, C. (2004). Efficient market hypothesis and forecasting. *International Journal of Forecasting*, 20(1).
- Lo, A. (2004). The adaptive markets hypothesis. *Journal of Portfolio Management*, 30(5).
- Hayek, F. (1945). The use of knowledge in society. *American Economic Review*, 35(4).

**Agency and systemic influence**

- Simon, H. (1955). A behavioral model of rational choice. *Quarterly Journal of Economics*, 69(1).
- Kahneman, D. & Tversky, A. (1979). Prospect theory. *Econometrica*, 47(2).
- Thaler, R. & Sunstein, C. (2008). *Nudge.*
- Zuboff, S. (2019). *The Age of Surveillance Capitalism.*
- Arthur, W. B. et al. (1997). Asset pricing under endogenous expectations in an artificial stock market.

> **Verification note (updated 18 August 2026).** The list above is the working
> shorthand and is superseded by **[REFERENCES.md](REFERENCES.md)**, which
> carries the verified form of every entry. All twenty were checked against
> publisher or DOI-level records; none was removed, and ten needed correction.
> Notably, Soros (1987) is cited in §3.3 above but was missing from this list
> entirely, and Aaronson is dated here to the 2013 preprint rather than the 2016
> published chapter. **Cite from REFERENCES.md, not from this section.**
>
> A second pass, **[SOURCE-CHECK.md](SOURCE-CHECK.md)**, asks whether each source
> says what this note claims it says. Six works were checked; four claims held
> and two did not. §2.4 misdescribed Popper's argument as logical when he calls
> it physical, and asserted an independence from chaos that his own text does not
> support; §3.1 called a martingale theorem a randomness result. Both are
> corrected above. Lorenz (1965) is added for the error-growth rate.
>
> Fourteen works remain unchecked substantively, including all of the agency and
> influence section. SOURCE-CHECK.md §5 lists them.

---

## 8. Open decisions

1. **Is determinism load-bearing or a frame?** Section 5 argues it may be
   decorative. Decide before drafting — it changes the title and the first
   three sections.
2. **Theory paper or empirical paper?** Propositions 3–5 are testable but
   require an operational *AT*. A theory paper can be written now; an empirical
   one needs the measurement work first.
3. **Simulation as evidence?** An agent-based market with a tunable autonomy
   parameter would demonstrate Propositions 1 and 2 cleanly and is achievable.
   It is evidence about a model rather than about markets, which is a real
   limitation and should be stated as one.
4. **Venue.** The argument is interdisciplinary enough that the venue will shape
   how much philosophy survives the edit.
