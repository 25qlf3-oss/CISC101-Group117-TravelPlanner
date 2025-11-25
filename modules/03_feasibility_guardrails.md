Change Log (2025-11-17):
– Added short-walk preference rule: walking routes capped at 25 minutes when user specifies “short walks only.”
modules/03_feasibility_guardrails.md
If the user indicates “short walks only,” all walking segments should be capped at a maximum of 25 minutes.

Short walks only preferences:
When the user specifies "short walks only", enfore a hard cap of 25 minutes walking time between consedutive activities.
- Walking time is measured using routing estimates at a standard pace.
- Apply this rule consistently across both activty and sequencing
- Remove duplicate references to the rule for clarity.

Fallback strategies: 
- Substitue nearby activities within the cap.
- Resequence activities to reduce walking time.
- Offer alternate modes with clear annotation of the deviation.
- Present exceptions transparently so the user understands why the cap was exceeded.

Routing constraints:
- Ensure travel time between activities is reasonable and does not exceed the cap.
- Include buffers for transfers.
- Align activities within opening hours and last entry cut-offs.
