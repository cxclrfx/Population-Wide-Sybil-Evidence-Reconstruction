# Corpus provenance

The frozen public corpus covers three Gitcoin Open Source quadratic funding rounds on Arbitrum: chain ID **42161**, round IDs **863, 865, and 867**. The combined donor population contains **9,991 donors**.

## Observation window

- Start: **2025-03-03T12:00:00Z**.
- End: **2025-04-23T23:59:00Z**.
- Observation provider: **Blockscout**.

These timestamps describe the acquisition observation window, not the funding rounds' opening and closing times.

## Acquisition and admission

| Measure | Count |
| --- | ---: |
| Donors | 9,991 |
| Complete | 9,991 |
| Partial | 0 |
| Failed | 0 |
| Not queried | 0 |
| Observed source events | 529,017 |
| Admitted events | 529,016 |
| Excluded events with unavailable token decimals | 1 |

Completeness is defined against the documented provider responses for the specified population and window. It is not an independent reconstruction of all chain activity.

One source ERC-20 event lacked token decimals and was excluded from analytical admission rather than assigned a guessed value.

## Analytical input scope

All 9,991 donors were included in the analytical population. Earlier shortlist nominations were neither the analytical core nor a population filter. The input excluded Passport scores, known Sybil labels, and external wallet classifications. This describes input composition; it does not establish strict experimental blindness.

The aggregate outcomes are in [RESULTS.json](RESULTS.json). Recorded verification counts are in [INTEGRITY.json](INTEGRITY.json), and inference limits are in [CLAIM_BOUNDARIES.md](CLAIM_BOUNDARIES.md).
