# Responsible Intelligence Research Framework

This document describes a repeatable approach for lawful open-source and cyber intelligence research. Adapt the steps to the question, the source types, and the applicable rules.

## 1. Define the question

- State the research question and intended use.
- Define scope, time window, and what is out of scope.
- Identify whether the work requires explicit authorization.
- Decide what evidence would support, weaken, or leave the question unresolved.

## 2. Plan sources

- Prefer primary and authoritative sources where possible.
- Record source URLs, access dates, and relevant publication or observation dates.
- Distinguish first-hand sources from commentary, reposts, and derived datasets.
- Respect terms of service, access controls, privacy, and applicable law.

## 3. Collect minimally

- Collect only information relevant to the defined question.
- Avoid bypassing authentication, access controls, rate limits, or technical restrictions.
- Do not target private individuals or sensitive personal information without a lawful, justified basis.
- Keep raw observations separate from transformed or enriched data.

## 4. Normalize and preserve provenance

For each observation, capture useful metadata such as:

| Field | Meaning |
|---|---|
| Source | Where the observation originated |
| Observed at | When it was collected |
| Published at | When the source says it was published, if known |
| Extract | The relevant observation, not an unsupported conclusion |
| Transformation | Any parsing, normalization, or enrichment applied |
| Confidence | A reasoned assessment, with limitations |

Do not silently overwrite source observations. Preserve enough provenance to reproduce the analysis.

## 5. Correlate carefully

- Use stable identifiers where available.
- Treat name, address, or visual similarity as a lead, not proof of identity.
- Seek independent corroboration for consequential claims.
- Track contradictory observations and alternative explanations.
- Avoid turning correlation into a claim of causation.

## 6. Use distributed or swarm workflows responsibly

When multiple agents or workers are used:

- Give each worker a bounded task and permitted source scope.
- Share only the context required to complete that task.
- Log task inputs, outputs, timestamps, and tool actions.
- Deduplicate and validate results centrally.
- Require human review before consequential conclusions or external actions.
- Include stop conditions and limits on collection volume.

## 7. Analyze and communicate

Separate the final output into:

1. **Observations** — what the sources directly show.
2. **Assessment** — what those observations may mean.
3. **Confidence** — how strongly the evidence supports the assessment.
4. **Limitations** — gaps, ambiguity, freshness, and source reliability.
5. **Next steps** — proportionate ways to resolve remaining uncertainty.

## 8. Close out

- Retain only what is necessary for the stated purpose.
- Remove unnecessary personal or sensitive information.
- Record the research end date and any important limitations.
- Revisit findings when sources change or become outdated.

---

**Guiding rule:** Publicly accessible does not automatically mean unrestricted, accurate, or appropriate to collect. Keep research lawful, ethical, proportionate, and within authorization.
