# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on the fact that 46% of started journeys end in an agreement, 31% of starters contact an agent within 7 days, 28% of uploaded income documents need clarification, 19% of new agreements miss a payment within 60 days)
and early qualitative themes (consumers don't know what is affordable, don't understand why information is requested, and fear the consequences of a wrong answer or a missed payment), 
I believe that replacing the single monthly-amount commitment with a guided journey 
(income as a range, plain-language reasons for each question, a recommended affordable plan, and clear missed-payment consequences and support options) 
for time-poor consumers with variable income and one or more open claims in the German pilot segment, 
will result in more instalment plans that people can actually keep, set up without an agent, as measured by a 20% relative reduction (19% to about 15%) 
in the 60-day missed-payment rate of new agreements. I will protect expected recovery value per started journey (it must not fall against the control group), 
along with the complaint rate and the vulnerable-consumer escalation path, and will make a go/no-go decision after 12 weeks from pilot launch 
(4 weeks of enrolment plus a 60-day observation window).
- **From M3, your primary success metric & guardrail metric:** The 60-day rate is the check that SSR reflects better outcomes. Percentage of repayment plans that miss a payment within 60 days. This rate must not increase above the current baseline of 19%.
- **From M4, the feature you scoped in your PRD this is what you're testing:** What if I miss an instalment.

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** What if I miss an instalment.
- **Persona pull your M2 persona:** A consumer with limited time and an uncertain income who is trying to deal with a debt online.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** more instalment plans that people can actually keep
- **Primary success metric the one number that defines success, from M3:** 20% relative reduction (19% to about 15%) 
in the 60-day missed-payment rate of new agreements
- **Baseline rate today's rate of your primary metric, from your M3 data:** 19%
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Percentage of repayment plans that miss a payment within 60 days. This rate must not increase above the current baseline of 19%.
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** _(not filled in)_
- **Sample size per arm use the calculator in the builder, baseline + MDE:** _(not filled in)_
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** _(not filled in)_
- **Significance threshold p < 0.05 is standard, explain any deviation:** _(not filled in)_

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** They are asked to commit to a monthly amount they cannot predict, and they fear that one wrong answer or one missed payment will make everything due at once. 46% of started journeys end in an agreement, 31% of starters contact an agent within 7 days, 28% of uploaded income documents need clarification, 19% of new agreements miss a payment within 60 days.
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** A direct answer to the core fear, in plain language.
The first line states what happens if they miss one instalment, including whether the full balance becomes due.
It uses short, non-legal wording, ideally under about 50 words.
Why: this is the fear that causes under-reporting and abandonment.
Verified copy.
Policy, Legal and Compliance confirm that every claim is accurate for each creditor and market in scope.
Where the answer differs, the block shows the right version or the feature launches only where one answer is true.
Why: a wrong reassurance is worse than none, and it can produce a failed plan at day 60.
Placement at the commitment point.
The block sits beside the amount choice and is visible by default, with no click-through and no modal.
It also appears on the summary step before the person confirms.
Why: the fear peaks when they choose the amount, so help placed elsewhere misses the moment.
One honest next step if they can't pay.
A single line points to the route that exists today, such as contacting support.
It does not promise adjustment, since that is still in NEXT.
Why: reassurance with no way out leaves them calling anyway.
- **Isolation check, what has NOT changed? list everything identical between arms (app version, recommendation engine, notifications, onboarding). If something changed inadvertently, your test is compromised.:** _(not filled in)_

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that a plain-language explanation on missed-payment consequences for consumers who don't know what is affordable will result in more instalment plans that people can actually keep,
as measured by a 20% change in the 60-day missed-payment rate of new agreements within 12 weeks.
We will protect expected recovery value per started journey (it must not fall against the control group) throughout the test.
- **Your shipping criteria (filled in):** _(not filled in)_
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** _(not filled in)_
