# Recovery verification

Display sorting is described in [the ordering notes](ordering.md); source dates below remain unchanged evidence fields.

Original IDs are preserved in the data files. Evidence labelled inherited has not been newly verified as full text.

## Predicting Chaotic Time Series

- title: Predicting Chaotic Time Series
- old year: 1987
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://oms-inet.files.svdcdn.com/production/files/predictingchaotic.pdf?dm=1553075489
- evidence location: p.846
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: full_text.
- brief reason: Historical state–future neighbors train a query-local linear predictor. It generates a forecast directly rather than augmenting or correcting a separate forecast.
- reason: Historical state–future neighbors train a query-local linear predictor. It generates a forecast directly rather than augmenting or correcting a separate forecast.
- saraf category: null
- method summary: Historical state–future neighbors train a query-local linear predictor. It generates a forecast directly rather than augmenting or correcting a separate forecast.
- method source: https://oms-inet.files.svdcdn.com/production/files/predictingchaotic.pdf?dm=1553075489

## Nonlinear forecasting as a way of distinguishing chaos from measurement error in time series

- title: Nonlinear forecasting as a way of distinguishing chaos from measurement error in time series
- old year: 1990
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://care-mendoza.nd.edu/assets/152212/sugiharamay_chaos_nature_1990_copy.pdf
- evidence location: Forecasting for a chaotic time series, pp.734–736
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: methods_sections.
- brief reason: Distance-weighted simplex-neighbor successors directly produce the forecast. This is standalone local trajectory prediction.
- reason: Distance-weighted simplex-neighbor successors directly produce the forecast. This is standalone local trajectory prediction.
- saraf category: null
- method summary: Distance-weighted simplex-neighbor successors directly produce the forecast. This is standalone local trajectory prediction.
- method source: https://care-mendoza.nd.edu/assets/152212/sugiharamay_chaos_nature_1990_copy.pdf

## Lazy learning for local modelling and control design

- title: Lazy learning for local modelling and control design
- old year: 1999
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://iridia.ulb.ac.be/mbiro/paperi/BonBirBer1999ijc.pdf
- evidence location: §1–2, pp.643–646
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: methods_sections.
- brief reason: Retained input/output cases support query-local weighted linear fitting and next-step output prediction. Keep the controlled system-identification scope visible; local fitting is not zero-computation training-free inference.
- reason: Retained input/output cases support query-local weighted linear fitting and next-step output prediction. Keep the controlled system-identification scope visible; local fitting is not zero-computation training-free inference.
- saraf category: null
- method summary: Retained input/output cases support query-local weighted linear fitting and next-step output prediction. Keep the controlled system-identification scope visible; local fitting is not zero-computation training-free inference.
- method source: https://iridia.ulb.ac.be/mbiro/paperi/BonBirBer1999ijc.pdf

## Short-Term Load Forecasting: Similar Day-Based Wavelet Neural Networks

- title: Short-Term Load Forecasting: Similar Day-Based Wavelet Neural Networks
- old year: 2010
- disposition: retrieved inputs before neural model
- category: input_augmentation
- evidence source: https://www.researchgate.net/publication/224084363_Short-Term_Load_Forecasting_Similar_Day-Based_Wavelet_Neural_Networks
- evidence location: §II-B–D, pp.324–326; §III, pp.327–328
- evidence status: inherited
- evidence scope: Inherited methods audit of author manuscript §§II-B–D; fresh DOI open failed, so no fresh full-text verification is claimed.
- brief reason: The selected historical day is wavelet-decomposed and supplied to the low/high-frequency neural predictors before the forecast is generated. Historical input-augmentation antecedent.
- reason: The selected historical day is wavelet-decomposed and supplied to the low/high-frequency neural predictors before the forecast is generated. Historical input-augmentation antecedent.
- saraf category: Retrieval as Input Augmentation
- method summary: The selected historical day is wavelet-decomposed and supplied to the low/high-frequency neural predictors before the forecast is generated. Historical input-augmentation antecedent.
- method source: https://www.researchgate.net/publication/224084363_Short-Term_Load_Forecasting_Similar_Day-Based_Wavelet_Neural_Networks

## Kalman Filter and Analog Schemes to Postprocess Numerical Weather Predictions

- title: Kalman Filter and Analog Schemes to Postprocess Numerical Weather Predictions
- old year: 2011
- disposition: point-forecast output correction
- category: output_correction
- evidence source: https://www.researchgate.net/publication/258537499_Kalman_Filter_and_Analog_Schemes_to_Postprocess_Numerical_Weather_Predictions
- evidence location: §2c–f, pp.3556–3559; Eq.6–8
- evidence status: inherited
- evidence scope: Inherited methods audit §§2c–f, Eqs.6–8; publisher access returned 403 on fresh check. AN/ANKF distinction is retained explicitly.
- brief reason: Mixed-method paper: AN directly averages verifying analog observations; ANKF uses analog forecast errors in a Kalman correction to the numerical forecast. The output-correction category applies to ANKF, not every method in the paper.
- reason: Mixed-method paper: AN directly averages verifying analog observations; ANKF uses analog forecast errors in a Kalman correction to the numerical forecast. The output-correction category applies to ANKF, not every method in the paper.
- saraf category: Retrieval as Post-hoc Refinement
- method summary: Mixed-method paper: AN directly averages verifying analog observations; ANKF uses analog forecast errors in a Kalman correction to the numerical forecast. The output-correction category applies to ANKF, not every method in the paper.
- method source: https://www.researchgate.net/publication/258537499_Kalman_Filter_and_Analog_Schemes_to_Postprocess_Numerical_Weather_Predictions

## Probabilistic Weather Prediction with an Analog Ensemble

- title: Probabilistic Weather Prediction with an Analog Ensemble
- old year: 2013
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://www.researchgate.net/publication/261510260_Probabilistic_Weather_Prediction_with_an_Analog_Ensemble
- evidence location: §2b(1), Eq.2, Fig.3; pp.3502–3504
- evidence status: inherited
- evidence scope: Inherited methods audit §2b(1), Eq.2, Fig.3; publisher access returned 403 on fresh check. Later Hu primary text corroborates the AnEn mechanism but is not fresh inspection of this paper.
- brief reason: Forecast-space analog selection retrieves verifying observations that constitute a predictive ensemble; its mean can provide a point forecast. Keep as an analog probabilistic forecaster, not merely interval calibration or an additive residual corrector.
- reason: Forecast-space analog selection retrieves verifying observations that constitute a predictive ensemble; its mean can provide a point forecast. Keep as an analog probabilistic forecaster, not merely interval calibration or an additive residual corrector.
- saraf category: null
- method summary: Forecast-space analog selection retrieves verifying observations that constitute a predictive ensemble; its mean can provide a point forecast. Keep as an analog probabilistic forecaster, not merely interval calibration or an additive residual corrector.
- method source: https://www.researchgate.net/publication/261510260_Probabilistic_Weather_Prediction_with_an_Analog_Ensemble

## Pattern similarity-based methods for short-term load forecasting – Part 1: Principles

- title: Pattern similarity-based methods for short-term load forecasting – Part 1: Principles
- old year: 2015
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://gdudek.el.pcz.pl/files/SBFM_Principles_15.pdf
- evidence location: Pattern definitions and forecasting framework, author manuscript pp.3–8
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: methods_sections.
- brief reason: Similarity weights combine stored output patterns and decode them to load values. The retrieved patterns directly supply a standalone nonparametric forecast.
- reason: Similarity weights combine stored output patterns and decode them to load values. The retrieved patterns directly supply a standalone nonparametric forecast.
- saraf category: null
- method summary: Similarity weights combine stored output patterns and decode them to load values. The retrieved patterns directly supply a standalone nonparametric forecast.
- method source: https://gdudek.el.pcz.pl/files/SBFM_Principles_15.pdf

## Pattern similarity-based methods for short-term load forecasting – Part 2: Models

- title: Pattern similarity-based methods for short-term load forecasting – Part 2: Models
- old year: 2015
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://gdudek.el.pcz.pl/files/SBFM_Models_15.pdf
- evidence location: §III–V; author manuscript pp.4–13; Algorithms2–4
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: methods_sections.
- brief reason: kNN/kernel and prototype variants directly map matched input patterns to output patterns. Preserve learned-prototype caveat; the whole family is not raw-case or training-free retrieval.
- reason: kNN/kernel and prototype variants directly map matched input patterns to output patterns. Preserve learned-prototype caveat; the whole family is not raw-case or training-free retrieval.
- saraf category: null
- method summary: kNN/kernel and prototype variants directly map matched input patterns to output patterns. Preserve learned-prototype caveat; the whole family is not raw-case or training-free retrieval.
- method source: https://gdudek.el.pcz.pl/files/SBFM_Models_15.pdf

## Analog forecasting with dynamics-adapted kernels

- title: Analog forecasting with dynamics-adapted kernels
- old year: 2016
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://arxiv.org/abs/1412.3831
- evidence location: §§2–3, §6.1–6.2
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: methods_sections.
- brief reason: Dynamics-adapted kernels weight historical successor observations to form the forecast. The multiscale correction is internal to the analog estimator, not correction of an independent base forecast.
- reason: Dynamics-adapted kernels weight historical successor observations to form the forecast. The multiscale correction is internal to the analog estimator, not correction of an independent base forecast.
- saraf category: null
- method summary: Dynamics-adapted kernels weight historical successor observations to form the forecast. The multiscale correction is internal to the analog estimator, not correction of an independent base forecast.
- method source: https://arxiv.org/abs/1412.3831

## On Combining Websensors and DTW Distance for kNN Time Series Forecasting

- title: On Combining Websensors and DTW Distance for kNN Time Series Forecasting
- old year: 2016
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://www.researchgate.net/publication/316991653_On_combining_Websensors_and_DTW_distance_for_kNN_Time_Series_Forecasting
- evidence location: Author manuscript p. 2, Section II, Eq. 1
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: full_text.
- brief reason: Text-informed DTW selects historical subsequences; their observed continuations are averaged into the forecast. Preserve inherited equation/notation and experimental-selection caveats.
- reason: Text-informed DTW selects historical subsequences; their observed continuations are averaged into the forecast. Preserve inherited equation/notation and experimental-selection caveats.
- saraf category: null
- method summary: Text-informed DTW selects historical subsequences; their observed continuations are averaged into the forecast. Preserve inherited equation/notation and experimental-selection caveats.
- method source: https://www.researchgate.net/publication/316991653_On_combining_Websensors_and_DTW_distance_for_kNN_Time_Series_Forecasting

## Pattern-based local linear regression models for short-term load forecasting

- title: Pattern-based local linear regression models for short-term load forecasting
- old year: 2016
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://gdudek.el.pcz.pl/files/PattBasLinRegSTLF_15.pdf
- evidence location: §2, manuscriptpp4–5, Eqs1–3
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: full_text.
- brief reason: Same-weekday nearest daily pattern pairs form a new local training set; a fitted linear map predicts and decodes the future profile. This is retrieval-then-fit, not neural context or output correction.
- reason: Same-weekday nearest daily pattern pairs form a new local training set; a fitted linear map predicts and decodes the future profile. This is retrieval-then-fit, not neural context or output correction.
- saraf category: null
- method summary: Same-weekday nearest daily pattern pairs form a new local training set; a fitted linear map predicts and decodes the future profile. This is retrieval-then-fit, not neural context or output correction.
- method source: https://gdudek.el.pcz.pl/files/PattBasLinRegSTLF_15.pdf

## Pattern matching under dynamic time warping for time series prediction

- title: Pattern matching under dynamic time warping for time series prediction
- old year: 2018
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://journal.hcmue.edu.vn/index.php/hcmuejos/article/download/146/138/0
- evidence location: §3.2 Fig.7 pp.154–155; §4 pp.155–158
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: full_text.
- brief reason: DTW matches are selected and following windows averaged directly; recursive extension can insert previous predictions. Preserve synthetic-memory and evaluation-separation caveats.
- reason: DTW matches are selected and following windows averaged directly; recursive extension can insert previous predictions. Preserve synthetic-memory and evaluation-separation caveats.
- saraf category: null
- method summary: DTW matches are selected and following windows averaged directly; recursive extension can insert previous predictions. Preserve synthetic-memory and evaluation-separation caveats.
- method source: https://journal.hcmue.edu.vn/index.php/hcmuejos/article/download/146/138/0

## Time Series Forecasting with KNN in R: the tsfknn Package

- title: Time Series Forecasting with KNN in R: the tsfknn Package
- old year: 2019
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://journal.r-project.org/articles/RJ-2019-004/RJ-2019-004.pdf
- evidence location: §2pp229–231,Eqs1–2/Table1
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: full_text.
- brief reason: Exact nearest lag vectors supply scalar or multi-horizon targets, aggregated by mean/median/distance weights. Direct kNN forecasting, with recursive and MIMO variants, belongs in the standalone lineage.
- reason: Exact nearest lag vectors supply scalar or multi-horizon targets, aggregated by mean/median/distance weights. Direct kNN forecasting, with recursive and MIMO variants, belongs in the standalone lineage.
- saraf category: null
- method summary: Exact nearest lag vectors supply scalar or multi-horizon targets, aggregated by mean/median/distance weights. Direct kNN forecasting, with recursive and MIMO variants, belongs in the standalone lineage.
- method source: https://journal.r-project.org/articles/RJ-2019-004/RJ-2019-004.pdf

## Pattern similarity-based machine learning methods for mid-term load forecasting: A comparative study

- title: Pattern similarity-based machine learning methods for mid-term load forecasting: A comparative study
- old year: 2021
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://gdudek.el.pcz.pl/files/SMLFM_Dudek_Pelka_20.pdf
- evidence location: §2 Eq.4–9; §4; §5.3–5.4
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: full_text.
- brief reason: Matched normalized yearly patterns directly supply future shapes; historical or separately forecast scale statistics decode them. Statistical decoding does not itself make this post-hoc point-output correction.
- reason: Matched normalized yearly patterns directly supply future shapes; historical or separately forecast scale statistics decode them. Statistical decoding does not itself make this post-hoc point-output correction.
- saraf category: null
- method summary: Matched normalized yearly patterns directly supply future shapes; historical or separately forecast scale statistics decode them. Statistical decoding does not itself make this post-hoc point-output correction.
- method source: https://gdudek.el.pcz.pl/files/SMLFM_Dudek_Pelka_20.pdf

## MLTF: Model less time-series forecasting

- title: MLTF: Model less time-series forecasting
- old year: 2022
- disposition: standalone analog/local prediction
- category: null
- evidence source: https://www.sciencedirect.com/science/article/pii/S0020025522001347
- evidence location: Introduction, contributions; Section 3 preview
- evidence status: inherited
- evidence scope: Classification re-audited against preserved old record; underlying source extraction is inherited, not freshly reverified. Prior depth: methods_sections.
- brief reason: Feature-cluster peers are Fourier-resampled and projected into a cross-series forecast. Preserve the primary preview/author-account limitation: the precise aggregation estimator remains unverified.
- reason: Feature-cluster peers are Fourier-resampled and projected into a cross-series forecast. Preserve the primary preview/author-account limitation: the precise aggregation estimator remains unverified.
- saraf category: null
- method summary: Feature-cluster peers are Fourier-resampled and projected into a cross-series forecast. Preserve the primary preview/author-account limitation: the precise aggregation estimator remains unverified.
- method source: https://www.sciencedirect.com/science/article/pii/S0020025522001347

## Conformal Prediction for Time Series with Modern Hopfield Networks

- title: Conformal Prediction for Time Series with Modern Hopfield Networks
- old year: 2023
- disposition: uncertainty/calibration-only
- category: uncertainty_calibration
- evidence source: https://arxiv.org/html/2303.12783v2
- evidence location: §§1.2, 2.2–2.4; Eqs.6–8
- evidence status: fresh
- evidence scope: Method locus freshly re-read from primary source on 2026-10-15; no experiment reproduction.
- brief reason: Learned soft retrieval reweights stored signed residuals; their lower/upper quantiles are added to an existing point forecast to construct an interval. No revised point predictor is established.
- reason: Learned soft retrieval reweights stored signed residuals; their lower/upper quantiles are added to an existing point forecast to construct an interval. No revised point predictor is established.
- saraf category: null
- method summary: Learned soft retrieval reweights stored signed residuals; their lower/upper quantiles are added to an existing point forecast to construct an interval. No revised point predictor is established.
- method source: https://arxiv.org/html/2303.12783v2

## Machine Learning Weather Analogs for Near-Surface Variables

- title: Machine Learning Weather Analogs for Near-Surface Variables
- old year: 2023
- disposition: standalone analog/local prediction
- category: analog_probabilistic_forecaster
- evidence source: https://link.springer.com/article/10.1007/s10546-022-00779-6
- evidence location: §§1, 2.1–2.3
- evidence status: fresh
- evidence scope: Method locus freshly re-read from primary source on 2026-10-15; no experiment reproduction.
- brief reason: A neural network learns the similarity embedding, then historical verifying observations selected in that space form an analog ensemble. Neural retrieval geometry does not make retrieved observations inputs to a downstream neural forecaster.
- reason: A neural network learns the similarity embedding, then historical verifying observations selected in that space form an analog ensemble. Neural retrieval geometry does not make retrieved observations inputs to a downstream neural forecaster.
- saraf category: null
- method summary: A neural network learns the similarity embedding, then historical verifying observations selected in that space form an analog ensemble. Neural retrieval geometry does not make retrieved observations inputs to a downstream neural forecaster.
- method source: https://link.springer.com/article/10.1007/s10546-022-00779-6

## Macroeconomic forecasting in times of crises

- title: Macroeconomic forecasting in times of crises
- old year: 2023
- disposition: point-forecast output correction
- category: output_correction
- evidence source: https://www.ecb.europa.eu/press/conferences/shared/pdf/20170929_advances_in_short_term_forecasting/Paper_6_Guerron_Zhong.pdf
- evidence location: June2017 draft §2.1–2.4 pp.5–9
- evidence status: inherited
- evidence scope: Inherited June 2017 working-draft §2.1–2.4 audit; final journal full text was not read. Do not transfer draft numerical results into the final publication.
- brief reason: The current ARMA/ARIMA forecast is corrected by the mean residual of analogous historical blocks. Mechanistic evidence is from the 2017 working draft, not a fresh read of the final 2023 journal version.
- reason: The current ARMA/ARIMA forecast is corrected by the mean residual of analogous historical blocks. Mechanistic evidence is from the 2017 working draft, not a fresh read of the final 2023 journal version.
- saraf category: Retrieval as Post-hoc Refinement
- method summary: The current ARMA/ARIMA forecast is corrected by the mean residual of analogous historical blocks. Mechanistic evidence is from the 2017 working draft, not a fresh read of the final 2023 journal version.
- method source: https://www.ecb.europa.eu/press/conferences/shared/pdf/20170929_advances_in_short_term_forecasting/Paper_6_Guerron_Zhong.pdf

## Kernel-based Optimally Weighted Conformal Time-Series Prediction

- title: Kernel-based Optimally Weighted Conformal Time-Series Prediction
- old year: 2025
- disposition: uncertainty/calibration-only
- category: uncertainty_calibration
- evidence source: https://proceedings.iclr.cc/paper_files/paper/2025/file/058983528186511a74968e88a6d0ad63-Paper-Conference.pdf
- evidence location: §§2–3.2, Eq.3, Eqs.4–10, Algorithm 1
- evidence status: fresh
- evidence scope: Method locus freshly re-read from primary source on 2026-10-15; no experiment reproduction.
- brief reason: Residual-history blocks localize a weighted empirical distribution of successor residuals; optimized lower/upper quantiles construct an interval around the supplied point forecast.
- reason: Residual-history blocks localize a weighted empirical distribution of successor residuals; optimized lower/upper quantiles construct an interval around the supplied point forecast.
- saraf category: null
- method summary: Residual-history blocks localize a weighted empirical distribution of successor residuals; optimized lower/upper quantiles construct an interval around the supplied point forecast.
- method source: https://proceedings.iclr.cc/paper_files/paper/2025/file/058983528186511a74968e88a6d0ad63-Paper-Conference.pdf

## RareCP: Regime-Aware Retrieval for Efficient Conformal Prediction

- title: RareCP: Regime-Aware Retrieval for Efficient Conformal Prediction
- old year: 2026
- disposition: uncertainty/calibration-only
- category: uncertainty_calibration
- evidence source: https://arxiv.org/html/2605.08857v1
- evidence location: §§2.2, 3.1–3.2; Eqs.1–6, 11–16
- evidence status: fresh
- evidence scope: Method locus freshly re-read from primary source on 2026-10-15; no experiment reproduction.
- brief reason: Sparse query-conditioned experts retrieve signed calibration residuals and mix their CDFs; residual quantiles give an asymmetric interval for a fixed forecasting backbone. The target is interval efficiency, not point accuracy.
- reason: Sparse query-conditioned experts retrieve signed calibration residuals and mix their CDFs; residual quantiles give an asymmetric interval for a fixed forecasting backbone. The target is interval efficiency, not point accuracy.
- saraf category: null
- method summary: Sparse query-conditioned experts retrieve signed calibration residuals and mix their CDFs; residual quantiles give an asymmetric interval for a fixed forecasting backbone. The target is interval efficiency, not point accuracy.
- method source: https://arxiv.org/html/2605.08857v1

## ResCP: Reservoir Conformal Prediction for Time Series Forecasting

- title: ResCP: Reservoir Conformal Prediction for Time Series Forecasting
- old year: 2026
- disposition: uncertainty/calibration-only
- category: uncertainty_calibration
- evidence source: https://arxiv.org/html/2510.05060v3
- evidence location: §§3.1, 3.2; Eqs.5–12
- evidence status: fresh
- evidence scope: Method locus freshly re-read from primary source on 2026-10-15; no experiment reproduction.
- brief reason: Reservoir-state similarity reweights horizon-aligned historical residuals; resampled quantiles construct a prediction interval. Retain ResCQR as a distinct learned-readout variant, not empirical-neighbor retrieval.
- reason: Reservoir-state similarity reweights horizon-aligned historical residuals; resampled quantiles construct a prediction interval. Retain ResCQR as a distinct learned-readout variant, not empirical-neighbor retrieval.
- saraf category: null
- method summary: Reservoir-state similarity reweights horizon-aligned historical residuals; resampled quantiles construct a prediction interval. Retain ResCQR as a distinct learned-readout variant, not empirical-neighbor retrieval.
- method source: https://arxiv.org/html/2510.05060v3

## Retrieval-Corrected Conformal Prediction for Time Series

- title: Retrieval-Corrected Conformal Prediction for Time Series
- old year: 2026
- disposition: uncertainty/calibration-only
- category: uncertainty_calibration
- evidence source: https://arxiv.org/html/2608.10553v1
- evidence location: §§3.2–3.3 Eqs.6–7, Algorithm 1; §4.1 frozen-forecast protocol
- evidence status: fresh_full_text_and_official_program
- evidence scope: Method locus freshly re-read from primary source on 2026-10-15; no experiment reproduction.
- brief reason: Retrieved positive/negative residual quantiles set asymmetric interval widths, then a calibrated scalar rescales those widths. The point forecasts remain frozen; correction in the title is interval correction.
- reason: Probabilistic retrieval/calibration extension. Retains a point forecast while constructing an asymmetric interval from retrieved residuals; keep separate from strict point-forecast SARAF refinement.
- saraf category: null
- method summary: Retrieves historical one-sided residuals to create local asymmetric interval widths, then applies a calibrated scalar correction based on normalized retrieval error. The official CIKM program independently lists the exact title and all four authors.
- method source: https://arxiv.org/html/2608.10553v1
- old id: jin2026rccp
- authors: ["Sangjin Jin", "Kangmin Kim", "Junhyeong Lee", "Yongjae Lee"]
- original year: 2026
- original venue: CIKM 2026 claimed by authors; independent official acceptance unverified
- original publication status: preprint
- original urls: {"official_url": "https://arxiv.org/abs/2608.10553", "arxiv_url": "https://arxiv.org/abs/2608.10553", "code_url": "https://github.com/jinsaaang/rccp", "source_urls": ["https://arxiv.org/pdf/2608.10553v1", "https://arxiv.org/abs/2608.10553", "https://github.com/jinsaaang/rccp"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: RCCP
- known public year: 2026
- earliest verified public date: 2026-08-11
- date caveat: arXiv v1 submission; official CIKM program independently verifies acceptance as of 2026-10-15, not the original acceptance date.
- venue: CIKM 2026, accepted full research paper
- publication status: accepted_peer_reviewed
- venue verified: true
- venue url: https://cikm2026.diag.uniroma1.it/program/
- paper url: https://arxiv.org/abs/2608.10553
- doi: 10.1145/3799682.3840955
- scope qualification: Probabilistic retrieval/calibration extension. Retains a point forecast while constructing an asymmetric interval from retrieved residuals; keep separate from strict point-forecast SARAF refinement.
- method location: §3 methods; official program Full paper C16.
- evidence level: full_text_and_official_program
- code url: https://github.com/jinsaaang/rccp
- code status: official_repository_reachable_not_executed
- flags: ["Replace stale author-claim-only publication caveat with independently verified accepted CIKM 2026 full-paper status.", "The program links DOI 10.1145/3799682.3840955; DOI landing page did not load in this audit, so evidence is the official program link.", "A separate probabilistic audit worker owns final classification; this record primarily communicates updated venue evidence.", "Do not turn the conditional coverage-gap result into an unrestricted finite-sample conditional-coverage guarantee."]
- sources: ["https://arxiv.org/abs/2608.10553", "https://arxiv.org/html/2608.10553v1", "https://cikm2026.diag.uniroma1.it/program/", "https://doi.org/10.1145/3799682.3840955", "https://github.com/jinsaaang/rccp"]

## Rollcast: Proper-Score Gated Rolling Anchors for Adaptive Probabilistic Time-Series Forecasting

- title: Rollcast: Proper-Score Gated Rolling Anchors for Adaptive Probabilistic Time-Series Forecasting
- old year: 2026
- disposition: boundary/unresolved
- category: probabilistic_residual_density_forecaster
- evidence source: https://arxiv.org/html/2609.05561v1
- evidence location: §§2–4 Eqs.5–14; §§6–7; §10
- evidence status: fresh
- evidence scope: Method locus freshly re-read from primary source on 2026-10-15; no experiment reproduction.
- brief reason: Retain an explicit probabilistic boundary: nearest-state residual distributions perturb rolling anchors, a proper-score gate mixes component densities, and particles generate multi-step predictive distributions. It is more than calibration-only and is not established as a plug-in point-forecast correction.
- reason: Retain an explicit probabilistic boundary: nearest-state residual distributions perturb rolling anchors, a proper-score gate mixes component densities, and particles generate multi-step predictive distributions. It is more than calibration-only and is not established as a plug-in point-forecast correction.
- saraf category: null
- method summary: Retain an explicit probabilistic boundary: nearest-state residual distributions perturb rolling anchors, a proper-score gate mixes component densities, and particles generate multi-step predictive distributions. It is more than calibration-only and is not established as a plug-in point-forecast correction.
- method source: https://arxiv.org/html/2609.05561v1

## From News to Forecast: Integrating Event Analysis in LLM-Based Time Series Forecasting with Reflection

- old id: wang2024newsforecast
- title: From News to Forecast: Integrating Event Analysis in LLM-Based Time Series Forecasting with Reflection
- authors: ["Xinlei Wang", "Maike Feng", "Jing Qiu", "Jinjin Gu", "Junhua Zhao"]
- original year: 2024
- original venue: NeurIPS 2024
- original publication status: peer_reviewed
- original urls: {"official_url": "https://proceedings.neurips.cc/paper_files/paper/2024/hash/6aef8bffb372096ee73d98da30119f89-Abstract-Conference.html", "arxiv_url": null, "code_url": "https://github.com/ameliawong1996/From_News_to_Forecast", "source_urls": ["https://proceedings.neurips.cc/paper_files/paper/2024/file/6aef8bffb372096ee73d98da30119f89-Paper-Conference.pdf"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: From News to Forecast
- known public year: 2024
- earliest verified public date: 2024-09-26
- date caveat: arXiv v1 submission date; earlier anonymous/public venue posting not established in this audit.
- venue: NeurIPS 2024
- publication status: peer_reviewed
- venue verified: true
- venue url: https://proceedings.neurips.cc/paper_files/paper/2024/hash/6aef8bffb372096ee73d98da30119f89-Abstract-Conference.html
- paper url: https://arxiv.org/abs/2409.17515
- arxiv id: 2409.17515
- saraf category: Retrieval as Input Augmentation
- scope qualification: External-document retrieval; not numeric nearest-neighbor matching.
- method summary: Selects date-, horizon- and geography-relevant articles from a crawled news pool, filters them with an LLM agent, and places selected evidence in the forecasting prompt. The numerical forecaster is LoRA-fine-tuned; error-driven reflection refines filtering using historical validation outcomes.
- method source: https://proceedings.neurips.cc/paper_files/paper/2024/file/6aef8bffb372096ee73d98da30119f89-Paper-Conference.pdf
- method location: Sections 3.1–3.3; especially news pre-pairing and filtering in §3.2, pp. 5–6.
- evidence level: full_text
- code url: https://github.com/daydreamer-amelia/From_News_to_Forecast
- code status: official_repository_reachable_not_executed
- flags: ["Add previously missing arXiv identity 2409.17515.", "Old GitHub URL redirects to the new owner name; preserve the old URL as an alias.", "Do not describe this as training-free or as test-target-driven online reflection.", "Document publication/availability times remain a separate leakage audit from numeric chronological splits."]
- sources: ["https://arxiv.org/abs/2409.17515", "https://proceedings.neurips.cc/paper_files/paper/2024/hash/6aef8bffb372096ee73d98da30119f89-Abstract-Conference.html", "https://proceedings.neurips.cc/paper_files/paper/2024/file/6aef8bffb372096ee73d98da30119f89-Paper-Conference.pdf", "https://github.com/daydreamer-amelia/From_News_to_Forecast"]
- evidence status: fresh_full_text
- reason: External-document retrieval; not numeric nearest-neighbor matching.

## A Multi-Scale CNN-Transformer Network with Residual Correction for Ultra-Short-Term Photovoltaic Power Forecasting

- old id: ye2026msctrcm
- title: A Multi-Scale CNN-Transformer Network with Residual Correction for Ultra-Short-Term Photovoltaic Power Forecasting
- authors: ["Xiao Ye", "Jun Yin", "Jiajia Zhang", "Anping Li", "Zhibo Liu", "Bin Chen", "Jingyao Yang", "Shilei Li", "Hongmei Li"]
- original year: 2026
- original venue: Processes14(5):759
- original publication status: peer_reviewed
- original urls: {"official_url": "https://www.mdpi.com/2227-9717/14/5/759", "arxiv_url": null, "code_url": null, "source_urls": ["https://www.mdpi.com/2227-9717/14/5/759/pdf", "https://www.mdpi.com/2227-9717/14/5/759/notes"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: MSCT-RCM
- known public year: 2026
- earliest verified public date: 2026-02-26
- date caveat: Publisher version-of-record date. Publisher notes separately list HTML update 2026-09-03.
- venue: Processes 14(5):759
- publication status: peer_reviewed
- venue verified: true
- venue url: https://www.mdpi.com/2227-9717/14/5/759
- paper url: https://www.mdpi.com/2227-9717/14/5/759
- doi: 10.3390/pr14050759
- saraf category: Retrieval as Post-hoc Refinement
- scope qualification: Output-side residual correction; the complete architecture is jointly optimized, so this is not a frozen-backbone/training-free plug-in.
- method summary: At test time, cosine KNN over a train-only feature/residual library selects five historical full-horizon residual sequences. Their similarity-weighted average feeds a learned residual correction module together with the baseline prediction; the correction is added to the numerical forecast.
- method source: https://www.mdpi.com/2227-9717/14/5/759
- method location: §2.3, Eq. 14 and residual fusion; final output Eq. 23; §3.2 Phase II joint training.
- evidence level: publisher_full_text_indexed_excerpts
- code url: null
- code status: no_official_code_link_verified_in_this_audit
- flags: ["Publisher direct fetch was rate-limited; title, authors, DOI, date and detailed KNN text were verified from indexed primary publisher content.", "Single historical residual sequence refers to the fused length-H sequence, not K=1; K=5 is documented.", "Phase II jointly optimizes backbone and correction module; pretraining initialization must not be misread as a permanently frozen backbone."]
- sources: ["https://www.mdpi.com/2227-9717/14/5/759", "https://www.mdpi.com/2227-9717/14/5/759/notes"]
- evidence status: fresh_publisher_full_text_indexed_excerpts
- reason: Output-side residual correction; the complete architecture is jointly optimized, so this is not a frozen-backbone/training-free plug-in.

## Bridging the Last Mile of Time Series Forecasting with LLM Agents

- old id: liao2026lastmile
- title: Bridging the Last Mile of Time Series Forecasting with LLM Agents
- authors: ["Yuhua Liao", "Zetian Wang", "Qiangqiang Nie", "Zhenhua Zhang"]
- original year: 2026
- original venue: arXiv preprint
- original publication status: preprint
- original urls: {"official_url": "https://arxiv.org/abs/2606.02497", "arxiv_url": "https://arxiv.org/abs/2606.02497", "code_url": null, "source_urls": ["https://arxiv.org/html/2606.02497v1"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: Last-mile forecasting
- known public year: 2026
- earliest verified public date: 2026-06-01
- date caveat: arXiv v1 submission date; no earlier public date established.
- venue: arXiv preprint
- publication status: preprint
- venue verified: false
- paper url: https://arxiv.org/abs/2606.02497
- saraf category: Retrieval as Post-hoc Refinement
- scope qualification: Agentic/context-evidence boundary: tool retrieval and memory retrieval revise an already-generated baseline; not a conventional numeric kNN wrapper.
- method summary: An agent reads prior-year analogs, calendar and event evidence, and stored outcome-grounded reflection memories. It applies constrained add/multiply/clip or point overrides to a separate editable forecast while retaining the original baseline. Later sessions retrieve memories only after previous outcomes are observed.
- method source: https://arxiv.org/html/2606.02497v1
- method location: §§3, 4.3–4.6; §5.5 with-memory versus no-memory case study.
- evidence level: full_text
- code url: null
- code status: no_official_code_link_verified_in_this_audit
- flags: ["Evidence is case-study scale on one domestic-air-route ticket-sales series, not a broad benchmark validation.", "The paper keyword ICML does not establish conference acceptance.", "Retain as core under general inference-augmentation scope, explicitly flagging the agentic boundary."]
- sources: ["https://arxiv.org/abs/2606.02497", "https://arxiv.org/html/2606.02497v1"]
- evidence status: fresh_full_text
- reason: Agentic/context-evidence boundary: tool retrieval and memory retrieval revise an already-generated baseline; not a conventional numeric kNN wrapper.

## CastFSR: A Fast--Slow--Reflect Agentic Reasoning Framework for Context-Aware Time Series Forecasting

- old id: tao2026castfsr
- title: CastFSR: A Fast--Slow--Reflect Agentic Reasoning Framework for Context-Aware Time Series Forecasting
- authors: ["Xiaoyu Tao", "Mingyue Cheng", "Bokai Pan", "Chuang Jiang", "Huanjian Zhang", "Tian Gao", "Yaguo Liu", "Qi Liu", "Enhong Chen"]
- original year: 2026
- original venue: arXiv preprint
- original publication status: preprint
- original urls: {"official_url": "https://arxiv.org/abs/2608.03031", "arxiv_url": "https://arxiv.org/abs/2608.03031", "code_url": "https://github.com/Xiaoyu-Tao/CastFSR", "source_urls": ["https://arxiv.org/html/2608.03031v2"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: CastFSR
- known public year: 2026
- earliest verified public date: 2026-08-04
- date caveat: arXiv v1 submission date; current v2 is 2026-08-11.
- venue: arXiv preprint
- publication status: preprint
- venue verified: false
- paper url: https://arxiv.org/abs/2608.03031
- saraf category: Retrieval as Post-hoc Refinement
- scope qualification: Agentic/context-evidence boundary: adaptive contextual-range selection and tool access rather than nearest-neighbor analog retrieval.
- method summary: Fast thinking creates a numerical forecast prior. Slow reasoning chooses context-specific look-back windows, retrieves horizon-aligned evidence from contextual histories or future-known resources, then revises selected forecast regions. Reflection checks temporal and domain consistency.
- method source: https://arxiv.org/html/2608.03031v2
- method location: Sequential formulation and Slow Deliberative Reasoning, Eq. 5; contextual resources and adaptive retrieval windows.
- evidence level: full_text
- code url: https://github.com/Xiaoyu-Tao/CastFSR
- code status: official_repository_reachable_not_executed
- flags: ["Core only under the broad operational definition of inference-time evidence retrieval; mark the distinction from retrieval of stored context/future examples.", "Separate CastFSR-Zero training-free orchestration from CastFSR-R1 SFT/RL training.", "Future-known context must actually be available at the forecast origin; target-blind wording is not by itself proof of operational data vintages."]
- sources: ["https://arxiv.org/abs/2608.03031", "https://arxiv.org/html/2608.03031v2", "https://github.com/Xiaoyu-Tao/CastFSR"]
- evidence status: fresh_full_text
- reason: Agentic/context-evidence boundary: adaptive contextual-range selection and tool access rather than nearest-neighbor analog retrieval.

## From Long News to Accurate Forecast: Importance-Aware Fusion and PRM-Guided Reflection for Time Series Forecasting

- old id: liu2026longnews
- title: From Long News to Accurate Forecast: Importance-Aware Fusion and PRM-Guided Reflection for Time Series Forecasting
- authors: ["Mingyang Liu", "Qingcan Kang", "Yuke Wang", "Shixiong Kai", "Kaichao Liang", "Hui-Ling Zhen", "Tao Zhong", "Mingxuan Yuan", "Linqi Song"]
- original year: 2026
- original venue: arXiv preprint
- original publication status: preprint
- original urls: {"official_url": "https://arxiv.org/abs/2606.03097", "arxiv_url": "https://arxiv.org/abs/2606.03097", "code_url": null, "source_urls": ["https://arxiv.org/html/2606.03097v1"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: Long News / Reward-Fusion + PRM
- known public year: 2026
- earliest verified public date: 2026-06-02
- date caveat: arXiv v1 submission date; no later version listed.
- venue: arXiv preprint
- publication status: preprint
- venue verified: false
- paper url: https://arxiv.org/abs/2606.03097
- saraf category: Retrieval as Input Augmentation
- scope qualification: External-news retrieval and compressed prompt conditioning; distinguish the actual test pipeline from offline reflection.
- method summary: The methods describe a test-time pipeline that uses frozen filtering logic to retrieve news, importance-aware compression/fusion to make a compact context, and an LLM to generate the forecast. Ground-truth error-conditioned supplementary retrieval and PRM scoring belong to offline refinement.
- method source: https://arxiv.org/html/2606.03097v1
- method location: §§3.1, 3.3, 3.6; inconsistent sentence in §4.1 Data preparation.
- evidence level: full_text_with_internal_inconsistency
- code url: null
- code status: no_official_code_link_verified_in_this_audit
- flags: ["Internal inconsistency: §§3.3/3.6 explicitly exclude PRM scoring/reflection at inference; §4.1 says PRM guides a search at inference. Record the discrepancy instead of silently resolving it.", "Inference-time news selection is clear enough for inclusion, but online PRM claims are not reliable without clarification.", "Not training-free: forecasting and auxiliary reward/compression modules are trained offline."]
- sources: ["https://arxiv.org/abs/2606.03097", "https://arxiv.org/html/2606.03097v1"]
- evidence status: fresh_full_text_with_internal_inconsistency
- reason: External-news retrieval and compressed prompt conditioning; distinguish the actual test pipeline from offline reflection.

## GlyRAG: Context-Aware Retrieval-Augmented Framework for Blood Glucose Forecasting

- old id: soumma2026glyrag
- title: GlyRAG: Context-Aware Retrieval-Augmented Framework for Blood Glucose Forecasting
- authors: ["Shovito Barua Soumma", "Hassan Ghasemzadeh"]
- original year: 2026
- original venue: IEEE Journal of Biomedical and Health Informatics, early access
- original publication status: peer_reviewed
- original urls: {"official_url": "https://doi.org/10.1109/JBHI.2026.3737468", "arxiv_url": "https://arxiv.org/abs/2601.05353", "code_url": null, "source_urls": ["https://arxiv.org/html/2601.05353v3", "https://api.crossref.org/works/10.1109/JBHI.2026.3737468"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: GlyRAG
- known public year: 2026
- earliest verified public date: 2026-01-08
- date caveat: arXiv v1 submission; journal online-ahead-of-print date is 2026-09-28. Latest arXiv v3 is 2026-09-23.
- venue: IEEE Journal of Biomedical and Health Informatics, online ahead of print
- publication status: peer_reviewed
- venue verified: true
- venue url: https://pubmed.ncbi.nlm.nih.gov/42804391/
- paper url: https://arxiv.org/abs/2601.05353
- doi: 10.1109/JBHI.2026.3737468
- saraf category: Retrieval as Input Augmentation
- scope qualification: Representation/cross-attention augmentation before the forecast head.
- method summary: A pretrained multimodal encoder represents a glucose window and its CGM-only language summary. Test queries retrieve three cosine-nearest same-participant training episodes. Cross-attention uses neighbor embeddings, then an adapter and forecast head combine query and retrieval features.
- method source: https://arxiv.org/html/2601.05353v3
- method location: §III-E, Eqs. 6–8 and inference algorithm; §IV-B training-only same-participant index.
- evidence level: full_text
- code url: null
- code status: no_official_code_link_verified_in_this_audit
- flags: ["Keep arXiv and journal as one paper. PubMed confirms title, both authors, DOI and 2026-09-28 publication date; author lab page independently lists the journal.", "The database stores outcomes, but shown cross-attention values are neighbor embeddings; do not claim raw retrieved future values are directly averaged.", "Retrospective personalized experiments do not establish prospective clinical utility or cross-participant retrieval."]
- sources: ["https://arxiv.org/abs/2601.05353", "https://arxiv.org/html/2601.05353v3", "https://pubmed.ncbi.nlm.nih.gov/42804391/", "https://ghasemzadeh.com/publication/shovito-2026-glyrag/", "https://doi.org/10.1109/JBHI.2026.3737468"]
- evidence status: fresh_full_text
- reason: Representation/cross-attention augmentation before the forecast head.

## GNA: Granular Neighbor Assembly for Retrieval-Augmented Multivariate Time-Series Forecasting

- old id: uhse2026gna
- title: GNA: Granular Neighbor Assembly for Retrieval-Augmented Multivariate Time-Series Forecasting
- authors: ["Vincent Uhse"]
- original year: 2026
- original venue: arXiv; review venue not established
- original publication status: under_review
- original urls: {"official_url": "https://arxiv.org/abs/2609.36281", "arxiv_url": "https://arxiv.org/abs/2609.36281", "code_url": null, "source_urls": ["https://arxiv.org/pdf/2609.36281v1", "https://arxiv.org/abs/2609.36281"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: GNA
- known public year: 2026
- earliest verified public date: 2026-09-28
- date caveat: arXiv v1 submission date.
- venue: arXiv preprint
- publication status: preprint
- venue verified: false
- paper url: https://arxiv.org/abs/2609.36281
- saraf category: null
- scope qualification: Core hybrid: explicit retrieved-future output mixture plus neighbor-feature cross-attention. A single strict SARAF two-way label would hide this combination.
- method summary: Retrieves causally available historical windows through learned embeddings, assembling both coherent whole-window futures and per-variate futures. A step/variate gate mixes retrieved futures and persistence, a scaled backbone forecast is added, and a separate cross-attention branch conditions on neighbor futures.
- method source: https://arxiv.org/html/2609.36281v1
- method location: §§3.1–3.5, especially Eq. 5; bank eligibility s ≤ t − max(L,H).
- evidence level: full_text
- code url: null
- code status: no_official_code_link_verified_in_this_audit
- flags: ["Old under_review status is not established by the current arXiv metadata or HTML; retain old status in provenance but present conservatively as preprint.", "Not training-free: retriever and forecaster/gates are trained.", "The base sees the usual lookback, but feature cross-attention is still part of the full predictor; not pure frozen-output post-processing."]
- sources: ["https://arxiv.org/abs/2609.36281", "https://arxiv.org/html/2609.36281v1"]
- evidence status: fresh_full_text
- reason: Core hybrid: explicit retrieved-future output mixture plus neighbor-feature cross-attention. A single strict SARAF two-way label would hide this combination.

## RACE: Residual-Aware Test-Time Adaptation for Neighbor-Rich Time-Series Foundation Model Forecasting

- old id: shi2026race
- title: RACE: Residual-Aware Test-Time Adaptation for Neighbor-Rich Time-Series Foundation Model Forecasting
- authors: ["Hao-Nan Shi", "Tong Wu", "Chen-Cong Sun", "Yuan Jiang", "Han-Jia Ye", "De-Chuan Zhan"]
- original year: 2026
- original venue: null
- original publication status: preprint
- original urls: {"official_url": "https://arxiv.org/abs/2610.00405", "arxiv_url": "https://arxiv.org/abs/2610.00405", "code_url": null, "source_urls": ["https://arxiv.org/pdf/2610.00405v1", "https://arxiv.org/abs/2610.00405"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: RACE
- known public year: 2026
- earliest verified public date: 2026-09-30
- date caveat: arXiv v1 submission is 2026-09-30 despite identifier beginning 2610; do not infer October 1 from the ID.
- venue: arXiv preprint
- publication status: preprint
- venue verified: false
- paper url: https://arxiv.org/abs/2610.00405
- saraf category: Retrieval as Post-hoc Refinement
- scope qualification: Explicit output-side correction of frozen TSFM forecasts.
- method summary: Retrieves query-compatible outcome-observed neighbors, transfers scale-aligned model-specific residuals, and aggregates coherent residual evidence. RACE-TF applies the training-free proposal; full RACE uses a fitted gate to apply or abstain. The same additive correction shifts every quantile.
- method source: https://arxiv.org/html/2610.00405v1
- method location: §§3.2–3.3, §4 residual evidence/gating; information boundary Eq. 2.
- evidence level: full_text
- code url: null
- code status: no_official_code_link_verified_in_this_audit
- flags: ["Do not call full RACE training-free: the Gate is domain-trained.", "Preserving quantile order and spread does not itself recalibrate interval width.", "Backbone-specific residual pools are necessary even when a gate transfers across backbones."]
- sources: ["https://arxiv.org/abs/2610.00405", "https://arxiv.org/html/2610.00405v1"]
- evidence status: fresh_full_text
- reason: Explicit output-side correction of frozen TSFM forecasts.

## RATL: Learning from Retrieved Residuals for Robust Multivariate Time-Series Forecasting

- old id: he2026ratl
- title: RATL: Learning from Retrieved Residuals for Robust Multivariate Time-Series Forecasting
- authors: ["Yuchen He", "Yueyang Cang", "Zhiyuan Ning", "Ningyu Wang", "Li Shi"]
- original year: 2026
- original venue: null
- original publication status: preprint
- original urls: {"official_url": "https://arxiv.org/abs/2609.03937", "arxiv_url": "https://arxiv.org/abs/2609.03937", "code_url": null, "source_urls": ["https://arxiv.org/pdf/2609.03937v1", "https://arxiv.org/abs/2609.03937"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: RATL
- known public year: 2026
- earliest verified public date: 2026-09-03
- date caveat: arXiv v1 submission date.
- venue: arXiv preprint
- publication status: preprint
- venue verified: false
- paper url: https://arxiv.org/abs/2609.03937
- saraf category: Retrieval as Post-hoc Refinement
- scope qualification: Learned output-side residual routing over a frozen backbone.
- method summary: A frozen forecaster supplies keys and model-specific signed residual trajectories in train-only memory. At inference, per-variable top-K search enforces causal availability with an extra horizon gap. A learned set-aware block/variable router combines residuals and a zero candidate; a validation-selected strength scales the additive correction.
- method source: https://arxiv.org/html/2609.03937v1
- method location: Method: Train-Only Residual Memory; Per-Variable Top-K Search; Eqs. 2–6 and J5 router.
- evidence level: full_text
- code url: null
- code status: no_official_code_link_verified_in_this_audit
- flags: ["The full RATL router is learned; only the Direct residual-averaging control is parameter-free after base fitting.", "Memory is base-specific and must be rebuilt after changing the forecaster.", "ArXiv abstract has malformed punctuation/accidental URL parsing; the canonical title and author identity are nevertheless consistent in full text."]
- sources: ["https://arxiv.org/abs/2609.03937", "https://arxiv.org/html/2609.03937v1"]
- evidence status: fresh_full_text
- reason: Learned output-side residual routing over a frozen backbone.

## Unlocking the Value of Text: Event-Driven Reasoning and Multi-Level Alignment for Time Series Forecasting

- old id: wang2026vot
- title: Unlocking the Value of Text: Event-Driven Reasoning and Multi-Level Alignment for Time Series Forecasting
- authors: ["Siyuan Wang", "Peng Chen", "Yihang Wang", "Wanghui Qiu", "Chenjuan Guo", "Bin Yang", "Yang Shu"]
- original year: 2026
- original venue: ICLR 2026
- original publication status: peer_reviewed
- original urls: {"official_url": "https://proceedings.iclr.cc/paper_files/paper/2026/hash/34a1fc7890141f1ada3d8bc6199cce07-Abstract-Conference.html", "arxiv_url": "https://arxiv.org/abs/2603.15452", "code_url": "https://github.com/decisionintelligence/VoT", "source_urls": ["https://arxiv.org/html/2603.15452v1"]}
- preserve original record: true
- identity verified: true
- authors list complete: true
- checked on: 2026-10-15
- inference retrieval: true
- not in today draft: true
- classification is audit inference: true
- acronym: VoT
- known public year: 2026
- earliest verified public date: 2026-03-16
- date caveat: Earliest verified authored arXiv submission in this audit; an earlier anonymous OpenReview posting may exist and was not established.
- venue: ICLR 2026
- publication status: peer_reviewed
- venue verified: true
- venue url: https://proceedings.iclr.cc/paper_files/paper/2026/hash/34a1fc7890141f1ada3d8bc6199cce07-Abstract-Conference.html
- paper url: https://arxiv.org/abs/2603.15452
- saraf category: Retrieval as Input Augmentation
- scope qualification: Retrieves error-corrected reasoning text into an event-forecast prompt, not numerical residuals as a final output correction.
- method summary: Training examples are summarized and their reasoning corrected using historical ground truth. At inference, semantic similarity retrieves one stored correction into the reasoning prompt. This event-driven numerical forecast is later fused with a numerical/endogenous-text branch through learned frequency weighting.
- method source: https://arxiv.org/html/2603.15452v1
- method location: §3.3.2, Knowledge Base Construction and Retrieval-Guided Prediction, Eqs. 3–6; §3.4.
- evidence level: full_text
- code url: https://github.com/decisionintelligence/VoT
- code status: official_repository_reachable_not_executed
- flags: ["Official proceedings abbreviate one author as Guo; the arXiv paper and official ICLR slides supply full name Chenjuan Guo. Preserve the complete seven-author list.", "Retrieved error-informed text does not make the mechanism output-residual refinement.", "No task-specific LLM fine-tuning does not imply the complete forecasting architecture is training-free."]
- sources: ["https://arxiv.org/abs/2603.15452", "https://arxiv.org/html/2603.15452v1", "https://proceedings.iclr.cc/paper_files/paper/2026/hash/34a1fc7890141f1ada3d8bc6199cce07-Abstract-Conference.html", "https://iclr.cc/media/iclr-2026/Slides/10011937.pdf", "https://github.com/decisionintelligence/VoT"]
- evidence status: fresh_full_text
- reason: Retrieves error-corrected reasoning text into an event-forecast prompt, not numerical residuals as a final output correction.

## A Memory-Network Based Solution for Multivariate Time-Series Forecasting

- saraf category: Retrieval as Input Augmentation
- disposition: recovered_core
- earliest verified public date: 2018-09-06
- known public year: 2018
- venue: preprint
- venue url: null
- evidence status: fresh_full_text
- method source: https://arxiv.org/html/1809.02105v1#S2.SS2
- method summary: Section 2.2 encodes non-overlapping historical blocks as memory. Query-dependent attention weights memory values; their concatenation with the query representation feeds the forecast layer. The parallel autoregressive branch is not retrieval-based output correction.
- reason: The prior catalogue omitted a genuine historical memory/input-augmentation predecessor. Joint training does not remove its inference-time retrieval.

## Few-shot Learning for Time-series Forecasting

- saraf category: Retrieval as Input Augmentation
- disposition: recovered_core
- earliest verified public date: 2020-09-30
- known public year: 2020
- venue: preprint
- venue url: null
- evidence status: fresh_full_text
- method source: https://arxiv.org/html/2009.14379v1#S3.SS1
- method summary: Section 3.1 attends from the causal query state to bidirectionally encoded support sequences. The retrieved weighted support representation is concatenated with the query state before next-step prediction.
- reason: A few-shot support-memory predecessor, recovered under broad representation augmentation. Complete support-series availability must be distinguished from a strictly chronological online deployment.

## Learning to Remember Patterns: Pattern Matching Memory Networks for Traffic Forecasting

- saraf category: Retrieval as Input Augmentation
- disposition: recovered_core
- earliest verified public date: 2021-10-20
- known public year: 2021
- venue: ICLR 2022
- venue url: https://openreview.net/pdf/3d2d0f8c044b58b34cdb6d2a91fcf86fc3792cae.pdf
- evidence status: fresh_full_text
- method source: https://arxiv.org/html/2110.10380v2#S3
- method summary: Sections 3.2–3.3 cluster training traffic patterns into keys and retrieve learned value memories by matching the current input. Graph-convolutional memory and the decoder use those retrieved representations before the prediction.
- reason: A genuine memory-augmented traffic forecasting predecessor; learned memory values are not copied empirical future trajectories. First public year is 2021; original 2022 is the ICLR publication year.

