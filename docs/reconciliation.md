# Reconciliation with the previous corpus

The earlier 38-core / 51-total draft did not continue from the full previous database. There were real omissions, in addition to differences in scope.

## Verified counts

- Previous source: 112 raw records, 8 duplicate records, 104 distinct records.
- Previous HTML: 104 records = 58 core + 27 contextual + 14 candidate + 5 excluded.
- Previous HTML, source ZIP and repository data were compared and are identical.
- Earlier current draft: 51 records = 38 core + 8 related + 3 provisional + 2 pending.
- Intersection: 28 records. Absent old records: 76, including 36 old core records.
- New-to-old-corpus records: 23. Reconciled union: 104 + 51 − 28 = 127.
- All 104 previous IDs remain in the new master corpus. None was silently deleted.

## Why 38 was misleading

The new search started from a narrower modern forecasting view rather than reconciling the established corpus first. This lost both legitimate historical/contextual records and genuine inference-time retrieval methods. The correction restores the original corpus and treats new classification as a view, not a destructive replacement.

## Intersection: 28 records

- `yang2022mqretnn` ↔ `arxiv-2207.10517`: MQ-ReTCNN: Multi-Horizon Time Series Forecasting with Retrieval-Augmentation
- `jing2022retime` ↔ `arxiv-2209.13525`: Retrieval Based Time Series Forecasting
- `liu2024ratd` ↔ `arxiv-2410.18712`: Retrieval-Augmented Diffusion Models for Time Series Forecasting
- `liu2025pir` ↔ `arxiv-2505.23583`: Improving Time Series Forecasting via Instance-aware Post-hoc Revision
- `zhang2025knnmts` ↔ `arxiv-2505.11625`: Nearest Neighbor Multivariate Time Series Forecasting
- `xiao2025finsrag` ↔ `arxiv-2502.05878`: Retrieval-augmented Large Language Models for Financial Time Series Forecasting
- `han2025raft` ↔ `arxiv-2505.04163`: Retrieval Augmented Time Series Forecasting
- `zhang2025timeraf` ↔ `arxiv-2412.20810`: TimeRAF: Retrieval-Augmented Foundation Model for Zero-Shot Time Series Forecasting
- `yang2025timerag` ↔ `arxiv-2412.16643`: TimeRAG: Boosting LLM Time Series Forecasting via Retrieval-Augmented Generation
- `zhong2025timevlm` ↔ `arxiv-2502.04395`: Time-VLM: Exploring Multimodal Vision-Language Models for Augmented Time Series Forecasting
- `chen2025trace` ↔ `arxiv-2506.09114`: TRACE: Grounding Time Series in Context for Multimodal Embedding and Retrieval
- `ning2025tsrag` ↔ `arxiv-2503.07649`: TS-RAG: Retrieval-Augmented Generation based Time Series Foundation Models are Stronger Zero-Shot Forecaster
- `asadi2026alignrag` ↔ `arxiv-2608.05571`: Align-RAG: Alignment Is All You Need for TSFM In-Context Learning
- `kang2026craft` ↔ `arxiv-2604.05543`: Channel-wise Retrieval for Multivariate Time Series Forecasting
- `zhang2026kref` ↔ `arxiv-2608.06748`: KReF: Training-Free Retrieval for Long-Term Time-Series Forecasting and Predictive Uncertainty
- `villa2026raef` ↔ `arxiv-2608.14054`: Model-Agnostic Retrieval-Augmented Extended Forecasting for Time Series
- `lee2026crossrag` ↔ `arxiv-2603.14709`: Not All Retrievals are Useful: Cross-Attention for Input-Aware RAG in Time Series Forecasting
- `du2026pfrp` ↔ `arxiv-2511.05859`: Predicting the Future by Retrieving the Past
- `lyu2026reditt` ↔ `arxiv-2607.12391`: ReDiTT: Retrieval Augmented Conditional Diffusion Transformers for Asynchronous Time Series
- `liang2026rag4cts` ↔ `arxiv-2603.04951`: Retrieval-Augmented Generation with Covariate Time Series
- `tire2026raf` ↔ `arxiv-2411.08249`: Retrieval Augmented Time Series Forecasting
- `zhou2026seraf` ↔ `arxiv-2606.14941`: Semantics-Enhanced Retrieval-Augmented Time Series Forecasting
- `zhou2026saraf` ↔ `arxiv-2606.04135`: Stationarity-Aware Retrieval-Augmented Time Series Forecasting
- `tang2026tabpfntsra` ↔ `tabpfn-tsra`: TabPFN-TSRA: Retrieval-Augmented TabPFN for Time-Series Forecasting
- `lyu2026tsmemory` ↔ `arxiv-2602.11550`: TS-Memory: Plug-and-Play Memory for Time Series Foundation Models
- `xiao2026tsrag` ↔ `arxiv-2608.06223`: TS-RAG: Retrieval Augmented Generation for Time Series Forecasting
- `nguyen2026vardiff` ↔ `vardiff`: VARDiff: Vision-augmented retrieval-guided diffusion for stock forecasting
- `choi2026predictive` ↔ `arxiv-2608.23221`: Which Histories Matter for Time Series Forecasting? Learning Predictive Relevance with Future Supervision

## Restored omissions: 76 records

- [Atmospheric Predictability as Revealed by Naturally Occurring Analogues](https://journals.ametsoc.org/abstract/journals/atsc/26/4/1520-0469_1969_26_636_aparbn_2_0_co_2.xml) (Journal of the Atmospheric Sciences) — ID: `lorenz1969analogues`; legacy_contextual; previous: contextual
- [Nearest-neighbour methods for time series analysis](https://onlinelibrary.wiley.com/doi/pdf/10.1111/j.1467-9892.1987.tb00435.x) (Journal of Time Series Analysis) — ID: `yakowitz1987nearest`; legacy_contextual; previous: contextual
- [Predicting Chaotic Time Series](https://www.inet.ox.ac.uk/publications/predicting-chaotic-time-series) (Physical Review Letters) — ID: `farmer1987chaotic`; related; previous: core
- [A New Look at Weather Forecasting through Analogues](https://journals.ametsoc.org/abstract/journals/mwre/117/10/1520-0493_1989_117_2230_anlawf_2_0_co_2.xml) (Monthly Weather Review) — ID: `vandendool1989local`; legacy_contextual; previous: contextual
- [Nonlinear prediction of chaotic time series](https://www.sciencedirect.com/science/article/pii/0167278989900742) (Physica D: Nonlinear Phenomena) — ID: `casdagli1989nonlinear`; legacy_contextual; previous: contextual
- [Nonlinear forecasting as a way of distinguishing chaos from measurement error in time series](https://www.nature.com/articles/344734a0) (Nature) — ID: `sugihara1990nonlinear`; related; previous: core
- [Nonparametric Regression and Short-Term Freeway Traffic Forecasting](https://ascelibrary.org/doi/10.1061/%28ASCE%290733-947X%281991%29117%3A2%28178%29) (Journal of Transportation Engineering) — ID: `davis1991traffic`; legacy_contextual; previous: contextual
- [Multivariate nearest-neighbour forecasts of EMS exchange rates](https://onlinelibrary.wiley.com/doi/pdf/10.1002/jae.3950070511) (Journal of Applied Econometrics) — ID: `mizrach1992exchange`; legacy_contextual; previous: contextual
- [Learning Prediction of Time Series: A Theoretical and Empirical Comparison of CBR with Some Other Approaches](https://cdn.aaai.org/Workshops/1994/WS-94-01/WS94-01-012.pdf) (AAAI Technical Report WS-94-01) — ID: `nakhaeizadeh1994cbr`; legacy_contextual; previous: contextual
- [Searching for analogues, how long must we wait?](https://www.tandfonline.com/doi/pdf/10.3402/tellusa.v46i3.15481) (Tellus A) — ID: `vandendool1994waiting`; legacy_contextual; previous: contextual
- [Lazy learning for local modelling and control design](https://www.tandfonline.com/doi/abs/10.1080/002071799220830) (International Journal of Control) — ID: `bontempi1999lazy`; related; previous: core
- [Out-of-sample tests of forecasting accuracy: An analysis and review](https://www.sciencedirect.com/science/article/pii/S0169207000000650) (International Journal of Forecasting) — ID: `tashman2000`; legacy_contextual; previous: contextual
- [Comparison of parametric and nonparametric models for traffic flow forecasting](https://www.sciencedirect.com/science/article/abs/pii/S0968090X02000098) (Transportation Research Part C: Emerging Technologies) — ID: `smith2002traffic`; legacy_candidate; previous: candidate
- [Strictly Proper Scoring Rules, Prediction, and Estimation](https://sites.stat.washington.edu/people/raftery/Research/PDF/Gneiting2007jasa.pdf) (Journal of the American Statistical Association) — ID: `gneiting2007`; legacy_contextual; previous: contextual
- [Short-Term Load Forecasting: Similar Day-Based Wavelet Neural Networks](https://doi.org/10.1109/TPWRS.2009.2030426) (IEEE Transactions on Power Systems) — ID: `chen2010similarday`; legacy_core_mapped; previous: core
- [Kalman Filter and Analog Schemes to Postprocess Numerical Weather Predictions](https://journals.ametsoc.org/view/journals/mwre/139/11/2011mwr3653.1.xml) (Monthly Weather Review) — ID: `dellemonache2011kalman`; legacy_core_mapped; previous: core
- [Searching and Mining Trillions of Time Series Subsequences under Dynamic Time Warping](https://doi.org/10.1145/2339530.2339576) (KDD) — ID: `rakthanmanon2012`; legacy_contextual; previous: contextual
- [Probabilistic Weather Prediction with an Analog Ensemble](https://journals.ametsoc.org/doi/pdf/10.1175/MWR-D-12-00281.1) (Monthly Weather Review) — ID: `dellemonache2013anen`; related; previous: core
- [A novel application of an analog ensemble for short-term wind power forecasting](https://impacts.ucar.edu/en/publications/a-novel-application-of-an-analog-ensemble-for-short-term-wind-pow/) (Renewable Energy) — ID: `alessandrini2015wind`; legacy_candidate; previous: candidate
- [Pattern similarity-based methods for short-term load forecasting – Part 1: Principles](https://www.sciencedirect.com/science/article/pii/S1568494615005414) (Applied Soft Computing) — ID: `dudek2015principles`; related; previous: core
- [Pattern similarity-based methods for short-term load forecasting – Part 2: Models](https://www.sciencedirect.com/science/article/abs/pii/S1568494615004755) (Applied Soft Computing) — ID: `dudek2015models`; related; previous: core
- [Analog forecasting with dynamics-adapted kernels](https://arxiv.org/abs/1412.3831) (Nonlinearity) — ID: `zhao2016kernels`; related; previous: core
- [Matrix Profile I: All Pairs Similarity Joins for Time Series: A Unifying View That Includes Motifs, Discords and Shapelets](https://ieeexplore.ieee.org/document/7837992/) (ICDM) — ID: `yeh2016`; legacy_contextual; previous: contextual
- [On Combining Websensors and DTW Distance for kNN Time Series Forecasting](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ICPR-2016/media/files/1551.pdf) (2016 23rd International Conference on Pattern Recognition) — ID: `marcacini2016websensors`; related; previous: core
- [Pattern-based local linear regression models for short-term load forecasting](https://www.sciencedirect.com/science/article/pii/S0378779615002710) (Electric Power Systems Research) — ID: `dudek2016local`; related; previous: core
- [An Application of Similarity Search in Streaming Time Series under DTW: Online Forecasting](https://dl.acm.org/doi/10.1145/3155133.3155148) (Proceedings of the Eighth International Symposium on Information and Communication Technology, pp. 10–17) — ID: `giao2017streaming`; legacy_candidate; previous: candidate
- [The Analog Data Assimilation](https://journals.ametsoc.org/view/journals/mwre/145/10/mwr-d-16-0441.1.xml) (Monthly Weather Review) — ID: `lguensat2017anda`; legacy_contextual; previous: contextual
- [A Memory-Network Based Solution for Multivariate Time-Series Forecasting](https://arxiv.org/abs/1809.02105) (preprint) — ID: `chang2018mtnet`; core; previous: core
- [Dealing with seasonality by narrowing the training set in time series forecasting with kNN](https://www.sciencedirect.com/science/article/abs/pii/S0957417418301441) (Expert Systems with Applications) — ID: `martinez2018season`; legacy_candidate; previous: candidate
- [Distribution-Free Predictive Inference for Regression](https://www.stat.cmu.edu/~ryantibs/papers/conformal-jasa.pdf) (Journal of the American Statistical Association) — ID: `lei2018`; legacy_contextual; previous: contextual
- [Pattern matching under dynamic time warping for time series prediction](https://journal.hcmue.edu.vn/index.php/hcmuejos/article/download/146/138/0) (Ho Chi Minh City University of Education Journal of Science) — ID: `son2018dtw`; related; previous: core
- [Temporal case-based reasoning for type 1 diabetes mellitus bolus insulin decision support](https://www.sciencedirect.com/science/article/abs/pii/S0933365717300428) (Artificial Intelligence in Medicine) — ID: `brown2018bolus`; legacy_exclude; previous: exclude
- [A methodology for applying k-nearest neighbor to time series forecasting](https://link.springer.com/article/10.1007/s10462-017-9593-z) (Artificial Intelligence Review) — ID: `martinez2019methodology`; legacy_candidate; previous: candidate
- [Time Series Forecasting with KNN in R: the tsfknn Package](https://journal.r-project.org/articles/RJ-2019-004/) (The R Journal 11(2),229–242) — ID: `martinez2019tsfknn`; related; previous: core
- [Efficient and Robust Approximate Nearest Neighbor Search Using Hierarchical Navigable Small World Graphs](https://arxiv.org/abs/1603.09320) (IEEE Transactions on Pattern Analysis and Machine Intelligence) — ID: `malkov2020`; legacy_contextual; previous: contextual
- [Few-shot Learning for Time-series Forecasting](https://arxiv.org/abs/2009.14379) (preprint) — ID: `iwata2020fewshot`; core; previous: core
- [Data size considerations and hyperparameter choices in case-based reasoning approach to glucose prediction](https://www.sciencedirect.com/science/article/abs/pii/S0208521621000516) (Biocybernetics and Biomedical Engineering) — ID: `zulj2021glucose`; legacy_candidate; previous: candidate
- [Kernel Analog Forecasting: Multiscale Test Problems](https://arxiv.org/abs/2005.06623) (Multiscale Modeling & Simulation) — ID: `burov2021multiscale`; legacy_contextual; previous: contextual
- [Pattern similarity-based machine learning methods for mid-term load forecasting: A comparative study](https://arxiv.org/abs/2003.01475) (Applied Soft Computing) — ID: `dudek2021patterns`; related; previous: core
- [Prediction method on financial time series data based on matrix profile](https://www.joca.cn/EN/10.11772/j.issn.1001-9081.2020060877) (Journal of Computer Applications) — ID: `gao2021matrixprofile`; legacy_candidate; previous: candidate
- [Tight lower bounds for dynamic time warping](https://www.sciencedirect.com/science/article/pii/S0031320321000820) (Pattern Recognition) — ID: `webb2021dtwbounds`; legacy_exclude; previous: exclude
- [Learning to Remember Patterns: Pattern Matching Memory Networks for Traffic Forecasting](https://arxiv.org/abs/2110.10380) (ICLR 2022) — ID: `lee2022pmmemnet`; core; previous: core
- [MLTF: Model less time-series forecasting](https://www.sciencedirect.com/science/article/pii/S0020025522001347) (Information Sciences) — ID: `samanta2022mltf`; related; previous: core
- [Conformal Prediction for Time Series with Modern Hopfield Networks](https://arxiv.org/abs/2303.12783) (NeurIPS 2023) — ID: `auer2023hopcpt`; related; previous: core
- [Forecast evaluation for data scientists: common pitfalls and best practices](https://link.springer.com/article/10.1007/s10618-022-00894-5) (Data Mining and Knowledge Discovery) — ID: `hewamalage2023`; legacy_contextual; previous: contextual
- [Learning to Forecast Dynamical Systems from Streaming Data](https://arxiv.org/abs/2109.09703) (SIAM Journal on Applied Dynamical Systems) — ID: `giannakis2023streaming`; legacy_contextual; previous: contextual
- [Machine Learning Weather Analogs for Near-Surface Variables](https://arxiv.org/abs/2103.04530) (Boundary-Layer Meteorology) — ID: `hu2023deepanalog`; related; previous: core
- [Macroeconomic forecasting in times of crises](https://onlinelibrary.wiley.com/doi/10.1002/jae.2951) (Journal of Applied Econometrics) — ID: `guerron2023crises`; legacy_core_mapped; previous: core
- [ResMem: Learn what you can and memorize the rest](https://arxiv.org/abs/2302.01576) (NeurIPS 2023) — ID: `yang2023resmem`; legacy_contextual; previous: contextual
- [From News to Forecast: Integrating Event Analysis in LLM-Based Time Series Forecasting with Reflection](https://arxiv.org/abs/2409.17515) (NeurIPS 2024) — ID: `wang2024newsforecast`; core; previous: core
- [S2IP-LLM: Semantic Space Informed Prompt Learning with LLM for Time Series Forecasting](https://proceedings.mlr.press/v235/pan24c.html) (ICML 2024) — ID: `pan2024s2ip`; legacy_contextual; previous: contextual
- [TimeRAG: It's Time for Retrieval-Augmented Generation in Time-Series Forecasting](https://openreview.net/forum?id=GvzL4LuycW) (unverified) — ID: `xiao2024timerag_submission`; legacy_candidate; previous: candidate
- [CBR-FoX: A case-based reasoning software tool for auditing time series predictions](https://www.sciencedirect.com/science/article/pii/S2352711025004169) (SoftwareX) — ID: `perez2025cbrfox`; legacy_exclude; previous: exclude
- [Kernel-based Optimally Weighted Conformal Time-Series Prediction](https://proceedings.iclr.cc/paper_files/paper/2025/hash/058983528186511a74968e88a6d0ad63-Abstract-Conference.html) (ICLR 2025) — ID: `lee2025kowcpi`; related; previous: core
- [RATFM: Retrieval-augmented Time Series Foundation Model for Anomaly Detection](https://arxiv.org/abs/2506.02081) (preprint) — ID: `maru2025ratfm`; legacy_exclude; previous: exclude
- [Adaptive Self-Retrieval for Foundation Model Time Series Forecasting](https://github.com/masadi-99/adaptive-self-retrieval) (unverified) — ID: `asr2026repository`; legacy_candidate; previous: candidate
- [Advances in Similar Day Methods for Short-Term Load Forecasting for Power Systems](https://www.mdpi.com/2571-9394/8/2/32) (Forecasting) — ID: `similardaysurvey2026`; legacy_candidate; previous: candidate
- [A Multi-Scale CNN-Transformer Network with Residual Correction for Ultra-Short-Term Photovoltaic Power Forecasting](https://www.mdpi.com/2227-9717/14/5/759) (Processes 14(5):759) — ID: `ye2026msctrcm`; core; previous: core
- [Bridging the Last Mile of Time Series Forecasting with LLM Agents](https://arxiv.org/abs/2606.02497) (arXiv preprint) — ID: `liao2026lastmile`; core; previous: core
- [CastFSR: A Fast--Slow--Reflect Agentic Reasoning Framework for Context-Aware Time Series Forecasting](https://arxiv.org/abs/2608.03031) (arXiv preprint) — ID: `tao2026castfsr`; core; previous: core
- [CometNet: Contextual Motif-guided Long-term Time Series Forecasting](https://arxiv.org/abs/2511.08049) (Proceedings of the AAAI Conference on Artificial Intelligence) — ID: `wang2026cometnet`; legacy_contextual; previous: contextual
- [Enhancing Multivariate Time Series Forecasting with Global Temporal Retrieval](https://proceedings.iclr.cc/paper_files/paper/2026/hash/7a3284ce53f620d244fca0c79d94c478-Abstract-Conference.html) (ICLR) — ID: `cao2026gtr`; legacy_contextual; previous: contextual
- [ForecastCompass: Guiding Agentic Forecasting with Adaptive Factor Memory](https://arxiv.org/abs/2605.30858) (unverified) — ID: `chang2026forecastcompass`; legacy_exclude; previous: exclude
- [From Long News to Accurate Forecast: Importance-Aware Fusion and PRM-Guided Reflection for Time Series Forecasting](https://arxiv.org/abs/2606.03097) (arXiv preprint) — ID: `liu2026longnews`; core; previous: core
- [GlyRAG: Context-Aware Retrieval-Augmented Framework for Blood Glucose Forecasting](https://arxiv.org/abs/2601.05353) (IEEE Journal of Biomedical and Health Informatics, online ahead of print) — ID: `soumma2026glyrag`; core; previous: core
- [GNA: Granular Neighbor Assembly for Retrieval-Augmented Multivariate Time-Series Forecasting](https://arxiv.org/abs/2609.36281) (arXiv preprint) — ID: `uhse2026gna`; core_hybrid; previous: core
- [Learning the Context of Errors: Black-Box Online Adaptation of Time Series Foundation Models](https://arxiv.org/abs/2606.14222) (preprint) — ID: `dai2026orca`; legacy_contextual; previous: contextual
- [Memory Mechanisms in Multivariate Time Series: A Survey of Architectures, Retrieval, and Evolution](https://www.researchsquare.com/article/rs-10171809/v1) (preprint) — ID: `qi2026memory`; legacy_contextual; previous: contextual
- [Online spatio-temporal forecasting with retrieval-augmented orthogonal landmark transformer and masked teacher-student learning](https://www.sciencedirect.com/science/article/pii/S0893608026010853) (Neural Networks (January 2027 issue; pre-cutoff online date unverified)) — ID: `ding2026roltmtsol`; legacy_candidate; previous: candidate
- [RACE: Residual-Aware Test-Time Adaptation for Neighbor-Rich Time-Series Foundation Model Forecasting](https://arxiv.org/abs/2610.00405) (arXiv preprint) — ID: `shi2026race`; core; previous: core
- [RareCP: Regime-Aware Retrieval for Efficient Conformal Prediction](https://arxiv.org/abs/2605.08857) (preprint) — ID: `heurich2026rarecp`; related; previous: core
- [RATL: Learning from Retrieved Residuals for Robust Multivariate Time-Series Forecasting](https://arxiv.org/abs/2609.03937) (arXiv preprint) — ID: `he2026ratl`; core; previous: core
- [ResCP: Reservoir Conformal Prediction for Time Series Forecasting](https://arxiv.org/abs/2510.05060) (ICLR 2026) — ID: `neglia2026rescp`; related; previous: core
- [Retrieval-Corrected Conformal Prediction for Time Series](https://arxiv.org/abs/2608.10553) (CIKM 2026, accepted full research paper) — ID: `jin2026rccp`; related; previous: core
- [Rollcast: Proper-Score Gated Rolling Anchors for Adaptive Probabilistic Time-Series Forecasting](https://arxiv.org/abs/2609.05561) (preprint) — ID: `vercellino2026rollcast`; related; previous: core
- [Unlocking the Value of Text: Event-Driven Reasoning and Multi-Level Alignment for Time Series Forecasting](https://arxiv.org/abs/2603.15452) (ICLR 2026) — ID: `wang2026vot`; core; previous: core

## New to the previous corpus: 23 records

- [SteerCast: Retrieval-Based Latent Steering for Decoder-Only Time Series Forecasting](https://arxiv.org/abs/2610.11229) (NeurIPS 2026) — ID: `arxiv-2610.11229`; core
- [Retrieval Is Not Enough: Refreshing Memory for Frozen Time-Series Forecasters](https://arxiv.org/abs/2610.07834) (preprint) — ID: `arxiv-2610.07834`; core
- [GRAM: Correcting Frozen Time-Series Foundation Models via Graph-Retrieved Amplitude Memory](https://arxiv.org/abs/2610.04827) (preprint) — ID: `arxiv-2610.04827`; core
- [TIMBRE: Teaching Time Series Forecasters to Read, Remember, and Reconcile](https://arxiv.org/abs/2610.04795) (preprint) — ID: `arxiv-2610.04795`; core
- [SEER: Self-Evolving Event Reasoning and Retrieval for Time Series Forecasting](https://arxiv.org/abs/2610.04109) (preprint) — ID: `arxiv-2610.04109`; core
- [Dual-Context Analog Retrieval for Time Series Forecasting](https://arxiv.org/abs/2610.03491) (preprint) — ID: `arxiv-2610.03491`; core
- [When Does Retrieval Help Time-Series Forecasting?](https://arxiv.org/abs/2609.20193) (preprint) — ID: `arxiv-2609.20193`; related
- [ROAR: Retrieval Opportunity-Aware Refinement for Zero-Shot Time Series Forecasting](https://arxiv.org/abs/2605.24911) (preprint) — ID: `arxiv-2605.24911`; core
- [MemCast: Memory-Driven Time Series Forecasting with Experience-Conditioned Reasoning](https://arxiv.org/abs/2602.03164) (ICML 2026) — ID: `arxiv-2602.03164`; core
- [TimeMRA: LLM-Empowered Time Series Forecasting via Multi-Scale Retrieval-Augmented Representations](https://proceedings.mlr.press/v306/shang26b.html) (ICML 2026) — ID: `timemra`; related
- [Spectral Retrieval-Augmented Time-Series Forecasting](https://arxiv.org/abs/2606.19412) (preprint) — ID: `arxiv-2606.19412`; core
- [Retrieve the Right Signal: Decomposition-Guided Retrieval-Augmented Forecasting for Financial Markets](https://cikm2026.diag.uniroma1.it/program/) (CIKM 2026) — ID: `retrieve-the-right-signal`; pending
- [Retrieval Mechanisms Surpass Long-Context Scaling in Time Series Forecasting](https://arxiv.org/abs/2605.08217) (ICLR 2026 TSALM Workshop) — ID: `arxiv-2605.08217`; related
- [An improved retrieval-augmented long-term grouting power prediction method: Rejecting low-similarity retrievals](https://doi.org/10.1016/j.engappai.2025.112733) (Engineering Applications of Artificial Intelligence 2026) — ID: `grouting-retrieval-2026`; provisional
- [Learning from History: A Retrieval-Augmented Framework for Spatiotemporal Prediction](https://arxiv.org/abs/2510.24049) (preprint) — ID: `arxiv-2510.24049`; related
- [Retrieval-Augmented Framework with Adaptive Gating for Time Series Forecasting](https://doi.org/10.1007/s12204-025-2847-z) (Journal of Shanghai Jiaotong University (Science) 2025) — ID: `adaptive-gating-2025`; provisional
- [STRATA-TS: Selective Knowledge Transfer for Urban Time Series Forecasting with Retrieval-Guided Reasoning](https://arxiv.org/abs/2508.18635) (preprint) — ID: `arxiv-2508.18635`; core
- [FLAIRR-TS – Forecasting LLM-Agents with Iterative Refinement and Retrieval for Time Series](https://arxiv.org/abs/2508.19279) (Findings of EMNLP 2025) — ID: `arxiv-2508.19279`; core
- [A Retrieval Augmented Spatio-Temporal Framework for Traffic Prediction](https://arxiv.org/abs/2508.16623) (AAAI 2026 AI for Social Impact Track) — ID: `arxiv-2508.16623`; core
- [Retrieval-Augmented Forecasting with Tabular Time Series Data](https://aclanthology.org/2025.trl-1.16/) (ACL 2025 TRL Workshop) — ID: `raf-li-tabular`; core
- [Agentic Retrieval-Augmented Generation for Time Series Analysis](https://arxiv.org/abs/2408.14484) (KDD 2024 Undergraduate Consortium) — ID: `arxiv-2408.14484`; core
- [Towards Resolution-Aware Retrieval Augmented Zero-Shot Forecasting](https://openreview.net/forum?id=JnNCD8jEgp) (NeurIPS 2024 TSALM Workshop) — ID: `arxiv-2510.16695`; core
- [Self-adaptive Retrieval-Augmented Reinforcement Learning for Time Series Forecasting](https://openreview.net/pdf?id=1jlci3sF4Q) (preprint) — ID: `srrf`; pending

## Duplicates and non-duplicates

The eight previous duplicate source-record pairs are not eight additional papers: `martinez2018season`, `martinez2019methodology`, `gao2021matrixprofile`, `marcacini2016websensors`, `giao2017streaming`, `dudek2016local`, `samanta2022mltf`, `zulj2021glucose`.
The 28 overlapping records are merged by identity while retaining old IDs and new draft IDs. Different papers sharing a title or acronym are not merged: Han RAFT vs Tire RAF, Ning TS-RAG vs Xiao TS-RAG, and the unresolved Xiao TimeRAG submission vs Yang TimeRAG.

## Verification limits

Previous Library originals were exposed as current version 1; earlier versions were not enumerated or restored. Recovery does not assert a new full-text audit of every inherited paper. Current public-source checks and inherited evidence are labelled separately. No repository write, publication or sharing-permission change is part of this correction.
