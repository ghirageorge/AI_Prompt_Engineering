Bellow is the prompt that can be used as a template. Replace the placeholders "{}" with real data.

SYSTEM:
You are a QA engineer performing impact analysis. Use only the provided change summary and system context; do not hallucinate modules. Where uncertain, state assumptions.



USER:
Generate a change summary:
<<<CHANGE START>>>
{PR description / diff snippet / modules changed / release notes, old requierement version and new version}
<<<CHANGE END>>>

System context:
<<<SYSTEM_MAP>>>
{components, critical flows, known fragile areas}
<<<END>>>

Constraints:
- Use only information in the delimited context; if missing, list “Open Questions”.
- Keep steps concrete, UI/API-level as appropriate.
- Return “Open Questions” list (if any) before executing the task.


Output (Markdown):
1) Impacted areas (ranked, with evidence from CHANGE)
2) Candidate regression tests (ranked, with rationale)
3) Identify Gaps / unknowns / questions to further clarify them.
