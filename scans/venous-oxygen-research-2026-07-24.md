# Daily Venous Oxygen Research Scan — 2026-07-24

**Scope:** (1) Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous oxygenation); (2) Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI).
**Ranking axis:** relevance to **non-invasive VENOUS** (not arterial) blood oxygen. Tissue-level StO₂/VO₂ work is flagged as such; arterial-only work is included only when its technique is directly transferable to venous, and the reason is stated.

---

## ⚠️ Read this first — day summary

This is a **low-volume niche**, and today's multi-angle sweep confirms it again. Across photoacoustic/optoacoustic oximetry, jugular/central-venous NIRS, diffuse-optical/DOT, hyperspectral, visible-light OCT, SFDI, wearable pulsatile spectroscopy, and the MRI reference, most results re-surface papers already catalogued in prior dated files.

**Two genuinely new items surfaced this cycle** (neither appears in any prior scan):

- **★ NEW — MC-PAT** (Gong et al., *Applied Physics Letters*, **Oct 2025**): Monte-Carlo–enhanced quantitative photoacoustic tomography that reports **explicit in-vivo venous sO₂ (74.5 ± 1.3 %)** alongside arterial (97.8 ± 0.8 %). This is the strongest new Topic-2 entry and the most directly venous-relevant new primary paper found today. → §2.2
- **★ NEW — Transabdominal fetal oximetry via diffuse optics** (Qian et al., arXiv/TechRxiv/PMC, **Sept 2025**): deep-tissue (through thick maternal abdomen) diffuse-optics pulsatile oximetry with a novel Exponential Pulsation Ratio feature and multi-detector ML fusion. It targets **fetal arterial** SpO₂, *not* venous — included in Topic 2 strictly as a **transferable deep-tissue diffuse-optics technique**, with an honest low venous-specific score. → §2.4

**No new Topic-1 (venous-specific SvO₂/ScvO₂) primary study surfaced today.** The Topic-1 top-5 below are the standing previously-surfaced anchors, each flagged, reported with honest scores. The core gap the series tracks — **truly non-invasive human deep-vein optical SvO₂ validated at clinical scale** — remains open and is not advanced by anything published today.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

> **Sparseness note:** No brand-new venous-specific Topic-1 primary paper appeared this cycle. The five entries are the established corpus, each carried forward with a "previously surfaced" flag and an honest relevance score.

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins  *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** J. M. May, et al. (Loughborough / jugular optical-sensing group)
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter), Proc. cdbme-2024-2072
- **Link / DOI:** https://www.degruyterbrill.com/document/doi/10.1515/cdbme-2024-2072/html · DOI 10.1515/cdbme-2024-2072
- **Relevance:** 9/10 (true, vessel-specific, non-invasive SvO₂; still proof-of-concept, n=3)
- **Novelty:** A pulse-oximeter-like optical sensor that isolates the external jugular vein waveform and estimates SvO₂ non-invasively, continuously, at a superficial deep-vein target — returning values in the healthy 60–90 % band.
- **Integration insights:** The clearest demonstration that a *simple, wearable-style optical* front-end (not a large PA/US or MRI system) can reach a venous target. Its unresolved need — calibration/validation against blood-gas co-oximetry — defines the translational bottleneck for the whole optical-venous program.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models  *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV NIRS + DNN + Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** 8/10 (tracks *changes* in SijvO₂, a deep venous target; model-based, not absolute)
- **Novelty:** Multi-channel NIRS whose reflectance→ΔSijvO₂ mapping is learned by a DNN trained on **subject-specific 3-D Monte-Carlo** photon-transport models — a personalised forward model rather than a population calibration.
- **Integration insights:** The subject-specific Monte-Carlo + DNN pattern is the methodological sibling of today's new MC-PAT (§2.2): both use rigorous light-transport modelling to make deep-tissue oximetry quantitative. Cross-modality convergence on Monte-Carlo fluence correction is the through-line of the field.

### 1.3 — A New Noninvasive Method for the Assessment of Central Venous Oxygen Saturation in Critically Ill Patients (Mespere VO100 jugular NIRS)  *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** (jugular NIRS / VO100 clinical group)
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia*, S1053-0770(23)00782-6
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PMID 37827917
- **Relevance:** 8/10 (clinical ScvO₂ surrogate via transcutaneous jugular NIRS)
- **Novelty:** Clinical validation of transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂ sampling, with strong linear correlation reported in COVID-19 and post-transplant cohorts.
- **Integration insights:** The commercial/clinical anchor of the venous-NIRS route — the reference point any new optical or optoacoustic venous device must beat on bias and continuous-monitoring capability.

### 1.4 — Noninvasive Tracking of Mixed Venous Oxygen Saturation via NIRS Cerebral Oximetry  *(previously surfaced — standing corpus)*
- **Authors:** (retrospective observational cohort)
- **Year / Venue:** 2023 · *Scientific Reports* 13, s41598-023-49078-1
- **Link / DOI:** https://www.nature.com/articles/s41598-023-49078-1 · PMC10709586
- **Relevance:** 6/10 (tracks *mixed venous* SvO₂ via a cerebral-oximetry surrogate — trend, not absolute vessel read)
- **Novelty:** Demonstrates that cerebral-oximetry NIRS trends can follow mixed venous SvO₂ in a real clinical cohort, extending the venous-surrogate concept beyond the jugular.
- **Integration insights:** Reinforces that NIRS captures a **mixed arterial+venous+capillary** compartment; the venous signal must be disentangled (pulsatility gating, venous-occlusion, or vessel-resolved imaging) to become a true SvO₂ read — the recurring limitation across Topic 1.

### 1.5 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂)  *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** (heart-failure iSvO₂ modelling group)
- **Year / Venue:** 2024/2025 · heart-failure clinical literature
- **Link / DOI:** (see scan 07-07 §1.1 for full metadata) *(venue/DOI not re-verified on source this cycle — flagged)*
- **Relevance:** 6/10 (model-derived SvO₂ estimate, not a direct optical vessel measurement)
- **Novelty:** A validated non-invasive *inferential* SvO₂ model for heart-failure patients, using routinely-available imaging/clinical inputs rather than a dedicated venous sensor.
- **Integration insights:** Represents the "estimate SvO₂ from correlated physiology" school — a benchmark for accuracy/utility that a direct optical venous read would need to surpass to justify new hardware.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans  *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** Gao, Zhu, et al.
- **Year / Venue:** 2023 · arXiv:2303.10775 (photoacoustic tomography + ultrasound)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 10/10 (direct, human, deep-vein, true venous sO₂ by optical/optoacoustic imaging)
- **Novelty:** Dual-wavelength PAT+US images the internal jugular vein and estimates SijvO₂ ≈ **72 ± 7 %** (n=7 healthy volunteers) — the single most important proof that optical/optoacoustic imaging can reach a deep venous target non-invasively.
- **Integration insights:** The flagship the entire Topic-2 corpus orbits. Today's new MC-PAT (§2.2) is the quantitative-methodology complement: where this paper proves the *target is reachable in humans*, MC-PAT sharpens *how accurately venous sO₂ can be recovered* once fluence is modelled. *(arXiv direct fetch returned 403 this cycle — metadata not re-read on source; SijvO₂ figure consistent across ≥15 prior scans.)*

### 2.2 — ★ NEW — Quantitative Photoacoustic Tomography of Blood Oxygenation Enhanced by Monte Carlo Modeling (MC-PAT)  *(newly catalogued this cycle — genuine venous demonstration)*
- **Authors:** Linghui Gong, Chao Cai, Hai Lin, Yidan Zhang, Zhaoyu Wang, Zequan Xu, Yubin Liu
- **Year / Venue:** **2025** (published Oct 13, 2025) · *Applied Physics Letters* **127(15):153701**
- **Link / DOI:** https://pubs.aip.org/aip/apl/article/127/15/153701/3367655 · **DOI 10.1063/5.0299956**
- **Relevance:** **9/10** (in-vivo, quantitative, explicit venous vs arterial sO₂ separation by optical imaging)
- **Novelty:** Couples **Monte-Carlo light-transport modelling** with finite-element acoustic inversion for 3-D quantitative mapping of tissue optical properties and blood oxygenation. Reports accurate absorption-coefficient recovery (0.44 ± 0.02 mm⁻¹, 1.85 % deviation) at 250 µm resolution, and — critically — **clear in-vivo arteriovenous differentiation: arterial 97.8 ± 0.8 % sO₂, venous 74.5 ± 1.3 % sO₂**, with 0.8 % error vs pulse oximetry (n=3 pilot).
- **Integration insights:** Directly attacks the dominant accuracy barrier for PA venous oximetry — **spectral coloring / wavelength-dependent fluence at depth** — by modelling the fluence rather than assuming it. The reported venous 74.5 % sits squarely in the physiological SvO₂ band and mirrors the IJV-PA anchor's ~72 %, giving a second, independently-modelled optical venous readout. It converges with the DNN+3-D-Monte-Carlo IJV work (§1.2) on the same principle: quantitative deep venous oximetry needs a modelled fluence prior, not an empirical one. Verify: title/authors/DOI/venue/in-vivo values cross-confirmed across AIP listing and a second index summary; AIP full-text direct fetch returned 403 (flagged), abstract-level metadata verified.

### 2.3 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂  *(previously surfaced — scan 07-15 §2.2, upgraded)*
- **Authors:** Sastry, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley), DOI 10.1002/advs.76366
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9/10 (in-vivo human venous sO₂ at the radial vein via an internal arterial reference)
- **Novelty:** The **arterial prior method (APM+)** uses the known high arterial sO₂ to calibrate local fluence at the artery and then estimate the oxygenation of neighbouring tissue/vessels — demonstrated in-vivo on the human **radial vein**.
- **Integration insights:** The purest expression of the field's **internal-reference principle**: use a compartment of *known* oxygenation to solve the unknown venous one. Complementary to MC-PAT (§2.2): APM+ calibrates fluence from a physiological anchor (the artery), MC-PAT from a physics model (Monte-Carlo) — two routes to the same goal of quantitative deep venous PA oximetry.

### 2.4 — ★ NEW — Transabdominal Fetal Oximetry via Diffuse Optics: Principled Analysis and Demonstration in Pregnant Ovine Models  *(newly catalogued this cycle — transferable technique, NOT venous-specific)*
- **Authors:** Weitai Qian, Rishad Raiyan Joarder, Randall Fowler, Begum Kasap, Mahya Saffarpour, Kourosh Vali, Tailai Lihe, Aijun Wang, Diana Farmer, Soheil Ghiasi (UC Davis)
- **Year / Venue:** **2025** (Sept 25, 2025) · arXiv:2509.21594 / TechRxiv / *PMC12486049* (PMID 41040802)
- **Link / DOI:** https://arxiv.org/abs/2509.21594 · https://pmc.ncbi.nlm.nih.gov/articles/PMC12486049/
- **Relevance:** **4/10** (fetal **arterial** SpO₂, not venous — included only as a transferable deep-tissue diffuse-optics method)
- **Novelty:** A principled diffuse-optics pipeline for estimating fetal oxygen saturation *through the thick maternal abdomen*, introducing the **Exponential Pulsation Ratio (EPR)** feature and an ML model that fuses multiple source–detector separations; MAE 4.81 % (simulation) / 6.85 % (in-vivo ovine).
- **Integration insights:** Not venous, but the engineering is squarely on the field's critical path: **recovering a saturation from a weak pulsatile signal buried under centimetres of scattering tissue** is exactly the deep-jugular / deep-limb-vein problem. The EPR feature and multi-detector fusion are directly portable to venous-pulsatility gating (venous-occlusion or respiratory-modulation) for deep-vein SvO₂. Included honestly as transferable technique, with a low venous-specific score. Metadata verified across arXiv/PMC/TechRxiv listings.

### 2.5 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry  *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (ADS-vis-OCT retinal-oximetry group)
- **Year / Venue:** 2023 · *Communications Medicine* (Nature), s43856-023-00288-8 (PMID 37095177)
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8
- **Relevance:** 7/10 (vessel-resolved retinal venous sO₂ — venous by vessel type, ~1 % bias; retinal, not systemic)
- **Novelty:** Adaptive spectroscopic vis-OCT that **removes vessel-specific spectral contaminants** to measure per-vessel sO₂ under each vessel's unique optical conditions, enabling clinically usable retinal artery/vein oximetry (retinal venous sO₂ ≈ 48–72 % depending on cohort).
- **Integration insights:** The retina remains the **per-vessel optical proving ground** where artery-vs-vein saturation is routinely separated with high spatial precision. Its adaptive per-vessel spectral-reference idea is conceptually the retinal analogue of MC-PAT's fluence modelling and APM+'s arterial prior — each solves the "the fluence/spectrum is vessel- and depth-dependent" problem in its own modality.

> **Standing Topic-2 context leads (not re-ranked):** sulfate/blood-matched PA phantoms for oximeter metrology (07-07 §2.2); PACT flow-pattern/oxygenation-heterogeneity imaging in human vessels (06-11); transmissive-detected hyperspectral single-vessel sO₂ (06-11 §2.1); high-resolution dual-camera hyperspectral retinal imager (06-18 §2.3); qPACT reviews & deep-learning spectral-decoloring/unmixing preprints; SFDI partial-occlusion oxygenation imaging (detects venous occlusion ≥25 %); T₂-oximetry cerebral venous mapping (MRI absolute reference). None newly advanced today.

---

## Cross-topic synthesis

1. **The one real movement this cycle is on Topic 2's quantitative-methodology front, not on venous targets.** MC-PAT (§2.2) is a genuine 2025 primary paper reporting an explicit in-vivo **venous 74.5 %** by optical imaging — independently corroborating the IJV-PA anchor's ~72 % (§2.1) with a completely different calibration route (Monte-Carlo fluence modelling vs empirical). Two modality-independent optical readouts now land in the same physiological venous band; that convergence is the day's most useful signal.

2. **The internal-reference principle keeps unifying the field.** Absolute non-invasive venous saturation is being reached not by a standalone absorption read but by a compartment/model of *known* fluence calibrating the unknown venous one: an artery calibrating a neighbour in APM+ (§2.3), a Monte-Carlo model supplying the fluence in MC-PAT (§2.2) and in the DNN+3-D-MC IJV work (§1.2), the LV/RV blood-pool ratio in MRI reference, and per-vessel adaptive spectral references in vis-OCT (§2.5). Every credible quantitative venous method now carries a fluence/spectral prior of some kind.

3. **The transferable-technique lane is live.** The new transabdominal fetal diffuse-optics paper (§2.4) is arterial and non-venous, but its EPR pulsation feature + multi-detector ML fusion for extracting saturation from a deep, faint pulsatile signal is directly portable to deep-vein venous-pulsatility gating — the practical route to peripheral SvO₂ without a catheter.

4. **The map is otherwise unchanged.** MRI (T₂/susceptometry) remains the absolute venous calibrator; the retina remains the per-vessel optical proving ground (vis-OCT, hyperspectral); the internal jugular vein remains the flagship deep-vein optical/optoacoustic target (IJV-PA, jugular NIRS/DNN, and now MC-PAT-class quantitative PAT); NIRS/venous-occlusion and venous-pulsatility PPG remain the practical peripheral surrogates; capnodynamic Capno-SvO₂ remains the non-optical benchmark to beat. **The unfilled prize — truly non-invasive human deep-vein optical SvO₂ validated at clinical scale — remains open.**

---

### Verification & honesty notes
- **Fully source-verified this cycle:** MC-PAT (§2.2) — title, 7 authors, *Applied Physics Letters* 127(15):153701, Oct 13 2025, DOI 10.1063/5.0299956, and in-vivo venous/arterial sO₂ values (cross-confirmed across the AIP listing and an independent index summary; AIP full text 403 on direct fetch — flagged). Transabdominal fetal diffuse-optics (§2.4) — title, 10 authors, UC Davis affiliation, Sept 25 2025, arXiv:2509.21594 / PMC12486049 / PMID 41040802 (cross-confirmed across arXiv, PMC, TechRxiv listings; arXiv/ResearchGate direct fetch 403 — flagged).
- **Previously-surfaced entries** carry metadata verified in earlier dated scans; where a direct source fetch 403'd today (arXiv IJV-PA, De Gruyter) this is noted inline and the figures are consistent with ≥15 prior scans. §1.5 venue/DOI not re-verified on source this cycle (flagged).
- **Sparseness is real, not padding:** only two new primary items exist across both topics today; no arterial-only work was added except the one explicitly-justified transferable-technique entry (§2.4), scored honestly low for venous relevance.
