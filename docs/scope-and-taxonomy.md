# Scope and taxonomy

**Reconciliation note (2026-10-15):** This document originally described the narrower 51-record review. The master corpus now retains 127 records, including all 104 previous records. See [the reconciliation](reconciliation.md); absence from a focused view is not deletion from the corpus.

## The source taxonomy

The source is [SARAF arXiv v1, Section 2.2](https://arxiv.org/html/2606.04135v1#S2.SS2), dated June 2, 2026. This review did not use the final publisher version to audit the taxonomy.

Its two headings are:

1. **Retrieval as Input Augmentation**: retrieved examples accompany the query before or during prediction.
2. **Retrieval as Post-hoc Refinement**: a retrieval branch corrects or ensembles an existing prediction.

The source paragraph names TimeRAG, RAFT, RAF, TRACE and TS-RAG under the first heading, and PFRP and PIR under the second. The RAF citations refer to two different papers, by Tire et al. and Li.

The catalogue preserves these headings. Placement of additional papers is an editorial mapping based on their own methods. It does not attribute later papers or new boundary interpretations to SARAF.

## A bibliographic inconsistency to preserve transparently

In [Section 2.2's input-augmentation paragraph](https://arxiv.org/html/2606.04135v1#S2.SS2.p2), the short source excerpt is “TimeRAG (Zhang et al., 2025)”. The paragraph describes clustering and DTW-based retrieval for LLM forecasting. The linked [bibliography entry](https://arxiv.org/html/2606.04135v1#bib.bib19) is Zhang et al.'s **TimeRAF**, arXiv:2412.20810.

The independently identified papers are:

- [TimeRAG by Yang et al.](https://arxiv.org/abs/2412.16643): DTW-based retrieval for LLM forecasting; ICASSP 2025.
- [TimeRAF by Zhang et al.](https://arxiv.org/abs/2412.20810): retrieval-augmented foundation-model forecasting; IEEE TKDE 2025.

The name and linked bibliography differ in the checked version. This does not establish which paper the authors intended to cite, and no claim is made about the final publisher version. Both papers are kept independently in the catalogue.

## Interpretation rules for this catalogue

- **Integration stage is primary.** Decide whether retrieved information changes model inputs/representations or changes an already formed forecast.
- **Retrieval objective is not integration stage.** A memory storing residuals does not automatically mean output correction if those residuals steer hidden states before decoding.
- **Training protocol is a separate axis.** Jointly trained output fusion is not synonymous with a frozen, training-free postprocessor.
- **Hybrid methods are not forced into a binary assignment.** When a defensible primary path exists, secondary pathways are noted; otherwise a separate hybrid view is used, as for GNA. Each paper is counted once.
- **A title containing retrieval is insufficient.** Check whether the system accesses historical examples, external contextual knowledge or an explicit memory at inference.

## Important boundary cases

### Input and representation augmentation

- [SteerCast](https://arxiv.org/html/2610.11229v1#S3) injects retrieved latent steering vectors during autoregressive decoding. It fits the broad representation-augmentation branch, not literal input concatenation. It does not wait for a complete base forecast and then correct the output.
- [TIMBRE](https://arxiv.org/html/2610.04795v1) updates hidden representations before the frozen prediction head.
- [SEER](https://arxiv.org/html/2610.04109v1#S3.SS2) retrieves event information, knowledge and reflective memory into the forecasting prompt. The retrieved objects need not be numeric neighbors.
- [MemCast](https://arxiv.org/abs/2602.03164) retrieves experience-conditioned reasoning into the forecasting process.
- [Align-RAG](https://arxiv.org/html/2608.05571v1) is primarily in-context input augmentation, but also includes output blending. Its primary classification does not erase that hybrid design.
- [Time-VLM](https://arxiv.org/abs/2502.04395v2) is classified using v2, whose history buffer and cosine retrieval differ materially from v1's current-input attention description.

### Output refinement and fusion

- [SARAF](https://arxiv.org/html/2606.04135v1#S3.SS5) and [SERAF](https://arxiv.org/abs/2606.14941) combine a retrieved-future prediction with a backbone prediction and learned fusion/projection. Their placement here is editorial, not an author self-classification or a claim of training-free operation.
- [SpecReTF](https://arxiv.org/abs/2606.19412) combines retrieval and base predictions with learned fusion; the broad output-fusion interpretation should remain explicit.
- [DuoTS](https://arxiv.org/html/2610.03491v1) adds a gated analog-derived correction to a base prediction. Its retrieval is inside the current lookback window and the model is jointly trained. It is not an external global-memory or frozen postprocessing method.
- [STRATA-TS](https://arxiv.org/html/2508.18635v2) uses retrieved context in an LLM, but that LLM refines an upstream spatiotemporal forecaster's prediction tokens. The primary mapping is relative to that base forecaster, with an input-conditioning secondary pathway.

### Related research outside the main split

- **Training-only retrieval:** TS-Memory and SRRF. Their deployed predictors do not retrieve examples at inference.
- **Standalone nonparametric prediction:** KReF. It does not augment a separate forecasting backbone.
- **Same-input semantic attention:** TimeMRA. Attention over semantic representations produced from the current input is not the same mechanism as retrieving historical examples from an external bank.
- **Evaluation and retriever learning:** *When Does Retrieval Help Time-Series Forecasting?*, *Which Histories Matter...*, and *Retrieval Mechanisms Surpass Long-Context Scaling...* are not counted as three new fusion architectures.
- **Broader output domains:** RAP covers spatiotemporal fields, and ReDiTT covers asynchronous events. They are relevant extensions rather than silently treated as identical benchmark settings.

## Versions and acronym collisions

- RAF (Tire et al., arXiv:2411.08249) and RAFT (Han et al., arXiv:2505.04163) share the title *Retrieval Augmented Time Series Forecasting* but are distinct papers. RAF (Li, tabular forecasting) is a third work.
- TimeRAG (Yang) and TimeRAF (Zhang) are different. A further anonymous OpenReview TimeRAG manuscript has an unresolved relationship to FinSeer and is not counted independently yet.
- TS-RAG (Ning et al., 2025) and TS-RAG (Xiao et al., 2026) are different papers.
- RIDDE / *Factorize to Generalize* and ROAR share arXiv:2605.24911, so are represented by one version-family record.
- FinSeer / FinSrag titles under arXiv:2502.05878 are one version family.
- TRACE here means the multimodal embedding-and-retrieval paper, not other unrelated uses of the acronym.

## Year and venue conventions

First public year, arXiv submission date, acceptance year and journal issue year are different fields. For example, Tire's RAF began as a 2024 preprint and has an AISTATS 2026 proceedings record; PFRP began in 2025 and is published at AAAI 2026. kNN-MTS is listed under 2024 in the [authors’ McGill IALab bibliography](https://mcgillialab.com/publications/), while its final issue is July 2025 and its arXiv v1 posting is May 16, 2025. Its exact first-public day was not primary-verified on final recheck, so it is placed at the end of the 2024 group rather than given an assumed day.

The Resolution-Aware paper has a 2024 workshop precursor beginning with *Towards* and an expanded 2025 arXiv version. The README displays the workshop title in the 2024 row, while the record links and explains the expanded version. Unknown first posting days are not fabricated from conference dates, DOI years or arXiv identifier prefixes.
