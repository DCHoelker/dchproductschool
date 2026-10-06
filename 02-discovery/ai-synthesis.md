# AI Synthesis, Product Health & Insights Summary (Module 2)

## Responses
- **Moment of misery / red flag #1 (e.g., “user gave up after 3 tries”):** User does not understand the process and what to deliver.
- **Moment of misery / red flag #2:** Users do not want to hand in private data.
- **Moment of misery / red flag #3:** Agents are confronted with incomplete instalments
- **Product Health & Insights Summary (Claude's output):** # Product Health & Insights Summary
**Debt repayment portal (consumer journey and agent handoff)**

*Data note: the inputs are synthetic quotes (10 consumer, 8 agent) and contain no bug reports or telemetry. Severities below are analytical judgments from the quotes, not measured impact.*

## Executive Summary
The portal appears to function technically, since consumers reach it, complete steps, and generate cases, but the quotes suggest it often fails to give people the confidence or clarity to finish. Consumers abandon or under-report out of fear, confusion, or a lack of reassurance rather than a lack of usability, and agents inherit cases with too little context to continue the journey. The central tension is that digital completion is likely being counted as success while repeated contact, failed plans, and distrust of system outputs suggest the underlying outcomes are weaker.

## Thematic Synthesis

### 1. Orientation & Entry Experience
Consumers arrive with a single, time-boxed question ("can I pay in pieces?") and meet dense case information instead. Multi-claim customers struggle most, unsure how claims relate or whether paying one affects the other.

- Answer to the core question is not immediately visible on entry: **High**
- Multi-claim structure and interdependence unclear: **High**
- Start date cannot accommodate payday timing, causing exit despite full comprehension: **Medium**

### 2. Affordability Assessment & Defaults
People with variable income have no clear way to express what they can afford and fear a single answer binds them indefinitely. Pre-set slider values appear to act as anchors, with users treating them as a social norm or an endorsed choice rather than an arbitrary default.

- Variable income poorly accommodated, with unclear "best month vs. worst month" framing: **High**
- Default values anchor plan size without explanation: **High**
- Perceived permanence of the commitment: **Medium**

### 3. Data Requests, Trust & Accessibility
Consumers do not understand why income is requested, who sees it, or whether it affects credit. Separately, document requirements exclude those paid in cash, pushing them to phone support. The two issues look similar in drop-off but have different causes: one is transparency, the other is access.

- No explanation of purpose, sharing, or credit impact for income data: **High**
- Payslip requirement blocks cash-paid users with no alternative evidence path: **High**
- Fear of giving a "wrong" answer leads to deliberate under-reporting, which degrades data quality: **High**

### 4. Fear of Consequences & Need for Reassurance
Avoidance is driven substantially by anxiety about what happens after a missed payment, with some users declining to start at all. Calls to the contact centre are often motivated by a wish for reassurance rather than missing information, which a content-focused journey is not designed to address.

- Consequences of a missed payment unclear or feared to be total acceleration: **Critical**
- Reassurance need unmet, so users default to calling: **Medium**

### 5. Agent Context & Handoff
This is the most concrete and consistent operational gap. Agents often see an empty or near-empty case when a customer says they already completed steps online, and they cannot see what the customer entered or what the system presented. The result is repeated data collection and customer frustration.

- Digital journey activity not visible to agents (inputs, offers shown): **Critical**
- Recommendations lack visible rationale, so agents will not relay them: **High**
- Agents cannot tell whether an offer was a true recommendation or a default: **High**

### 6. Data Quality & Correction Mechanisms
Acquired portfolios carry outdated addresses and balances, and any stale figure shown in the journey surfaces as customer anger that agents must resolve. When the system wrongly declines an eligible customer, there is no fast, logged correction path, so agents rely on workarounds.

- Stale or inaccurate portfolio data exposed to customers: **High**
- No fast, auditable override for incorrect eligibility outcomes: **High**

### 7. Plan Sustainability & Vulnerability Handling
Agents attribute many failed agreements to customers who committed under stress and without full consideration, not to avoidance. Signals of vulnerability (illness, job loss, bereavement) are audible by phone but invisible to a form, and a quick route to a human is seen as necessary.

- Plans accepted without realistic affordability reflection, then failing and returning escalated: **High**
- No quick path from the digital journey to a person for vulnerable customers: **High**

### 8. Metric Integrity
The quotes describe a risk that self-service success is measured by plan sign-ups rather than plan survival. If SSR rises while 60-day missed payments exceed the 19% baseline, the metric would be capturing enrolment, not resolution.

- Success measure may reward silent over-commitment over durable outcomes: **High**

### Minor Technical Debt
Unexplained default framing on secondary controls, limited start-date flexibility messaging, and lack of in-journey signposting to support channels.
- **Did the AI catch the specific moment of misery / pain point you found in Step 1?:** Yes. The AI identified the critical decision point. Consumers lack the confidence to commit because they don't understand affordability, data requests, or the consequences of their decision.
- **Did it smooth over a critical frustration into a generic bullet point?:** Yes, it derived from the emotional input the generic problem.
- **Did the AI try to suggest features or a roadmap despite the constraints?:** There were no suggestions, as prompted.
- **Logic leak / hallucination #1 (e.g., “AI suggested a new search bar feature, roadmap leak”):** "Unexplained default framing on secondary controls" and "lack of in-journey signposting to support channels" are not in the quotes.
- **Logic leak / hallucination #2:** 8. Metric Integrity

The quotes contain no mention of "SSR," a 19% baseline, or a 60-day window. The only basis is A8, which says roughly: "I'd rather take a good call than have someone silently sign up to a plan that fails in six weeks." That is a qualitative statement from one agent, not a metric. Also, six weeks is not the same as 60 days.
