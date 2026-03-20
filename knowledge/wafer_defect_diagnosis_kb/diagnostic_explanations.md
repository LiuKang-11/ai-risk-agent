# Diagnostic Explanations

## Explanation template
- predicted class
- confidence
- feature evidence
- contextual evidence
- likely causes
- why alternatives were deprioritized
- what evidence would strengthen or weaken the conclusion

## Example 1
Predicted class: `Scratch`
Reasoning: strong scratch-line score, repeated alignment with handling path, recent robot alarm history, and limited evidence for contamination.
Likely causes: end-effector contact, cassette damage, or wafer transfer misalignment.

## Example 2
Predicted class: `Donut`
Reasoning: ring score is high, center remains relatively clean, and similar issues recurred on the same chamber after maintenance.
Likely causes: radial process non-uniformity, chamber seasoning drift, or gas flow imbalance.

## Example 3
Predicted class: `Random`
Reasoning: no dominant geometry, high randomness score, spread across wafers and lots, plus contamination indicators.
Likely causes: contamination source, broad particle generation, or unstable upstream process.

## Explainability rules
- cite feature evidence before causal interpretation
- tie the cause ranking to process step and recent history
- explicitly note uncertainty when confidence is moderate or mixed
