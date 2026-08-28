# Daily Venous-Oxygen Research Scan — 2026-08-28

## ⚠️ Read this first — day summary

- **Environment limitation (today):** the session's network-egress allowlist again blocked all `WebFetch` access to primary sources — `arxiv.org`, `pubmed.ncbi.nlm.nih.gov`, `pmc.ncbi.nlm.nih.gov`, and `physicsworld.com` all returned **EGRESS_BLOCKED**. `WebSearch` worked, so titles/authors/venues below are **search-derived** and, where they could not be re-confirmed against the source page today, are flagged **⚠ unverified metadata**. Anchor-paper metadata is carried from earlier scans where it *was* fetch-verified (dates noted).
- **No genuinely-new venous-specific paper surfaced today.** Every candidate that search returned — Hybrid-Net (arXiv 2512.15394), the SPOI-AE physics-informed unmixing autoencoder (arXiv 2602.16357), the Davenet/Gateau ULM+PA planar-array paper (arXiv 2608.19823), the sulfate-phantom PA paper (arXiv 2512.01458), and the UTSW high-resolution hyperspectral retinal system — is **already surfaced in one or more prior dated scans** and is therefore not re-ranked as new here (see *Duplicate-check log* below).
- **The true-venous field remains sparse**, exactly as the last several scans reported. The strongest true-venous work is unchanged since the 06-10 corpus; those anchors recur below and are marked *previously surfaced*. I am **not** padding with arterial-only SpO₂ work — arterial items appear only where the technique is directly transferable to venous, with the reason stated.
- Net honest verdict for the day: **quiet.** No new lead worth elevating; the corpus is stable.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new human venous-specific paper today. The five strongest true-venous entries — all previously surfaced — are carried forward with honest scores. This reflects genuine low publication volume in this niche, not an incomplete search.*

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** research group publishing in *Current Directions in Biomedical Engineering* (as fetch-verified 06-10).
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter), CDBME.
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072 ⚠ unverified today (De Gruyter egress-blocked)
- **Relevance:** 9/10 — directly targets non-invasive *venous* sO₂ at the jugular via a pulse-oximeter-style optical sensor.
- **Novelty:** Pulse-oximeter-analogue sensor placed over the external/internal jugular; exploits arterio-venous compliance differences to render venous blood detectably pulsatile, estimating SvO₂ in the healthy 60–90% band across a small subject cohort (3 subjects; EJV waveform correctly identified).
- **Integration insights:** The cleanest "wearable optical → true venous sO₂" proof point; the reference design for a low-cost venous analogue to SpO₂. Complements the deep-tissue PA and imaging methods in Topic 2 (which localize the vessel but need bulkier hardware).

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669 (opg.optica.org/ol) — venue re-confirmed via search today.
- **Link:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 ⚠ page not fetched today (Optica egress-blocked); citation search-confirmed.
- **Relevance:** 8/10 — IJV-specific, non-invasive, venous.
- **Novelty:** Couples subject-specific 3-D Monte-Carlo light-transport modeling with a DNN to map multi-channel NIRS surface reflectance to IJV sO₂ *changes*, handling anatomical variability that defeats fixed calibration.
- **Integration insights:** The modeling/ML calibration layer that a device like §1.1 needs to generalize across patients; the Monte-Carlo prior is reusable for PA and DOT venous inversion in Topic 2.

### 1.3 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* (12938-017-0351-x).
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x ⚠ unverified today (egress-blocked); citation search-confirmed via Springer.
- **Relevance:** 8/10 — foundational peripheral venous method.
- **Novelty:** Induces artificial respiration-like modulation of peripheral vasculature to make venous blood pulsatile, then extracts a venous PPG for regional venous sO₂ — the conceptual root of the modulation-based venous-oximetry line.
- **Integration insights:** Method ancestor of the jugular device (§1.1) and the e-tattoo (§1.4); establishes that arterio-venous compliance contrast is an exploitable, reproducible signal source.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01)*
- **Authors:** Lu group (UT Austin); IEEE (EMBC-lineage) proceedings.
- **Year / Venue:** 2023–2024 · *IEEE* (Xplore doc 10340010) / associated MRS 2024 presentation. ⚠ metadata search-confirmed.
- **Link:** https://ieeexplore.ieee.org/document/10340010 ⚠ page not fetched today (IEEE egress-blocked).
- **Relevance:** 8/10 — explicitly separates arterial *and* venous oxygenation in a conformal wearable.
- **Novelty:** Ultrathin conformal optical "e-tattoo" resolving arterial and venous compartments simultaneously from the wrist; characterizes and mitigates artery/vein crosstalk (the close-proximity problem) via spatial filtering — a key step toward continuous ambulatory venous oximetry.
- **Integration insights:** The form-factor endpoint for the §1.1/§1.3 modulation approaches — shows the sensing principle can shrink to skin-conformal hardware suitable for continuous ward/home use.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6). ⚠ unverified today.
- **Link:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 ⚠ unverified today (ScienceDirect egress-blocked).
- **Relevance:** 7/10 — non-invasive ScvO₂ surrogate via transcutaneous jugular NIRS; commercially fielded (ongoing trials NCT04624009, NCT04778150).
- **Novelty:** Clinical validation of the Mespere VO100 measuring SjvO₂ over the jugular as a non-invasive stand-in for catheter ScvO₂ in critically ill patients.
- **Integration insights:** The commercial-maturity reference point for jugular venous NIRS; benchmarks the accuracy bar (trend-monitoring, not absolute) that optical/PA methods in Topic 2 must beat to displace catheters.

> **Device/regulatory anchor (not ranked):** *Noninvasix LIVOx optoacoustic central venous oxygenation monitor* — FDA **Breakthrough Device Designation** for non-invasive real-time ScvO₂ in adults at risk of septic shock (previously surfaced scan 08-11; not yet FDA-approved / not yet US-available). The optoacoustic ScvO₂ device milestone to watch for peer-reviewed validation data.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Year / Venue:** 2023 · preprint arXiv:2303.10775 (+ SPIE 8943 lineage, 2014). ⚠ page not fetched today (arXiv egress-blocked); citation search-confirmed.
- **Link:** https://arxiv.org/abs/2303.10775 ⚠ unverified today.
- **Relevance:** 9/10 — human, in vivo, PA, *venous* (IJV).
- **Novelty:** Dual-wavelength PAT + ultrasound images the internal jugular vein in 7 healthy volunteers; reported average IJV sO₂ ≈ 72 ± 7%, demonstrating true venous oximetry at depth non-invasively.
- **Integration insights:** The proof that PA reaches a clinically relevant central vein through intact tissue; the benchmark every new PA-oximetry method (2.2–2.4) is implicitly measured against for venous applicability.

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley), 10.1002/advs.76366. ⚠ page not fetched today (Wiley egress-blocked); citation search-confirmed.
- **Link:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366 ⚠ unverified today.
- **Relevance:** 9/10 — solves the fluence problem for deep-tissue PA sO₂ and reports in-vivo human radial-vein values.
- **Novelty:** Uses high, known arterial oxygenation as a local in-situ fluence reference to correct spectral coloring, cutting median sO₂ error to **2.9%** (vs 9.8% for linear unmixing) in phantom/ex-vivo tissue; the updated method (APM+) adds an intravascular-fluence-variation correction and demonstrates on human radial vein.
- **Integration insights:** Directly attacks the single biggest barrier to quantitative deep venous PA — unknown local fluence — using the artery as a self-calibrator. Pairs naturally with §2.1's IJV geometry and §1.2's Monte-Carlo priors.

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2024 · PACT venue (PMC11161372). ⚠ page not fetched today (PMC egress-blocked); citation search-confirmed.
- **Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/ ⚠ unverified today.
- **Relevance:** 8/10 — human, intravascular sO₂ heterogeneity and flow, PACT.
- **Novelty:** Shows intravascular oxygenation heterogeneity can be turned into a *contrast mechanism* for visualizing flow patterns inside human vessels with PACT — including recovering the parabolic laminar-flow wavefront inside a deep vein in vivo. Oxygenation as a tracer, not just an endpoint.
- **Integration insights:** Supports vessel-type discrimination (arterial vs venous by hemodynamics) and confirms human-scale PACT sensitivity to venous-range sO₂ gradients — the same "oxygenation + flow together" theme as the ULM+PA leads below.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature), s43856-023-00288-8. ⚠ page not fetched today; citation search-confirmed.
- **Link:** https://www.nature.com/articles/s43856-023-00288-8 ⚠ unverified today.
- **Relevance:** 8/10 — resolves *per-vessel arterial and venous* retinal sO₂ non-invasively.
- **Novelty:** Adaptively removes vessel-specific spectral contaminants; RMSE ≈ 2.1% vs pulse oximeter in major arteries, and repeatability SD ≈ 2.3% in *veins* — among the most accurate non-invasive per-vessel venous sO₂ figures reported. Demonstrated in glaucoma, ischemia, DR, CRVO, sickle-cell retinopathy.
- **Integration insights:** Sets the accuracy ceiling for optical venous oximetry in an accessible vascular bed; the adaptive spectral-correction idea is transferable to PA/DOT venous inversion where spectral coloring is the dominant error (cf. §2.2).

### 2.5 — Simultaneous 3D Co-Registered Perfusion and Oxygenation with ULM, Photoacoustic Imaging, and a Planar Matrix Array *(previously surfaced — first surfaced 08-25)*
- **Authors:** Léa Davenet, Jacques Battaglia, Franck Lager, Pascal Dargent, Charlotte Lussey-Lepoutre, Bertrand Tavitian, Olivier Couture, Lori Bridal, Jérôme Gateau (LIB / PARCC / CRC, Paris).
- **Year / Venue:** 2026 (August) · preprint **arXiv:2608.19823**. ⚠ page not fetched today (arXiv egress-blocked); citation search-confirmed.
- **Link:** https://arxiv.org/abs/2608.19823 ⚠ unverified today.
- **Relevance:** 7/10 — Topic-2 imaging technique yielding co-registered vessel-level sO₂; **tissue/vessel-level and small-animal, not human SvO₂** (score capped accordingly).
- **Novelty:** Integrates multispectral photoacoustic oximetry with **ultrasound localization microscopy (ULM)** on a *single planar ultrasonic matrix array*, producing spatially co-registered 3-D maps of blood oxygenation *and* sub-diffraction microvascular perfusion at once. Validated in vessel-mimicking phantoms and in vivo in mice.
- **Integration insights:** Co-registering oxygenation with ULM flow direction is a plausible route to *label a vessel as venous vs arterial from its hemodynamics* rather than from sO₂ alone — a recurring gap in PA venous oximetry (telling the target vein from neighboring arteries). Shared planar array points toward a single-probe deep venous imager; watch for a human/large-vessel follow-up and a peer-reviewed version.

---

## Standing context leads (not ranked in the top-5)

- **High-resolution hyperspectral retinal imaging system, UTSW (PMC12997856)** — first surfaced 08-13; still the most recent genuinely-new retinal-oximetry hardware entry. Simultaneously extracts per-vessel diameter and oxygenation; deep-learning pansharpening RMSE ≈ 2.15. Reports **average venule sO₂ ≈ 58%** vs arteriole ≈ 98% — a clean per-vessel *venous* readout in an accessible bed. Small-animal (mouse) validation; not human SvO₂. ⚠ metadata search-derived.
- **Hybrid-Net — Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and Oxygen Saturation Estimation (arXiv 2512.15394, Dec 2025; Shang, Jandhyala, Wu, Hoffer-Hawlik et al.)** — jointly segments vessels and estimates in-vessel sO₂ from dual-wavelength sPA; segmentation ≥0.978 (sim)/0.998 (exp), sO₂ MSE ≤0.048 (sim)/0.003 (exp). Vessel-level, not venous-specific; relevant because vessel segmentation is a prerequisite to isolating a target vein. *Previously surfaced.*
- **SPOI-AE — Optical Inversion & Spectral Unmixing of sPA Images with Physics-Informed Neural Networks (arXiv 2602.16357, Feb 2026; Ter Martirosyan, Huang, Qin, Yu, Emelianov)** — physics-informed autoencoder for non-linear sPA optical inversion; in-vivo mouse lymph-node tissue sO₂. Tissue-level; a transferable inversion tool for venous sO₂ quantification. *Previously surfaced.*
- **Sulfate phantoms to mimic NIR photoacoustic response of whole blood at selected oxygen saturations (arXiv 2512.01458, Dec 2025)** — calibration/phantom methodology for PA blood-sO₂ validation. Enabling, not a measurement result. *Previously surfaced.*
- **Capnodynamic non-invasive mixed-venous SvO₂ (NCT06632197, ongoing trial)** — non-optical, but the most active *venous* clinical effort; watch for first results.

---

## Duplicate-check log (why nothing new was ranked today)

| Candidate returned by search | arXiv/ID | First surfaced in prior scan(s) | Action |
|---|---|---|---|
| Hybrid-Net sPA segmentation + sO₂ | 2512.15394 | 06-11 … 08-23 (37 files) | Not re-ranked; standing lead |
| SPOI-AE physics-informed unmixing | 2602.16357 | 06-25 … 08-23 (12 files) | Not re-ranked; standing lead |
| Davenet/Gateau ULM+PA planar array | 2608.19823 | 07-08 … 08-25 | Kept as §2.5 (prev. surfaced) |
| Sulfate-phantom PA blood sO₂ | 2512.01458 | 06-14 … 08-23 (36 files) | Not re-ranked; standing lead |
| UTSW hyperspectral retinal HSI | PMC12997856 | 06-18 … 08-23 (22 files) | Standing lead (venule sO₂ 58%) |

No candidate cleared the "genuinely new / newer version" bar today.

---

## Cross-topic synthesis

1. **A quiet day, honestly reported.** Every paper web-search surfaced today is already in the corpus; no new venous-specific study appeared. This is consistent with the field's genuinely low publication volume in *non-invasive, true-venous* oximetry — not a gap in searching. Primary-source verification was additionally constrained by the environment's egress block on arXiv/PubMed/PMC.

2. **The field's shape is unchanged and still bimodal.** Topic 1 (true human venous) rests on the same five anchors since June — jugular optical sensing (§1.1), IJV DNN/Monte-Carlo (§1.2), peripheral pulse-modulation (§1.3), the e-tattoo (§1.4), jugular NIRS (§1.5) — plus the Noninvasix LIVOx device milestone. Topic 2 momentum sits in *imaging technique*: fluence-corrected deep-tissue PA (§2.2 APM+), per-vessel vis-OCT retinal venous sO₂ (§2.4), and the 2026 convergence of **PA oxygenation + ULM/Doppler perfusion** on shared arrays (§2.3, §2.5).

3. **The unsolved core problems are stable and shared.** (a) *Which vessel is the vein?* — hemodynamic co-registration (§2.3, §2.5) and vessel segmentation (Hybrid-Net) offer physics/ML discriminators that pure spectral methods lack. (b) *Unknown local fluence / spectral coloring* — attacked by artery-referenced calibration (§2.2), adaptive spectral removal (§2.4), physics-informed inversion (SPOI-AE), and Monte-Carlo priors (§1.2). The near-term opportunity remains **porting these Topic-2 advances onto the Topic-1 clinical venous targets** (IJV, radial/peripheral veins).

4. **Confidence caveat.** Because source-page fetching was blocked, all metadata above is search-derived; recurring anchors were fetch-verified in earlier scans, and items are flagged ⚠ where they could not be re-confirmed against the source this run. Re-verify against arXiv/PMC on the next scan where fetching is available.

---
*Scan generated 2026-08-28. Sources located via `WebSearch`; direct source-page verification unavailable today due to network egress restrictions (arXiv, PubMed/PMC, De Gruyter, Optica, IEEE, Wiley, ScienceDirect, physicsworld all egress-blocked). Metadata flagged ⚠ where it could not be confirmed against the source this run.*
