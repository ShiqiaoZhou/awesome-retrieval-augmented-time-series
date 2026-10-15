# Original focused-review verification

This document preserves evidence for the original 51 focused-review records. For restored records, see [recovery verification](recovery-verification.md). For canonical stable IDs, use the [crosswalk](../data/reconciliation-crosswalk.csv); the arXiv-based IDs below remain aliases.

Checked on 2026-10-15. This file records the evidence supporting the catalogue; it is not a comparative performance ranking. Detailed date and version caveats are retained rather than guessed.

## SteerCast: Retrieval-Based Latent Steering for Decoder-Only Time Series Forecasting

- Record: `arxiv-2610.11229`
- Role: core
- Known public year: 2026; earliest verified date: 2026-10-08
- Date qualification: arXiv v1 submission date, 2026-10-08 04:30:54 UTC; earlier public venue posting date not established
- Venue: NeurIPS 2026 (accepted poster)
- Venue evidence: https://neurips.cc/virtual/2026/poster/154457
- Paper: https://arxiv.org/abs/2610.11229
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Sections 3.1–3.3: offline memory pairs history embeddings with latent displacements between ground-truth and model-predicted continuations. At test time top-k histories supply averaged steering vectors, injected into hidden states at each autoregressive generation step. Thus residual-based memory does not by itself make this output-space post-hoc refinement.
- Method source: https://arxiv.org/html/2610.11229v1#S3
- Code link reported by an author/paper: https://github.com/Davido111200/SteerCast (availability and implementation completeness are not implied unless noted below)
- Note: Fits a broad representation/process-augmentation definition, but not literal input concatenation. It does not first finish the query's base forecast and then correct the output. Keep explicitly marked as a latent-steering boundary case under a strict SARAF two-way taxonomy.
- Note: arXiv v1 submission date, 2026-10-08 04:30:54 UTC; earlier public venue posting date not established
- Note: Public code repository verified, including steercast/, finetune/, scripts/, and three backbone entry points

## Retrieval Is Not Enough: Refreshing Memory for Frozen Time-Series Forecasters

- Record: `arxiv-2610.07834`
- Role: core
- Known public year: 2026; earliest verified date: 2026-10-06
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2610.07834
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Maintain and refresh an external memory for frozen forecasters, use retrieved examples for kernel regression, and apply a validation-calibrated closed-form correction weight to the base forecast.
- Method source: https://arxiv.org/html/2610.07834v2
- Note: 当前v2为2026-10-07；搜索和当前正文未找到作者官方代码链接。

## GRAM: Correcting Frozen Time-Series Foundation Models via Graph-Retrieved Amplitude Memory

- Record: `arxiv-2610.04827`
- Role: core
- Known public year: 2026; earliest verified date: 2026-10-04
- Date qualification: arXiv v1 submission date, 2026-10-04 00:20:36 UTC
- Venue: arXiv preprint; no accepted conference/journal venue verified as of 2026-10-15
- Venue evidence: https://arxiv.org/abs/2610.04827
- Paper: https://arxiv.org/abs/2610.04827
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Section 3.1 and Figure 1: a frozen TSFM supplies the base prediction. Offline amplitude-memory prototypes summarize its dimensionless amplitude-scaling errors, with graph edges for bias/shape relations. Online top-K retrieval expands a prototype subgraph; the trainable graph fusion module produces horizon-wise error components added to the frozen forecast. Zero correction exactly recovers the base forecast.
- Method source: https://arxiv.org/html/2610.04827v1#S3.SS1
- Code link reported by an author/paper: https://github.com/ecnuabmlab/GRAM (availability and implementation completeness are not implied unless noted below)
- Note: arXiv v1 submission date, 2026-10-04 00:20:36 UTC
- Note: Public implementation verified; gram/, scripts/, requirements.txt and reproduction instructions visible

## TIMBRE: Teaching Time Series Forecasters to Read, Remember, and Reconcile

- Record: `arxiv-2610.04795`
- Role: core
- Known public year: 2026; earliest verified date: 2026-10-03
- Date qualification: arXiv v1 submission date, 2026-10-03 22:46:20 UTC
- Venue: arXiv preprint; submitted to ICASSP 2027 according to author website, not accepted
- Venue evidence: https://guanxinyu.blog/
- Paper: https://arxiv.org/abs/2610.04795
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Section 3.1 Eq. (1): frozen numerical future states H receive an evidence-driven update ΔH, then the frozen head predicts from H+ΔH. Retrieved historical response curves are state-conditioned by amplitude/time transforms (Section 3.2), and reliability-weighted cross-attention fuses evidence into ΔH (Section 3.3). Retrieval/bank contents stay fixed.
- Method source: https://arxiv.org/html/2610.04795v1#S3
- Code link reported by an author/paper: https://github.com/stephen-guan-researcher/TIMBRE (availability and implementation completeness are not implied unless noted below)
- Note: Representation-level integration before the frozen forecast head. A separate median-preserving interval-width readout is post-head, but that does not make the primary retrieval mechanism post-hoc forecast refinement.
- Note: arXiv v1 submission date, 2026-10-03 22:46:20 UTC
- Note: Public source release verified, including model, training, evaluation and memory code, tests and configs

## SEER: Self-Evolving Event Reasoning and Retrieval for Time Series Forecasting

- Record: `arxiv-2610.04109`
- Role: core
- Known public year: 2026; earliest verified date: 2026-10-02
- Date qualification: arXiv v1 submission date, 2026-10-02 22:30:10 UTC
- Venue: arXiv preprint; no accepted conference/journal venue verified as of 2026-10-15
- Venue evidence: https://arxiv.org/abs/2610.04109
- Paper: https://arxiv.org/abs/2610.04109
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Section 3.2 Eq. (2) computes the forecast as f(x_t, R(events, knowledge, memory)). Retrieved external events, filtering guidance, and distilled domain knowledge construct textual context supplied to a frozen LLM forecaster before prediction. Error-driven reflection updates future retrieval/context; it is not a post-hoc correction of the current output.
- Method source: https://arxiv.org/html/2610.04109v1#S3.SS2
- Code link reported by an author/paper: https://github.com/BennyTMT/SEER (availability and implementation completeness are not implied unless noted below)
- Note: arXiv v1 submission date, 2026-10-02 22:30:10 UTC
- Note: Official public repository verified; visible files are assets/, paper/, .gitignore, CITATION.cff, and README.md. Implementation release was not verified.

## Dual-Context Analog Retrieval for Time Series Forecasting

- Record: `arxiv-2610.03491`
- Role: core
- Known public year: 2026; earliest verified date: 2026-10-02
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2610.03491
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Section 3, Eq. (1): add a gated analog-based correction to a base forecast. The retrieval bank is inside the current lookback window; the retrieved analogs and their observed successors inform the correction. Joint training does not imply a frozen post-processing protocol.
- Method source: https://arxiv.org/html/2610.03491v1
- Code link reported by an author/paper: https://anonymous.4open.science/r/DuoTS-244D (availability and implementation completeness are not implied unless noted below)
- Note: 官方原文§1提供匿名代码链接，尚未单独验证仓库可打开。

## Which Histories Matter for Time Series Forecasting? Learning Predictive Relevance with Future Supervision

- Record: `arxiv-2608.23221`
- Role: related; retrieval_learning_and_evaluation
- Known public year: 2026; earliest verified date: 2026-08-24
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2608.23221
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: Section 3: a pattern-similarity candidate pool is reranked with a residual MLP trained using future compatibility. Inference scoring only observes the past. Section 5.6 separates retrieval ranking quality from forecast aggregation, so a single SARAF fusion class is not inherent.
- Method source: https://arxiv.org/html/2608.23221v1
- Code link reported by an author/paper: https://github.com/dearyonghoon/which-histories-matter/ (availability and implementation completeness are not implied unless noted below)
- Note: SARAF对比为匹配检索规则的protocol，作者明确不是SARAF原生benchmark复现；不要将其当作端到端预测排名直接比较。
- Note: Learns predictive relevance and evaluates ranking; the output-integration architecture is not fixed.

## Model-agnostic Retrieval-Augmented Extended Forecasting for time series

- Record: `arxiv-2608.14054`
- Role: core
- Known public year: 2026; earliest verified date: 2026-08-14
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2608.14054
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Sections 2.2–2.3, Eqs. (2)–(5): retrieve directly in raw input space, concatenate high-similarity past–future examples, average lower-similarity examples, and join them with the query as an extended input to a frozen forecasting model. Retrieval does not post-process its output.
- Method source: https://arxiv.org/html/2608.14054v1
- Code link reported by an author/paper: https://github.com/jpvilla1990/raef/ (availability and implementation completeness are not implied unless noted below)
- Note: arXiv未给正式发表venue；原文§3.1直接链接官方实验代码。

## KReF: Training-Free Retrieval for Long-Term Time-Series Forecasting and Predictive Uncertainty

- Record: `arxiv-2608.06748`
- Role: related; standalone_retrieval_forecaster
- Known public year: 2026; earliest verified date: 2026-08-07
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2608.06748
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: Historical context–continuation neighbors directly produce a nonparametric forecast and predictive uncertainty; no separate pretrained backbone is augmented or corrected.
- Method source: https://arxiv.org/pdf/2608.06748
- Note: PDF标题元数据为AAAI Proceedings Template只是排版模板，不能据此声称AAAI接收。未找到官方代码链接。
- Note: A standalone nonparametric retrieval predictor, without a separate base forecasting model to augment or refine.

## TS-RAG: Retrieval Augmented Generation for Time Series Forecasting

- Record: `arxiv-2608.06223`
- Role: core
- Known public year: 2026; earliest verified date: 2026-08-06
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2608.06223
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Section 3.2, Eq. (5): prepend learned reference tokens to patch inputs and encode retrieved sequences separately. Section 3.3, Eqs. (9)–(10): self/cross-attention fuses representations before prediction. This is a different paper from Ning et al. TS-RAG (2025).
- Method source: https://arxiv.org/html/2608.06223v1
- Note: 不同于Ning等NeurIPS2025的TS-RAG。作者列表有一处原文差异：arXiv摘要元数据为3位作者，HTML正文另外列Shuangli Li；建议显示Yixiong Xiao et al.并保留此注记。未找到作者官方代码链接。

## Align-RAG: Alignment Is All You Need for TSFM In-Context Learning

- Record: `arxiv-2608.05571`
- Role: core
- Known public year: 2026; earliest verified date: 2026-08-06
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2608.05571
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Align retrieved demonstrations to the current context for TSFM in-context learning. The primary route is input augmentation; the full method also blends retrieved futures and a no-demonstration forecast.
- Method source: https://arxiv.org/html/2608.05571v1
- Code link reported by an author/paper: https://github.com/masadi-99/align-rag (availability and implementation completeness are not implied unless noted below)
- Note: 原文和官方仓库链接交叉核验；无已核验正式venue。

## When Does Retrieval Help Time-Series Forecasting?

- Record: `arxiv-2609.20193`
- Role: related; evaluation
- Known public year: 2026; earliest verified date: 2026-07-29
- Date qualification: 按arXiv官方submission history为2026-07-29；编号却是2609.20193，日期与编号月份不一致，原样记录且应提示读者。
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2609.20193
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: The paper varies lookback relative to dominant seasonal period and uses repeat/lookup controls to identify regimes where retrieval helps. Its contribution is evaluation and applicability analysis, not a new plugin.
- Method source: https://arxiv.org/pdf/2609.20193
- Code link reported by an author/paper: https://github.com/KurbanIntelligenceLab/retrieval-regime (availability and implementation completeness are not implied unless noted below)
- Note: 官方代码仓库已打开核验。
- Note: 按arXiv官方submission history为2026-07-29；编号却是2609.20193，日期与编号月份不一致，原样记录且应提示读者。
- Note: Studies when retrieval helps; does not introduce a new retrieval-augmentation architecture.

## ReDiTT: Retrieval Augmented Conditional Diffusion Transformers for Asynchronous Time Series

- Record: `arxiv-2607.12391`
- Role: related; asynchronous_event_prediction
- Known public year: 2026; earliest verified date: 2026-07-14
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: TMLR 2026
- Venue evidence: https://openreview.net/forum?id=sv35KiCipb
- Paper: https://arxiv.org/abs/2607.12391
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: §4: Retrieve top-k latent event-sequence references from training memory using observed prefix, then condition latent flow/diffusion transformer blocks by cross-attention to generate future event times/types.
- Method source: https://arxiv.org/html/2607.12391v1#S4
- Code link reported by an author/paper: https://github.com/BorealisAI/ReDiTT (availability and implementation completeness are not implied unless noted below)
- Note: Accepted TMLR per arXiv and original manuscript, OpenReview identity sv35KiCipb. Scope is marked temporal event forecasting.
- Note: Retrieval-conditioned forecasting of asynchronous event times and event types.

## Semantics-Enhanced Retrieval-Augmented Time Series Forecasting

- Record: `arxiv-2606.14941`
- Role: core
- Known public year: 2026; earliest verified date: 2026-06-12
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: ICML 2026 Workshop on Forecasting as a New Frontier of Intelligence (AI Forecasting Workshop)
- Venue evidence: https://research.birmingham.ac.uk/en/publications/semantics-enhanced-retrieval-augmented-time-series-forecasting/
- Paper: https://arxiv.org/abs/2606.14941
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Sections 2.3–2.6: parallel retrieval compares numeric histories and template-generated textual descriptions of the same histories. Gaussian-weighted retrieved futures from both branches are fused, gated against a linear encoder forecast, and passed through a learned projection. No external text corpus is required.
- Method source: https://arxiv.org/html/2606.14941#S2
- Note: Curator mapping to the broad output-fusion/refinement branch, with multimodal/semantic retrieval tags. This is not an original SARAF §2.2 seed and not a training-free post-hoc module.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## Stationarity-Aware Retrieval-Augmented Time Series Forecasting

- Record: `arxiv-2606.04135`
- Role: core
- Known public year: 2026; earliest verified date: 2026-06-02
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: KDD 2026, Research Track; proceedings V.2, pp. 6875–6886
- Venue evidence: https://doi.org/10.1145/3770855.3817813
- Paper: https://arxiv.org/abs/2606.04135
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Sections 3.4–3.5: time-aligned Pearson retrieval creates candidates; stationarity controls diversity-aware selection and Gaussian weighting of retrieved futures. The resulting retrieval forecast is fused with a backbone prediction through a learned output projection.
- Method source: https://arxiv.org/html/2606.04135#S3
- Code link reported by an author/paper: https://github.com/ShiqiaoZhou/SARAF (availability and implementation completeness are not implied unless noted below)
- Note: Curator mapping to the broad output-fusion/refinement branch. SARAF does not explicitly classify itself in §2.2; this is not a claim that the complete method is training-free post-processing.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## ROAR: Retrieval Opportunity-Aware Refinement for Zero-Shot Time Series Forecasting

- Record: `arxiv-2605.24911`
- Role: core
- Known public year: 2026; earliest verified date: 2026-05-24
- Date qualification: 同一arXiv记录v1为Factorize to Generalize: Retrieval-Guided Invariant-Dynamic Decomposition for Time Series Forecasting (RIDDE)；ROAR标题及当前方法为v2，2026-10-08。应计为一个版本链而非两篇独立记录。
- Venue: preprint
- Venue evidence: No accepted venue verified; preprint.
- Paper: https://arxiv.org/abs/2605.24911
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Estimate whether a query offers useful retrieval opportunity, then apply a retrieval-guided correction to the forecasting output. The current ROAR paper is a revision of RIDDE under the same arXiv identifier.
- Method source: https://arxiv.org/html/2605.24911v2
- Related version titles: Factorize to Generalize: Retrieval-Guided Invariant-Dynamic Decomposition
- Note: 未找到作者官方代码链接。避免将RIDDE和ROAR重计；如需要严格按方法版本分类，应保留v1输入增强→v2后校正变更注记。
- Note: 同一arXiv记录v1为Factorize to Generalize: Retrieval-Guided Invariant-Dynamic Decomposition for Time Series Forecasting (RIDDE)；ROAR标题及当前方法为v2，2026-10-08。应计为一个版本链而非两篇独立记录。

## Channel-wise Retrieval for Multivariate Time Series Forecasting

- Record: `arxiv-2604.05543`
- Role: core
- Known public year: 2026; earliest verified date: 2026-04-07
- Date qualification: Earliest verified arXiv v1 submission date; IEEE Xplore added the article on 2026-04-21.
- Venue: ICASSP 2026 (Oral)
- Venue evidence: https://ieeexplore.ieee.org/abstract/document/11463178
- Paper: https://arxiv.org/abs/2604.05543
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: §3.3 performs independent retrieval for each channel: a time-domain sparse relation graph restricts candidates and low-frequency complex spectral cosine ranks them. §3.4 projects and averages retrieved future horizons, then adds alpha times this retrieval forecast to a separate direct forecast. The paper explicitly says the additive correction can augment any forecaster without architecture changes.
- Method source: https://arxiv.org/html/2604.05543v2
- Note: Independent of SpecReTF: different title, authors, arXiv identity, and algorithm. IEEE verifies ICASSP 2026; the official program verifies Oral. No author-verified public code URL found.
- Note: Earliest verified arXiv v1 submission date; IEEE Xplore added the article on 2026-04-21.

## Not All Retrievals are Useful: Cross-Attention for Input-Aware RAG in Time Series Forecasting

- Record: `arxiv-2603.14709`
- Role: core
- Known public year: 2026; earliest verified date: 2026-03-16
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: KDD MILETS Workshop 2026 (oral presentation)
- Venue evidence: https://kdd-milets.github.io/milets2026/
- Paper: https://arxiv.org/abs/2603.14709
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Cross-attention conditions the relevance of retrieved historical segments on the current input and integrates selected representations before forecasting.
- Method source: https://arxiv.org/html/2603.14709v3
- Code link reported by an author/paper: https://github.com/seunghan96/cross-rag/ (availability and implementation completeness are not implied unless noted below)
- Note: Workshop官方日程列为ID7，并在Oral Session条目下出现；不要写成KDD主会。

## Retrieval-Augmented Generation with Covariate Time Series

- Record: `arxiv-2603.04951`
- Role: core
- Known public year: 2026; earliest verified date: 2026-03-05
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: https://arxiv.org/abs/2603.04951
- Paper: https://arxiv.org/abs/2603.04951
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Hierarchical raw-regime knowledge base, two-stage pointwise/multivariate retrieval, and self-supervised context-count selection supply retrieved examples to a frozen TSFM for numeric sensor forecasting.
- Method source: https://arxiv.org/html/2603.04951v2
- Code link reported by an author/paper: https://github.com/RAG4CTS-Project/RAG4CTS (availability and implementation completeness are not implied unless noted below)
- Note: Prediction used downstream for maintenance; actual numeric forecasting makes this in scope.

## TS-Memory: Plug-and-Play Memory for Time Series Foundation Models

- Record: `arxiv-2602.11550`
- Role: related; training_time_retrieval
- Known public year: 2026; earliest verified date: 2026-02-12
- Date qualification: Earliest verified arXiv v1 submission date.
- Venue: KDD 2026 (Research Track)
- Venue evidence: https://kdd2026.kdd.org/papers/
- Paper: https://arxiv.org/abs/2602.11550
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: The abstract and §§4.1–4.3 explicitly describe offline retrieval: a leakage-safe kNN teacher aggregates historical futures into quantile targets; these distributional corrections are distilled into a lightweight parametric memory adapter. At inference the adapter fuses with the frozen TSFM without datastore search. It is retrieval-distilled forecasting, not online retrieval-augmented forecasting.
- Method source: https://arxiv.org/html/2602.11550v1
- Code link reported by an author/paper: https://github.com/sisuolv/TS-Memory (availability and implementation completeness are not implied unless noted below)
- Note: Official code is linked from current arXiv abstract. Can be listed in Related Work / Retrieval Distillation. Its output fusion resembles post-hoc refinement structurally, but SARAF's online retrieval categories should not obscure that deployment is retrieval-free.
- Note: Earliest verified arXiv v1 submission date.
- Note: Retrieval provides an offline teacher; the deployed forecasting model is retrieval-free.

## MemCast: Memory-Driven Time Series Forecasting with Experience-Conditioned Reasoning

- Record: `arxiv-2602.03164`
- Role: core
- Known public year: 2026; earliest verified date: 2026-02-03
- Date qualification: Earliest verified arXiv v1 submission date.
- Venue: ICML 2026
- Venue evidence: https://proceedings.mlr.press/v306/tao26a.html
- Paper: https://arxiv.org/abs/2602.03164
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: §3.3 constructs hierarchical memory from training examples: historical future summaries, successful/failed forecasting experience, and general laws. §3.4 retrieves top-k patterns using a hybrid cosine-feature/DTW score and constructs an augmented LLM context P(Y|X,C_sim); retrieved reasoning experience also supports trajectory selection. Reflection may revise forecasts, but retrieval principally supplies input context rather than an independent numerical correction forecast.
- Method source: https://arxiv.org/html/2602.03164v1
- Code link reported by an author/paper: https://github.com/ustc-time-series/MemCast (availability and implementation completeness are not implied unless noted below)
- Note: The paper's original code URL https://github.com/Xiaoyu-Tao/MemCast-TS redirects to the listed official repository. ICML venue is verified in PMLR.
- Note: Earliest verified arXiv v1 submission date.

## VARDiff: Vision-augmented retrieval-guided diffusion for stock forecasting

- Record: `vardiff`
- Role: provisional
- Known public year: 2026; earliest verified date: not established
- Date qualification: Exact earliest posting date has not been established.
- Venue: Information Sciences 2026
- Venue evidence: https://www.sciencedirect.com/science/article/pii/S0020025526000447
- Paper: https://doi.org/10.1016/j.ins.2026.123113
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: publisher_method_excerpt
- Method: Publisher methods/abstract: Image-encoded historical trajectories retrieved with pretrained vision embeddings guide a conditional diffusion denoiser through cross-attention; generation is conditioned throughout.
- Method source: https://www.sciencedirect.com/science/article/pii/S0020025526000447
- Code link reported by an author/paper: https://github.com/AppliedAI-Lab/VARDiff (availability and implementation completeness are not implied unless noted below)
- Note: Volume 736, 2026-04-25, article 123113; exact early-online date not verified. Author name differs slightly between publisher contribution text and repository BibTeX.

## TimeMRA: LLM-Empowered Time Series Forecasting via Multi-Scale Retrieval-Augmented Representations

- Record: `timemra`
- Role: related; same_input_semantic_attention
- Known public year: 2026; earliest verified date: not established
- Date qualification: 2026；未能确认最早公开日。PMLR卷306正式出版日为2026-09-29，会议日期2026-07-06至11；不能将出版日自动当作首次公开日。OpenReview正文和API当前无法读取日期。
- Venue: ICML 2026 (PMLR 306:109951–109968)
- Venue evidence: https://proceedings.mlr.press/v306/shang26b.html
- Paper: https://proceedings.mlr.press/v306/shang26b.html
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: Section 4.3, Eq. (20): time features query multiscale LLM semantic representations generated from the same input; decoding and projection follow in Eqs. (21)–(23). This is not historical context–continuation retrieval.
- Method source: https://raw.githubusercontent.com/mlresearch/v306/main/assets/shang26b/shang26b.pdf
- Code link reported by an author/paper: https://github.com/shangzongjiang/TimeMRA (availability and implementation completeness are not implied unless noted below)
- Note: 已下载官方PDF并读取§2.2和§4。正式venue及代码已核验；首次公开日期未核验。
- Note: 2026；未能确认最早公开日。PMLR卷306正式出版日为2026-09-29，会议日期2026-07-06至11；不能将出版日自动当作首次公开日。OpenReview正文和API当前无法读取日期。
- Note: Attention retrieves semantic representations derived from the same input, rather than historical context–continuation examples.

## TabPFN-TSRA: Retrieval-Augmented TabPFN for Time-Series Forecasting

- Record: `tabpfn-tsra`
- Role: core
- Known public year: 2026; earliest verified date: not established
- Date qualification: Exact initial publication day could not be verified. Do not substitute search-engine relative dates. Public workshop record is 2026.
- Venue: 2nd ICML Workshop on Foundation Models for Structured Data (FMSD), 2026
- Venue evidence: https://icml-structured-fm-workshop.github.io/accepted-papers/
- Paper: https://openreview.net/forum?id=pGK4RbJTC9
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Paper §2 and official code describe level-shift-corrected correlation retrieval of historical analogues and their observed continuations. Retrieved windows become temporally aligned feature columns for TabPFN regression; no explicit gradient fine-tuning of TabPFN is required.
- Method source: https://openreview.net/pdf?id=pGK4RbJTC9
- Code link reported by an author/paper: https://github.com/sibo-cai/TabPFN-TSRA (availability and implementation completeness are not implied unless noted below)
- Note: Curator assignment from paper and official implementation; not in SARAF §2.2.
- Note: Exact initial publication day could not be verified. Do not substitute search-engine relative dates. Public workshop record is 2026.

## Spectral Retrieval-Augmented Time-Series Forecasting

- Record: `arxiv-2606.19412`
- Role: core
- Known public year: 2026; earliest verified date: not established
- Date qualification: arXiv v1 is verified as 2026-06-17, but an earlier anonymous ICLR 2026 OpenReview manuscript exists. Its exact first-public date and decision could not be verified; do not label the arXiv date as absolute first publication.
- Venue: arXiv preprint; earlier ICLR 2026 submission exists, acceptance unverified
- Venue evidence: https://arxiv.org/abs/2606.19412
- Paper: https://arxiv.org/abs/2606.19412
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: §3.3: STFT-based amplitude/phase similarity with recency weighting selects top-K historical context/future pairs. Retrieved futures are similarity-weighted then linearly projected to a retrieval forecast; a separate query pathway makes a direct forecast. These two forecast outputs are concatenated and linearly fused. Under SARAF's broad distinction, this is output-level ensemble/refinement rather than appending retrieved segments to the input.
- Method source: https://arxiv.org/html/2606.19412v1
- Note: Taxonomy mapping has medium confidence because the main architecture is jointly trained, rather than strictly post-training correction; its retrieval branch combines at forecast level. Not the same as CRAFT or SIREN. No verified public code URL found.
- Note: arXiv v1 is verified as 2026-06-17, but an earlier anonymous ICLR 2026 OpenReview manuscript exists. Its exact first-public date and decision could not be verified; do not label the arXiv date as absolute first publication.

## Retrieve the Right Signal: Decomposition-Guided Retrieval-Augmented Forecasting for Financial Markets

- Record: `retrieve-the-right-signal`
- Role: pending
- Known public year: 2026; earliest verified date: not established
- Date qualification: Exact earliest posting date has not been established.
- Venue: CIKM 2026
- Venue evidence: https://cikm2026.diag.uniroma1.it/program/
- Paper: https://cikm2026.diag.uniroma1.it/program/
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: official_program_abstract
- Method: Official accepted-program abstract: Causal trend decomposition, retrieval in detrended space, retrieved futures used as direct forecasts and Retrieval-as-Context tokens into the backbone.
- Method source: https://cikm2026.diag.uniroma1.it/program/
- Note: No full manuscript located; method acronym rendered as unresolved LaTeX. Include only as separately marked accepted/pending-original entry until full text read.

## Retrieval Mechanisms Surpass Long-Context Scaling in Time Series Forecasting

- Record: `arxiv-2605.08217`
- Role: related; evaluation
- Known public year: 2026; earliest verified date: not established
- Date qualification: Exact earliest public date not verified. Author CV labels the project February 2026; the official workshop accepted list confirms a pre-arXiv workshop paper. arXiv v1 was submitted 2026-05-06 12:15:05 UTC. Do not label May 6 the first public date without this qualification.
- Venue: ICLR 2026 Workshop on Time Series in the Age of Large Models (TSALM), accepted research paper
- Venue evidence: https://tsalm-workshop.github.io/accepted-papers/
- Paper: https://arxiv.org/abs/2605.08217
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: Sections 3.1, 3.5 and 4.3 evaluate the existing RAFT baseline with a 720-step context and top-k cosine-similar historical segments. The paper describes retrieved segments entering the Transformer as dynamic exogenous inputs, before attention/forecasting. Its contribution is the comparison with continuous long-context scaling; do not count it as a new RAFT proposal.
- Method source: https://arxiv.org/html/2605.08217v1#S3
- Code link reported by an author/paper: https://github.com/RishiAhuja/ahuja2026retrieval (availability and implementation completeness are not implied unless noted below)
- Note: Exact earliest public date not verified. Author CV labels the project February 2026; the official workshop accepted list confirms a pre-arXiv workshop paper. arXiv v1 was submitted 2026-05-06 12:15:05 UTC. Do not label May 6 the first public date without this qualification.
- Note: Analysis/evaluation paper using the existing RAFT (Han et al., 2025) baseline; not a new independently named forecasting method
- Note: Official code URL is stated in paper Appendix F; opening the repository did not return content, so repository availability is not verified
- Note: Compares the existing RAFT method with long-context scaling; not a new forecasting method.

## An improved retrieval-augmented long-term grouting power prediction method: Rejecting low-similarity retrievals

- Record: `grouting-retrieval-2026`
- Role: provisional
- Known public year: 2026; earliest verified date: not established
- Date qualification: Exact earliest posting date has not been established.
- Venue: Engineering Applications of Artificial Intelligence 2026
- Venue evidence: https://www.sciencedirect.com/science/article/pii/S0952197625027642
- Paper: https://doi.org/10.1016/j.engappai.2025.112733
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: publisher_method_excerpt
- Method: Publisher method text: TimeXer is trained first; retrieved target continuations below a similarity threshold are substituted with the TimeXer prediction, and a separately trained GRU fuses the processed forecasts. A final fixed-model stage tunes the rejection threshold.
- Method source: https://www.sciencedirect.com/science/article/pii/S0952197625027642
- Note: Published issue Volume163 Part1, 2026-01-01; exact early online date unknown (DOI contains 2025, not proof of first-public date).

## Predicting the Future by Retrieving the Past

- Record: `arxiv-2511.05859`
- Role: core
- Known public year: 2025; earliest verified date: 2025-11-08
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: AAAI 2026, Technical Track on Machine Learning II, 40(25):20896–20904
- Venue evidence: https://ojs.aaai.org/index.php/AAAI/article/view/39230
- Paper: https://arxiv.org/abs/2511.05859
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Methodology builds a Global Memory Bank of historical patterns and their continuations. Retrieval produces a global forecast, dynamically fused with a local forecaster output. SARAF groups it with post-hoc refinement, although PFRP contains learned fusion and should not be described as universally training-free.
- Method source: https://arxiv.org/html/2511.05859#Sx3
- Code link reported by an author/paper: https://github.com/ddz16/PFRP (availability and implementation completeness are not implied unless noted below)
- Note: Explicitly assigned by SARAF §2.2.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## Learning from History: A Retrieval-Augmented Framework for Spatiotemporal Prediction

- Record: `arxiv-2510.24049`
- Role: related; spatiotemporal_field_prediction
- Known public year: 2025; earliest verified date: 2025-10-28
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: https://arxiv.org/abs/2510.24049
- Paper: https://arxiv.org/abs/2510.24049
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: Historical nearest analogs supply true future evolution as a conditional reference; separate query/reference encoders are concatenated before a decoder. Evaluations are meteorology, turbulence, and wildfire fields.
- Method source: https://arxiv.org/html/2510.24049v1
- Note: Grid/physical-field prediction; keep in explicitly labeled extended applications if main scope is ordinary numerical TS.
- Note: Retrieval for grid-valued weather, turbulence and wildfire prediction; an extension beyond the main sequence-forecasting scope.

## Retrieval-Augmented Framework with Adaptive Gating for Time Series Forecasting

- Record: `adaptive-gating-2025`
- Role: provisional
- Known public year: 2025; earliest verified date: 2025-09-05
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: Journal of Shanghai Jiaotong University (Science) 2025
- Venue evidence: https://link.springer.com/article/10.1007/s12204-025-2847-z
- Paper: https://doi.org/10.1007/s12204-025-2847-z
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: publisher_abstract
- Method: Publisher abstract describes time/frequency top-k historical retrieval, cross-attention between query and references in a retrieval branch, and adaptive gating with the original branch.
- Method source: https://link.springer.com/article/10.1007/s12204-025-2847-z
- Note: Full text paywalled; classification provisional from explicit publisher method description.

## STRATA-TS: Selective Knowledge Transfer for Urban Time Series Forecasting with Retrieval-Guided Reasoning

- Record: `arxiv-2508.18635`
- Role: core
- Known public year: 2025; earliest verified date: 2025-08-26
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: https://arxiv.org/abs/2508.18635
- Paper: https://arxiv.org/abs/2508.18635
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: §3 inference procedure: A pretrained spatio-temporal base model first generates prediction tokens; fine-tuned LLaMA receives these, city context, and retrieved source sequences/metadata to produce the final corrected forecast. Retrieval also conditions the final LLM input, so this is a hybrid.
- Method source: https://arxiv.org/html/2508.18635v2
- Note: Choose primary post-hoc relative to the ST base forecaster; explicitly flag input-conditioning secondary role.

## FLAIRR-TS – Forecasting LLM-Agents with Iterative Refinement and Retrieval for Time Series

- Record: `arxiv-2508.19279`
- Role: core
- Known public year: 2025; earliest verified date: 2025-08-24
- Date qualification: Earliest verified arXiv v1 submission date.
- Venue: Findings of EMNLP 2025
- Venue evidence: https://aclanthology.org/2025.findings-emnlp.834/
- Paper: https://arxiv.org/abs/2508.19279
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Published paper §2.2: a sliding-window database is built from the training split; Pearson correlation retrieves the top-M historical context segments together with their actual continuations, and these examples directly augment the Forecaster-agent context. The Refiner-agent iteratively updates prompts, but the retrieval mechanism enters through the input, not a numerical output-correction ensemble.
- Method source: https://aclanthology.org/2025.findings-emnlp.834.pdf
- Note: No author-verified public code URL found. Taxonomy assignment is this review's mapping to SARAF §2.2, not a label claimed by the authors.
- Note: Earliest verified arXiv v1 submission date.

## A Retrieval Augmented Spatio-Temporal Framework for Traffic Prediction

- Record: `arxiv-2508.16623`
- Role: core
- Known public year: 2025; earliest verified date: 2025-08-14
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: AAAI 2026 AI for Social Impact Track
- Venue evidence: https://ojs.aaai.org/index.php/AAAI/article/view/41264
- Paper: https://arxiv.org/abs/2508.16623
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Original paper framework: Decoupled spatial/temporal vectors are retrieved from memory, fused with queries by cross-attention, then passed to a universal predictor; retrieval operates before the prediction head.
- Method source: https://ojs.aaai.org/index.php/AAAI/article/download/41264/45225
- Code link reported by an author/paper: https://github.com/RWLinno/RAST (availability and implementation completeness are not implied unless noted below)
- Note: Official proceedings identifies AI for Social Impact special track, not technical main track.

## TRACE: Grounding Time Series in Context for Multimodal Embedding and Retrieval

- Record: `arxiv-2506.09114`
- Role: core
- Known public year: 2025; earliest verified date: 2025-06-10
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: NeurIPS 2025, Main Conference Track
- Venue evidence: https://proceedings.neurips.cc/paper_files/paper/2025/hash/03adea6231459e2aab0a68d0aa19793a-Abstract-Conference.html
- Paper: https://arxiv.org/abs/2506.09114
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Section 3.4 retrieves time-series/text pairs with context-grounded embeddings. Their representations become a learned soft prompt prepended to a frozen TSFM query. Section 4.4 evaluates retrieval-augmented forecasting. This is Chen et al. multimodal TRACE, not the different paper named TRACE about parameter-efficient learning.
- Method source: https://arxiv.org/html/2506.09114#S3.SS4
- Code link reported by an author/paper: https://github.com/Graph-and-Geometric-Learning/TRACE-Multimodal-TSEncoder (availability and implementation completeness are not implied unless noted below)
- Note: Explicitly assigned by SARAF §2.2.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## Retrieval-Augmented Forecasting with Tabular Time Series Data

- Record: `raf-li-tabular`
- Role: core
- Known public year: 2025; earliest verified date: 2025-06-05
- Date qualification: OpenReview public search record reports Published 05 Jun 2025; ACL Anthology archival volume is July 2025.
- Venue: 4th Table Representation Learning Workshop (TRL at ACL 2025), pp. 192–199
- Venue evidence: https://aclanthology.org/2025.trl-1.16/
- Paper: https://aclanthology.org/2025.trl-1.16/
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Sections 3.2–3.3: a schema-aware dual encoder retrieves historical table slices using schema alignment and temporal decay; a Transformer consumes retrieved tables through cross-attention. Retriever and forecaster are co-trained. It is not the Tire RAF paper, nor evidence of using a pretrained TSFM.
- Method source: https://aclanthology.org/2025.trl-1.16.pdf
- Note: Explicitly cited alongside Tire RAF in SARAF §2.2; the two are separate works.
- Note: OpenReview public search record reports Published 05 Jun 2025; ACL Anthology archival volume is July 2025.

## Improving Time Series Forecasting via Instance-aware Post-hoc Revision

- Record: `arxiv-2505.23583`
- Role: core
- Known public year: 2025; earliest verified date: 2025-05-29
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: NeurIPS 2025, Main Conference Track
- Venue evidence: https://proceedings.neurips.cc/paper_files/paper/2025/hash/331c41353b053683e17f7c88a797701d-Abstract-Conference.html
- Paper: https://arxiv.org/abs/2505.23583
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: Section 3 first identifies unreliable forecasts, then performs local revision using covariates/exogenous context and global revision using similar historical instances. The revised outputs are combined with the original forecast. This is genuinely forecast-level revision, with learned revision modules.
- Method source: https://arxiv.org/html/2505.23583#S3
- Code link reported by an author/paper: https://github.com/ustc-time-series/PIR (availability and implementation completeness are not implied unless noted below)
- Note: Explicitly assigned by SARAF §2.2.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## Retrieval Augmented Time Series Forecasting

- Record: `arxiv-2505.04163`
- Role: core
- Known public year: 2025; earliest verified date: 2025-05-07
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: ICML 2025 (PMLR 267:21774–21797)
- Venue evidence: https://proceedings.mlr.press/v267/han25d.html
- Paper: https://arxiv.org/abs/2505.04163
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Sections 3.2–3.3: multi-period retrieval matches training histories using Pearson correlation. The associated future values augment the query for forecasting; the model learns to use the retrieved evidence.
- Method source: https://arxiv.org/html/2505.04163#S3
- Code link reported by an author/paper: https://github.com/archon159/RAFT (availability and implementation completeness are not implied unless noted below)
- Note: Explicitly assigned by SARAF §2.2.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## TS-RAG: Retrieval-Augmented Generation based Time Series Foundation Models are Stronger Zero-Shot Forecaster

- Record: `arxiv-2503.07649`
- Role: core
- Known public year: 2025; earliest verified date: 2025-03-06
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: NeurIPS 2025, Main Conference Track
- Venue evidence: https://proceedings.neurips.cc/paper_files/paper/2025/hash/eed25c037bc08afcbefab6f7a6b700e0-Abstract-Conference.html
- Paper: https://arxiv.org/abs/2503.07649
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Section 3.2 uses pretrained encoder embeddings and Euclidean nearest-neighbor retrieval over a dedicated database. An Adaptive Retrieval Mixer integrates retrieved contexts with the TSFM representation for zero-shot forecasting. Use the final ARM terminology rather than automatically copying the older v1 MoE description.
- Method source: https://arxiv.org/html/2503.07649#S3.SS2
- Code link reported by an author/paper: https://github.com/UConn-DSIS/TS-RAG (availability and implementation completeness are not implied unless noted below)
- Note: Explicitly assigned by SARAF §2.2.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## Retrieval-augmented Large Language Models for Financial Time Series Forecasting

- Record: `arxiv-2502.05878`
- Role: core
- Known public year: 2025; earliest verified date: 2025-02-09
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: preprint
- Venue evidence: https://arxiv.org/abs/2502.05878
- Paper: https://arxiv.org/abs/2502.05878
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: §3.2–3.3: FinSeer learns retrieval relevance from StockLLM feedback; retrieved historical price/indicator sequences are provided alongside the query to StockLLM for future stock-movement prediction.
- Method source: https://arxiv.org/html/2502.05878v3#S3
- Related version titles: Enhancing Financial Time-Series Forecasting with Retrieval-Augmented Large Language Models
- Note: Stock movement direction classification, not continuous-value forecasting. Earlier title Enhancing Financial Time-Series Forecasting with Retrieval-Augmented Large Language Models is the same arXiv record.

## Time-VLM: Exploring Multimodal Vision-Language Models for Augmented Time Series Forecasting

- Record: `arxiv-2502.04395`
- Role: core
- Known public year: 2025; earliest verified date: 2025-02-06
- Date qualification: Earliest verified arXiv v1 submission date.
- Venue: ICML 2025
- Venue evidence: https://proceedings.mlr.press/v267/zhong25a.html
- Paper: https://arxiv.org/abs/2502.04395v2
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Latest v2 §3.1 explicitly maintains a capacity-M circular memory bank of historical patch representations. Current patches retrieve cosine-similar top-k memories; an MLP processes retrieved features and adds them residually to the input patch features. These temporal features combine with VLM visual/text embeddings before a forecasting head. This is historical-feature retrieval augmenting the forecasting input/representation.
- Method source: https://arxiv.org/html/2502.04395
- Code link reported by an author/paper: https://github.com/CityMind-Lab/ICML25-TimeVLM (availability and implementation completeness are not implied unless noted below)
- Note: Important version distinction: v1 §3.1 primarily described learnable memory queries attending to current patch embeddings; v2 replaces the description with an explicit historical circular buffer and top-k retrieval. Classify from v2, not v1. Buffer update/order and split boundaries deserve care in reproducibility.
- Note: Earliest verified arXiv v1 submission date.

## TimeRAF: Retrieval-Augmented Foundation model for Zero-shot Time Series Forecasting

- Record: `arxiv-2412.20810`
- Role: core
- Known public year: 2024; earliest verified date: 2024-12-30
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: IEEE Transactions on Knowledge and Data Engineering 37(9):5654–5665, 2025
- Venue evidence: https://doi.org/10.1109/TKDE.2025.3579137
- Paper: https://arxiv.org/abs/2412.20810
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Sections 3.4–3.5: an end-to-end learnable retriever selects knowledge-base time-series segments. Channel Prompting integrates retrieved and query embeddings before the forecasting backbone, supporting zero-shot forecasting. This differs from DTW-based TimeRAG.
- Method source: https://arxiv.org/html/2412.20810#S3
- Code link reported by an author/paper: https://github.com/hwanyu112/TimeRAF (availability and implementation completeness are not implied unless noted below)
- Note: TimeRAF is the actual Zhang et al. bibliography item behind SARAF’s mismatched TimeRAG citation. Assignment also independently supported by its method.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## TimeRAG: BOOSTING LLM Time Series Forecasting via Retrieval-Augmented Generation

- Record: `arxiv-2412.16643`
- Role: core
- Known public year: 2024; earliest verified date: 2024-12-21
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: ICASSP 2025
- Venue evidence: https://ieeexplore.ieee.org/abstract/document/10889933/metrics
- Paper: https://arxiv.org/abs/2412.16643
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Section II constructs a clustered historical knowledge base, retrieves similar reference sequences with DTW, and combines references with the prediction query as an LLM prompt.
- Method source: https://arxiv.org/html/2412.16643#S2
- Note: SARAF §2.2 names TimeRAG and describes this mechanism, but its linked Zhang et al. reference is TimeRAF. Identity and category were repaired using the TimeRAG primary paper.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## Retrieval Augmented Time Series Forecasting

- Record: `arxiv-2411.08249`
- Role: core
- Known public year: 2024; earliest verified date: 2024-11-12
- Date qualification: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions
- Venue: AISTATS 2026 (PMLR 300:4294–4302)
- Venue evidence: https://proceedings.mlr.press/v300/tire26a.html
- Paper: https://arxiv.org/abs/2411.08249
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: Section 4: Chronos-encoder embeddings retrieve historical context–continuation pairs by nearest-neighbor similarity. Retrieved sequences are normalized, continuity-aligned, and concatenated before the query context as TSFM input. This is distinct from Han et al. RAFT despite the identical paper title.
- Method source: https://arxiv.org/html/2411.08249#S4
- Code link reported by an author/paper: https://github.com/kutaytire/Retrieval-Augmented-Time-Series-Forecasting (availability and implementation completeness are not implied unless noted below)
- Note: Explicitly cited in SARAF §2.2 input-augmentation paragraph; method rechecked against arXiv v2.
- Note: arXiv v1 submission date; earliest verified authored preprint in this check, not a claim excluding earlier anonymous public submissions

## Retrieval-Augmented Diffusion Models for Time Series Forecasting

- Record: `arxiv-2410.18712`
- Role: core
- Known public year: 2024; earliest verified date: 2024-10-24
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: NeurIPS 2024
- Venue evidence: https://proceedings.neurips.cc/paper_files/paper/2024/hash/053ee34c0971568bfa5c773015c10502-Abstract-Conference.html
- Paper: https://arxiv.org/abs/2410.18712
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: §4.1–4.3: Top-k embedding-based references from training windows condition each denoising step through Reference-Modulated Attention. Retrieval guides generation rather than correcting a completed forecast.
- Method source: https://arxiv.org/html/2410.18712v1#S4
- Code link reported by an author/paper: https://github.com/stanliu96/RATD (availability and implementation completeness are not implied unless noted below)

## Agentic Retrieval-Augmented Generation for Time Series Analysis

- Record: `arxiv-2408.14484`
- Role: core
- Known public year: 2024; earliest verified date: 2024-08-18
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: KDD 2024 Undergraduate Consortium
- Venue evidence: https://kdd.org/kdd2024/undergraduate-consortium/
- Paper: https://arxiv.org/abs/2408.14484
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: §3 and forecasting experiments: Task-specific agents retrieve prompts containing historical-pattern knowledge from shared prompt pools and use them with the current input; forecasting is one of four evaluated tasks.
- Method source: https://arxiv.org/html/2408.14484v1
- Note: Official program confirms Undergraduate Consortium, not KDD main track or generic KDD workshop.

## Resolution-Aware Retrieval Augmented Zero-Shot Forecasting

- Record: `arxiv-2510.16695`
- Role: core
- Known public year: 2024; earliest verified date: not established
- Date qualification: Exact earliest posting date has not been established.
- Venue: NeurIPS 2024 TSALM Workshop
- Venue evidence: https://tsalm-workshop.github.io/neurips-2024/
- Paper: https://arxiv.org/abs/2510.16695
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: §2.2–2.5: Retrieve reference weather stations at resolution-dependent spatial scales; a location-aware transfer component integrates retrieved station encodings before the Informer decoder predicts.
- Method source: https://arxiv.org/html/2510.16695v1#S2
- Related version titles: Towards Resolution-Aware Retrieval Augmented Zero-Shot Forecasting
- Note: Workshop precursor titled Towards Resolution-Aware Retrieval Augmented Zero-Shot Forecasting, presented 2024-12-15, OpenReview JnNCD8jEgp; expanded arXiv first submitted 2025-10-19. Exact earliest posting date not verified; use known_public_year 2024 rather than claiming first posting day.
- Note: The 2024 workshop title begins “Towards”; the later arXiv version drops that word. This catalogue treats the workshop and expanded preprint as one version family, without asserting identical content.

## Nearest Neighbor Multivariate Time Series Forecasting

- Record: `arxiv-2505.11625`
- Role: core
- Known public year: 2024; earliest verified date: not established
- Date qualification: Known public year 2024 is supported by the authors’ McGill IALab publication list, 2024 section item 10, and the author manuscript’s ©2024 IEEE publication statement. The exact earliest day was not primary-verified on final recheck; the arXiv v1 date is 2025-05-16, and the final journal issue is July 2025.
- Venue: IEEE TNNLS 2025
- Venue evidence: https://ieeexplore.ieee.org/document/10752995/
- Paper: https://arxiv.org/abs/2505.11625
- SARAF mapping: Retrieval as Post-hoc Refinement
- Evidence level: full_text
- Method: §III-A–B and Eq.3: Cache model representations and corresponding future values, retrieve nearest neighbors, and interpolate a similarity-weighted future with the original model forecast. No additional retrieval training required.
- Method source: https://arxiv.org/html/2505.11625v1#S3.SS2
- Code link reported by an author/paper: https://github.com/hlhang9527/KNN-MTS (availability and implementation completeness are not implied unless noted below)
- Note: Keep 2024 as the known public year; do not claim a verified November 14 day because the IEEE page could not expose that date on final recheck. The author-lab bibliography is the primary year evidence. arXiv first submission 2025-05-16 is a later posting, not the first-public year. Final journal issue: IEEE TNNLS 36(7):12606–12618, July 2025. Code URL appears in original paper; repository availability has not been re-opened.
- Note: Known public year 2024 is supported by the authors’ McGill IALab publication list, 2024 section item 10, and the author manuscript’s ©2024 IEEE publication statement. The exact earliest day was not primary-verified on final recheck; the arXiv v1 date is 2025-05-16, and the final journal issue is July 2025.

## Retrieval Based Time Series Forecasting

- Record: `arxiv-2209.13525`
- Role: core
- Known public year: 2022; earliest verified date: 2022-09-27
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: CIKM 2022 AMLTS Workshop
- Venue evidence: https://arxiv.org/pdf/2209.13525
- Paper: https://arxiv.org/abs/2209.13525
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: §4.1–4.2: Relational retrieval selects related reference series using a graph, takes period-aligned snippets, separately embeds target and references, concatenates them, and applies content/temporal attention before output synthesis.
- Method source: https://arxiv.org/pdf/2209.13525
- Note: Workshop explicitly named on original first page; do not call CIKM main conference or copy placeholder DOI.

## MQRetNN: Multi-Horizon Time Series Forecasting with Retrieval Augmentation

- Record: `arxiv-2207.10517`
- Role: core
- Known public year: 2022; earliest verified date: 2022-07-21
- Date qualification: Earliest date established in this review; earlier public versions may exist.
- Venue: KDD 2022 MileTS Workshop
- Venue evidence: https://kdd-milets.github.io/milets2022/papers/MILETS_2022_paper_4213.pdf
- Paper: https://arxiv.org/abs/2207.10517
- SARAF mapping: Retrieval as Input Augmentation
- Evidence level: full_text
- Method: §3.2–3.3: Cross-entity retrieval selects encoded contexts from an offline pretrained MQCNN datastore, adds cross-entity attention after the encoder, and concatenates retrieved context to the input embedding. Workshop version title is MQ-ReTCNN; treat as the same work.
- Method source: https://arxiv.org/pdf/2207.10517
- Related version titles: MQ-ReTCNN: Multi-Horizon Time Series Forecasting with Retrieval Augmentation
- Note: Do not copy placeholder ACM DOI from workshop PDF.

## Self-adaptive Retrieval-Augmented Reinforcement Learning for Time Series Forecasting

- Record: `srrf`
- Role: pending
- Known public year: unverified; earliest verified date: not established
- Date qualification: 最早公开日期未由官方来源确认；不可按ICLR2026标签自动写2026首发。
- Venue: preprint / OpenReview submission; ICLR 2026 acceptance unconfirmed
- Venue evidence: https://openreview.net/forum?id=1jlci3sF4Q
- Paper: https://openreview.net/pdf?id=1jlci3sF4Q
- SARAF mapping: Not assigned to the main two-way taxonomy
- Evidence level: full_text
- Method: Section 3 and Figure 2: retrieved historical futures inform reinforcement-learning states during training. Inference retains only the trained base model, with no retrieval overhead.
- Method source: https://openreview.net/pdf?id=1jlci3sF4Q
- Note: 官方PDF的可搜索正文是Anonymous/Paper under double-blind review；forum被验证页阻挡，API返回403，未核验decision。二手库列Shiyuan Teng, Binli Luo, Xianhan Tan, Song Yu, Zhifang Liao及匿名代码https://anonymous.4open.science/r/ACAC-9999/README.md，但这些作者/代码与ICLR接收不能以二手条目当正式结论。建议放待核验或训练期相关工作附录。
- Note: 最早公开日期未由官方来源确认；不可按ICLR2026标签自动写2026首发。

