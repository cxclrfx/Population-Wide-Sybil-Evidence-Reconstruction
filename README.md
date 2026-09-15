# From Funding to Integrity
## A Population-Wide Reconstruction of Sybil-Resistance Signals

**9,991 donors. 529,016 admitted events. 340,631 evidence relationships. 4,279 wallets surfaced for review.**

This case study reconstructs wallet-level evidence across an entire funding participant population. Complete acquisition coverage of **9,991 out of 9,991 donors** supports a frozen result containing **8,387 accepted evidence edges**, **471 reconstructed clusters**, and **2,684 cluster members**. The reconstruction shows wallet-level evidence structure that is absent from aggregate public matching outputs: relationships between participants, the evidence families associated with those relationships, and the resulting review population.

The release presents a verified aggregate account of that work. Acquisition, event admission, relationship counts, cluster membership, and integrity checks are reported separately so that each number has a clear meaning. The result combines population-wide coverage with an explicit record of what entered the analysis and what was excluded. Its central contribution is a structured view of participant relationships, expressed through frozen, cross-checked results.

## Results at a glance

| Measure | Frozen result |
| --- | ---: |
| Donors in the population | 9,991 |
| Acquisition complete | 9,991 / 9,991 |
| Partial, failed, or unqueried donors | 0 / 0 / 0 |
| Observed source events | 529,017 |
| Events admitted to analysis | 529,016 |
| Evidence relationships | 340,631 |
| Accepted evidence edges | 8,387 |
| Informational edges | 332,244 |
| Reconstructed clusters | 471 |
| Cluster members | 2,684 |
| Wallets surfaced for review | 4,279 |

The relationship totals reconcile exactly: **8,387 accepted edges + 332,244 informational edges = 340,631 evidence relationships**. The observed and admitted event totals differ by exactly one event, whose exclusion is documented below. Acquisition status also reconciles to the full donor population, with no partial, failed, or unqueried participants in the frozen completion record.

Machine-readable figures are provided in [RESULTS.json](RESULTS.json). Coverage and observation dates are documented in [PROVENANCE.md](PROVENANCE.md), and verification counts are recorded in [INTEGRITY.json](INTEGRITY.json).

## What the reconstruction adds

Public matching outputs provide an aggregate view of funding outcomes. A participant-level reconstruction adds a different unit of analysis: the relationships visible among wallets within a defined observation window. This makes it possible to describe the structure behind a review population, including the volume of recorded relationships, the accepted subset, and the groups reconstructed from the evidence.

The frozen result organizes these findings at three distinct levels. Evidence relationships describe connections recorded by the analysis. Reconstructed clusters summarize group structure. Wallets surfaced for review identify the donor-level population associated with accepted evidence. Keeping these levels separate makes the result interpretable without treating a relationship count as a count of people or a group count as a count of incidents.

The distinction is visible in the headline figures. The reconstruction contains 471 clusters and 2,684 cluster members, alongside 4,279 wallets surfaced for review. These totals answer different questions: how many groups were reconstructed, how many wallets appear as cluster members, and how many donor wallets enter the review population. They are presented independently rather than combined into a single headline number.

This gives the case study a concrete contribution to funding-integrity review. It moves from a participant list and observed activity to an organized account of relationships and group structure, while preserving the denominator of the full population. The published aggregates make the scale of that contribution inspectable and provide a stable reference for discussing the frozen result.

## Full-population coverage

Every one of the 9,991 donors was included in acquisition coverage and in the analysis population. The completed acquisition record contains 9,991 complete participants, zero partial participants, zero failed participants, and zero participants left unqueried. All 9,991 donors had locally available observed events in the frozen record.

This coverage matters because the meaning of a result depends on its denominator. A result derived from an initial shortlist describes that shortlist; the result here describes the full donor population within the documented source and observation scope. Earlier shortlist nominations did not determine which donors entered the analysis. Population membership was preserved across acquisition and analytical inclusion.

The observation window spans **March 3, 2025, at 12:00:00 UTC through April 23, 2025, at 23:59:00 UTC**. Reporting one defined window alongside the population and completion counts anchors the analysis to a specific body of observations. It also makes clear which period the frozen relationship structure describes. The source context and the precise UTC timestamps are recorded in the provenance document.

## From observed events to admitted evidence

The source acquisition recorded 529,017 observed events. Of these, 529,016 were admitted to analysis. One source ERC-20 event lacked token decimals and was excluded from analytical admission. The missing value was not guessed.

That single-event difference is retained explicitly in the aggregate results. Observed events and admitted events are separate quantities, and their reconciliation is part of the account of the analysis. A reader can therefore trace the transition from source volume to analytical volume without assuming that every observation was suitable for use.

The admitted events support 340,631 evidence relationships. Within that total, 8,387 edges are recorded as accepted evidence and 332,244 as informational. This distinction preserves the recorded status of the relationships and explains how the headline total is composed. The accepted subset provides the basis for identifying donor wallets surfaced for review.

The analysis input excluded Passport scores, known Sybil labels, and external wallet classifications. The reported reconstruction therefore describes the evidence structure produced from the admitted observations without those classifications as analytical inputs. That input boundary is part of the provenance of the result and helps readers understand what information the analysis used.

## Evidence families

The frozen output records the following evidence-family occurrences associated with accepted edges:

| Evidence family | Recorded occurrences |
| --- | ---: |
| Temporal | 23,114 |
| Amount | 7,777 |
| Funding | 6,097 |
| Sink | 5,089 |
| Route behavior | 1,313 |

These figures provide an aggregate view of the kinds of evidence represented in the accepted relationships. Temporal occurrences form the largest recorded family, followed by amount, funding, sink, and route behavior. The table preserves the recorded family totals without collapsing them into a synthetic measure of certainty.

The unit here is an occurrence, distinct from an edge or a wallet. Multiple occurrences can be associated with the same relationship, and evidence families can overlap. The table therefore complements the relationship and participant counts: it describes the composition of recorded evidence while the other totals describe the scale and structure of the reconstruction.

Read together, these views show both breadth and organization. The population count establishes scope, admitted events establish analytical volume, relationships establish connectivity, and family occurrences describe the recorded evidence composition. Clusters and review wallets then summarize two different aspects of the resulting participant-level structure.

## Execution and integrity

Recorded analysis runtime was **292.453 seconds**. Recorded acquisition runtime was **13,227.844 seconds**. These are the durations reported for the frozen work, shown separately because acquiring observations and analyzing admitted events are distinct activities. They accompany the result as execution measurements for this case study.

The frozen final integrity verification records **PASS**, covering **108,203 acquisition files** and **229 run files**. A separate recorded check covered **229 tracked canonical production files**, with **zero changed files**. These figures state the exact extent of the reported file checks, and the integrity document keeps their roles distinct.

This release also includes [SHA256SUMS](SHA256SUMS), containing a SHA-256 checksum for each of the other five files. Those checksums allow the released documents to be checked for byte-level consistency after download or transfer. The repository thus provides both the aggregate outcome of the frozen source verification and a direct integrity check for the material distributed here.

For release verification, calculate the SHA-256 digest of each listed file and compare it with its entry in SHA256SUMS. Preserve the files as downloaded when doing so: changing line endings, formatting, or text changes their bytes and therefore their digests. The checksum list covers the complete five-document package accompanying it.

## Corpus provenance

The frozen public corpus covers three **Gitcoin Open Source quadratic funding rounds on Arbitrum**, with **chain ID 42161** and **round IDs 863, 865, and 867**. Their combined donor population supplies the 9,991 participants used throughout this case study. The associated observation acquisition used Blockscout within the stated UTC window.

The corpus context, observation window, acquisition completion, and analytical input exclusions are consolidated in [PROVENANCE.md](PROVENANCE.md). Together they define the scope against which the aggregate results should be read. Acquisition completeness refers to the documented provider responses and observation scope for that population.

## Claim boundaries

Wallets surfaced for review are not confirmed Sybils; clusters do not establish one controller; low or absent accepted evidence does not clear a wallet. Family occurrences overlap and are not independent proofs. Provider-window completeness is not independent verification of the entire chain. Excluding external classifications from analytical input does not establish strict experimental blindness. No ground-truth performance comparison or superiority over Passport or matching mechanisms is claimed. Integrity checks establish byte consistency, not the truth of classifications. See [CLAIM_BOUNDARIES.md](CLAIM_BOUNDARIES.md).

## Release contents

| File | Purpose |
| --- | --- |
| [README.md](README.md) | Case study, results, and interpretation |
| [RESULTS.json](RESULTS.json) | Aggregate metrics and recorded durations |
| [INTEGRITY.json](INTEGRITY.json) | Frozen verification statuses and counts |
| [PROVENANCE.md](PROVENANCE.md) | Corpus, window, and acquisition scope |
| [CLAIM_BOUNDARIES.md](CLAIM_BOUNDARIES.md) | Compact limits on inference |
| [SHA256SUMS](SHA256SUMS) | SHA-256 checksums for the five documents |

The release is a fixed aggregate case study. Its six files provide a concise record of population coverage, analytical volume, reconstructed relationships, and integrity verification. The contribution is a population-wide evidence structure that can support focused review of funding integrity, with explicit units, reconciled totals, and a documented observation scope.
