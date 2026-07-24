# When Should a Low-Capacity State Deploy an AI System?

**A readiness filter, with three worked examples from Sierra Leone**

Akwasi Appiah Obeng | July 2026

---

## The problem this solves

Funders and governments are building pipelines of AI use cases for African public services faster than anyone is building the filter that decides which ones should proceed. The pipeline question is treated as a supply problem: find more use cases. It is closer to a selection problem: most candidate deployments are plausible, few are ready, and the difference is not visible from the proposal.

This is a filter for that judgment. It comes out of advising a government that is actively deploying AI across its public services, and it is built on one distinction that most readiness assessments miss.

---

## The distinction that does the work

The same AI system plays a different role depending on the setting it enters.

In a high-capacity state, a tool typically **augments** an existing professional capacity. It makes an established workflow faster or more consistent. There is a body of practitioners who can judge its output, override it, and carry on without it.

In a low-resource state, the same tool often **substitutes** for a capacity that is scarce or absent. It performs the function rather than enhancing it. A diagnostic tool supporting a large body of radiologists is an augmentation. The same tool deployed where there is roughly one radiologist per hundred thousand people is a substitution.

Substitutes are load bearing from the day they launch. This produces two properties that ordinary readiness frameworks do not capture:

- **They are hard to remove**, because there is little prior capacity to fall back to.
- **They are hard to evaluate**, because judging them requires the very expertise whose absence made them necessary.

The practical consequence is counterintuitive but firm. AI deployments in low-resource settings warrant *more* scrutiny before launch, not less. And pre-deployment is the decisive moment, because it is the last point at which external expertise can still be brought to bear before workflows reorganise around the system and reversal becomes politically and operationally costly.

---

## The filter

Five questions, applied before public commitment. The first two are diagnostic. The last three are gates: a deployment that fails any of them is not ready, regardless of model performance.

**1. Augmentation or substitution?**
Does this system assist a capacity that exists, or perform a function the state currently cannot? Answer determines how hard the remaining questions bite.

**2. What is the exposure surface?**
Who bears the cost of a wrong output, and how directly? Rank: internal government process, official decision support, frontline worker guidance, direct citizen interaction. Risk rises sharply at each step.

**3. GATE — Is there a preserved fallback?**
If the system fails, is withdrawn, or is suspended, how does the service continue? A named fallback that has been tested, not an assumption that staff will revert to the old way. Substitution deployments frequently have none, and nobody notices until the vendor exits.

**4. GATE — Is it reversible, and at what cost?**
What does exit cost at six months, at eighteen, at three years? If the honest answer is that reversal becomes impossible once workflows adapt, the deployment decision is effectively permanent and should be treated as one.

**5. GATE — Can it be evaluated locally, by someone?**
Who in-country can judge whether this is working? If nobody can, the state is accepting vendor claims indefinitely. Either build or contract that judgment before launch, or do not launch.

---

## Three worked examples

Three deployment types drawn from a single West African state's current AI activity. All three are plausible. They score very differently.

### A. Governance and assurance function

*A pre-deployment review capability inside government, maintaining an inventory of state AI systems and reviewing high-risk deployments before commitment.*

Augmentation or substitution: neither, strictly. It creates a capacity that does not exist rather than replacing one. Exposure surface: internal. No citizen-facing output. Fallback: the status quo, which is fragmented review through procurement teams and donor projects. Reversibility: high, an institution can be wound down without harming service users. Local evaluation: yes, its own outputs are documents and determinations that can be inspected.

**Verdict: proceed.** Low risk, and it is the enabling condition for the other two. This is the deployment that makes the rest of the pipeline assessable.

### B. Decision support with human ground truthing

*Satellite-based yield forecasting feeding a government planning function, with field agents verifying predictions against ground observation.*

Augmentation or substitution: substitution in effect. It replaces manual survey capacity that is thin, not a strong existing forecasting profession. Exposure surface: official decision support. A wrong forecast produces a worse planning or procurement call, not direct citizen harm. Fallback: manual survey persists but degrades if the model becomes the default and survey capacity is redirected. This is the live risk and it is manageable if named. Reversibility: moderate. Ground truthing preserves the human judgment loop, which is precisely what keeps exit cheap. Local evaluation: yes, and unusually clean, because forecasts can be scored against realised harvest.

**Verdict: proceed with a fallback condition.** Approve on the explicit condition that survey capacity is maintained rather than reallocated on the strength of the model. The ground truthing design is what makes this tier work, and it should be treated as a requirement, not a feature.

### C. Citizen-facing agentic service in a health context

*A multilingual conversational layer delivering maternal health guidance and appointment follow-up directly to caregivers in local languages, with escalation to human health workers.*

Augmentation or substitution: substitution, in the strongest form. It delivers guidance where the health worker to population ratio means the alternative is frequently nothing. Exposure surface: direct citizen interaction, in a clinical domain, with a low-literacy user group that cannot readily assess whether advice is wrong. Highest exposure of the three by a wide margin. Fallback: must be specified precisely. What happens to a registered pregnancy when the service is down? Reversibility: low once caregivers rely on it. Local evaluation: hard. Judging clinical guidance quality in four languages requires exactly the scarce clinical and linguistic expertise the system exists to stretch.

**Verdict: highest value, highest risk, and the one that most needs the review function in example A to exist first.** Not a reason to stop. It is a reason to sequence: the escalation thresholds, the confidence scoring, and the human override path are not implementation details here, they are the deployment decision.

---

## What would tell us it worked

Readiness is a prediction. It should be checked. For each tier, the evidence that would settle it:

| Tier | Primary question | Evidence to collect |
|---|---|---|
| A. Governance | Did review change any deployment decision? | Count of reviews where conditions were imposed, deployments delayed, or systems rejected; whether decisions held |
| B. Decision support | Are forecasts better than the counterfactual, and did fallback survive? | Forecast error against realised yield; survey capacity headcount tracked over time as the leading indicator of hidden substitution |
| C. Citizen-facing | Did guidance quality hold, and did escalation work? | Clinician-adjudicated sample of outputs by language; escalation rates against a defined expected range; differential outcomes by language, since failure will not be uniform |

The third row carries a warning worth stating. Evaluation capacity is itself the constraint. If a state cannot assemble the expertise to adjudicate a sample of AI-generated clinical guidance in four languages, it is not in a position to evaluate the system, and that is a finding about readiness rather than a gap to be filled later.

---

## Why this framing matters for pipeline building

A pipeline sorted only by opportunity produces a list where the most attractive use cases are frequently the least ready, because attractiveness and exposure rise together. The systems that promise the most, citizen-facing services in health and education, are exactly the ones where substitution is deepest, reversal is hardest, and local evaluation is least available.

Sorting by readiness instead produces a sequence rather than a list. Build the assurance layer first, because it is cheap and reversible and makes everything after it assessable. Take the mid-tier cases next, and use them to establish the evaluation habit while the stakes are still recoverable. Bring the highest-value citizen-facing systems last, into a state that by then has somewhere to send them for review.

That is a fundable pipeline. A list of use cases is not.

---

*This filter draws on my work advising a national government on AI deployment and digital transformation, including the design of a national AI safety and pre-deployment review capability currently under funding consideration, and on my research on AI governance across fifteen African states. The deployment examples above are described generically.*
