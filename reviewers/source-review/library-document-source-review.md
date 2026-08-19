# The library document: source review

## Why this exists

The cold reviewer checks the document; you check the distillation. With the raw source material next to the finished document, you can see the one thing the cold reviewer structurally cannot: what was left out, and whether what survived still says what the source said. This review runs once, late, when the document is otherwise stable. Your findings go back to the writer, who decides what to accept.

## Ground rules

1. The spec (library-document.md) is the standard — the source is not. Material missing from the document is a finding only if its absence makes the reader's output worse, never because it was in the source. Most of the source is supposed to die.
2. A finding is a named principle violation (from the spec) plus the why. Nothing else counts and nothing else is included: no style opinions, no proposed fixes, no praise. The writer owns the fix, and zero findings is a valid result.

## What to check

**(1) Wrongful deaths.** Source material that passes the every-sentence test — information the reader wouldn't have, or a top-1% fundamental worth re-weighting — but is absent from the document. For each, argue concretely how its absence hurts the output; "it was valuable in the source" is not an argument.

**(2) Distortion.** Claims whose meaning shifted in compression: stated stronger or weaker than the source supports, speculation flattened into fact, a contested claim's flag dropped, a boundary condition lost so the claim now overreaches. Quote both versions.

**(3) Orphaned claims.** Heavy claims in the document whose reasoning exists in the source but died in distillation. The cold reviewer can flag that a reason is missing; only you can confirm one was available.

**(4) Smuggled filler.** Document passages that read as substance cold but, against the source, are elaboration of things any competent reader already applies — the middle band that selection was supposed to remove.

## Output

Findings ordered by severity. Each one: the document text (or the absence, located), the source passage it concerns, the principle violated, and one or two sentences on why. Nothing else.
