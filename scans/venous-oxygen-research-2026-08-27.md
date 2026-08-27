# Daily Venous-Oxygen Research Scan — 2026-08-27

## ⚠️ Read this first — day summary

- **Environment limitation (today):** the session's network egress allowlist again blocked all `WebFetch`/`curl` access to primary sources. Every domain tested — arXiv, PubMed/PMC, IOPscience, De Gruyter, Optica (opg), Wiley, Semantic Scholar — returned `EGRESS_BLOCKED`. `WebSearch` works, so **metadata below is search-derived and could not be re-verified against the source page today.** Items whose metadata could not be independently confirmed this run are flagged **⚠ unverified metadata**; recurring anchors carry titles/venues that *were* fetch-verified in earlier scans (dates noted).
- **One genuinely-new lead today (Topic 2):** *Photoacoustics on the go: An Embedded Photoacoustic Sensing Platform* (**arXiv:2510.25256**, Oct 2025). First compact, low-power **embedded** PA sensing platform aimed at non-invasive real-time monitoring of oxygenation / blood flow / glucose several cm below the skin, using LiDAR-style low-cost laser diodes and an MCU-driven transmitter. **Not venous-specific and not a new oximetry result** — a hardware/form-factor advance — but directly transferable to the wearable deep-venous PA trajectory, and it does not appear in any prior scan. Surfaced here for the first time under Topic 2 "new this scan."
- **The true-venous field remains sparse**, exactly as the last several scans reported. No new *human, venous-specific, non-invasive* SvO₂/ScvO₂ paper surfaced today. The strongest true-venous work is unchanged since the 06-10 corpus; those anchors recur below and are marked *previously surfaced*. I am **not** padding with arterial-only SpO₂ work.
- Nothing else that surfaced today was new: the sulfate-phantom metrology paper (arXiv:2512.01458), the hyperspectral retinal system (JBO 31(3):036006 / PMC12997856), APM+ (Adv. Sci.), the IJV-PA anchor (arXiv:2303.10775), PACT flow, ADS-vis-OCT, and the *npj Acoustics* PA-detection review all map to already-catalogued entries.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new human venous-specific paper today. The five strongest true-venous entries — all previously surfaced — are carried forward with honest scores. This reflects genuine low publication volume in this niche, not an incomplete search.*

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** research group publishing in *Current Directions in Biomedical Engineering* (full author list fetch-verified 06-10; not re-fetched today).
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter), CDBME.
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072 ⚠ unverified today (De Gruyter egress-blocked)
- **Relevance:** 9/10 — directly targets non-invasive *venous* sO₂ at the jugular via a pulse-oximeter-style optical sensor.
- **Novelty:** Pulse-oximeter-analogue single-point sensor over the external jugular vein; identifies the EJV waveform and estimates SvO₂ from the venous pulse (≈70–72 %) and the respiration/breathing pulse (≈74–75 %), all within the healthy 60–90 % band, across a 3-subject proof-of-concept cohort.
- **Integration insights:** The cleanest "wearable optical → true venous sO₂" proof point; the reference design for a low-cost venous analogue to SpO₂. Complements the deep-tissue PA and imaging methods in Topic 2 (which localize the vessel but need bulkier hardware). Still awaiting calibration/validation against gold-standard blood-gas co-oximetry.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669 (fetch-verified 06-10). ⚠ metadata unverified today.
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 ⚠ unverified today.
- **Relevance:** 8/10 — IJV-specific, non-invasive, venous.
- **Novelty:** Couples subject-specific 3-D Monte-Carlo light-transport modeling with a DNN to map surface optical signals to IJV sO₂ *changes*, handling anatomical variability that defeats fixed calibration.
- **Integration insights:** The modeling/ML calibration layer that a device like §1.1 needs to generalize across patients; the Monte-Carlo prior is reusable for PA and DOT venous inversion in Topic 2.

### 1.3 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* (12938-017-0351-x).
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x ⚠ unverified today (PMC egress-blocked).
- **Relevance:** 8/10 — foundational peripheral venous method.
- **Novelty:** Induces artificial respiration-like modulation of peripheral vasculature to make venous blood pulsatile, then extracts a venous PPG for regional venous sO₂ — the conceptual root of the modulation-based venous-oximetry line.
- **Integration insights:** Method ancestor of the jugular device (§1.1) and the e-tattoo (§1.4); establishes that arterio-venous compliance contrast is an exploitable, reproducible signal source.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01)*
- **Year / Venue:** 2024–2025 · wearable-electronics / biosensing venue. ⚠ metadata unverified today.
- **Relevance:** 8/10 — explicitly separates arterial *and* venous oxygenation in a conformal wearable.
- **Novelty:** Ultrathin conformal optical "e-tattoo" that resolves arterial and venous compartments simultaneously, pushing venous oximetry toward continuous ambulatory monitoring.
- **Integration insights:** The form-factor endpoint for the §1.1/§1.3 modulation approaches — shows the sensing principle can shrink to skin-conformal hardware suitable for continuous ward/home use.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6); PMID 37827917. ⚠ unverified today.
- **Link:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 ⚠ unverified today.
- **Relevance:** 7/10 — non-invasive ScvO₂ surrogate via transcutaneous jugular NIRS; commercially fielded.
- **Novelty:** Clinical validation of the Mespere VO100 measuring SjvO₂ over the jugular as a non-invasive stand-in for catheter ScvO₂ in critically ill patients. Corroborated by ongoing SjvO₂-vs-ScvO₂ correlation studies (e.g. NCT04624009, NCT04778150) reporting strong linear correlation in COVID-ventilated and post-liver-transplant cohorts.
- **Integration insights:** The commercial-maturity reference point for jugular venous NIRS; benchmarks the accuracy bar (trend-monitoring, not absolute) that optical/PA methods in Topic 2 must beat to displace catheters.

> **Device/regulatory anchor (not ranked):** *Noninvasix LIVOx optoacoustic central venous oxygenation monitor* (ScvO₂ for septic shock) — previously surfaced scan 08-11. Optoacoustic ScvO₂ device milestone; watch for peer-reviewed validation data.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Year / Venue:** 2023 · preprint arXiv:2303.10775 (+ associated SPIE lineage). ⚠ unverified today (arXiv egress-blocked).
- **Link:** https://arxiv.org/abs/2303.10775 ⚠ unverified today.
- **Relevance:** 9/10 — human, in vivo, PA, *venous* (IJV).
- **Novelty:** Dual-wavelength PAT + ultrasound images the internal jugular vein in seven healthy volunteers; reported average IJV sO₂ ≈ 72 ± 7 %, demonstrating true venous oximetry at depth non-invasively as a real-time surrogate for cerebral oxygen consumption.
- **Integration insights:** The proof that PA reaches a clinically relevant central vein through intact tissue; the benchmark every new PA-oximetry method (2.2–2.4) is implicitly measured against for venous applicability.

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley), 10.1002/advs.76366. ⚠ unverified today (Wiley/doi egress-blocked).
- **Link:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366 ⚠ unverified today.
- **Relevance:** 9/10 — solves the fluence problem for deep-tissue PA sO₂ and reports in-vivo human radial-vein values.
- **Novelty:** Uses high, known arterial oxygenation as a local in-situ fluence reference to correct spectral coloring, cutting median sO₂ error to **2.9 %** (vs 9.8 % for linear unmixing); demonstrated on human radial vein.
- **Integration insights:** Directly attacks the single biggest barrier to quantitative deep venous PA — unknown local fluence — using the artery as a self-calibrator. Pairs naturally with §2.1's IJV geometry and §1.2's Monte-Carlo priors.

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2024 · photoacoustic-computed-tomography venue (PMC11161372). ⚠ metadata unverified today.
- **Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/ ⚠ unverified today.
- **Relevance:** 8/10 — human, intravascular sO₂ heterogeneity and flow, PACT.
- **Novelty:** Shows intravascular oxygenation heterogeneity can be turned into a *contrast mechanism* for visualizing laminar flow patterns inside a deep human vein in real time with PACT — oxygenation as a tracer, not just an endpoint.
- **Integration insights:** Supports vessel-type discrimination and confirms human-scale PACT sensitivity to venous-range sO₂ gradients; a conceptual sibling of the oxygenation+flow co-registration theme running through 2026 PA work.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature), s43856-023-00288-8; PMC10126115. ⚠ unverified today.
- **Link:** https://www.nature.com/articles/s43856-023-00288-8 ⚠ unverified today.
- **Relevance:** 8/10 — resolves *per-vessel arterial and venous* retinal sO₂ non-invasively.
- **Novelty:** Adaptively removes vessel-specific spectral contaminants; RMSE ≈ 2.1 % vs pulse oximeter in major arteries, and repeatability SD ≈ 2.3 % in *veins* — among the most accurate non-invasive per-vessel venous sO₂ figures reported. Demonstrated in glaucoma, ischemia, DR, CRVO, sickle-cell retinopathy.
- **Integration insights:** Sets the accuracy ceiling for optical venous oximetry in an accessible vascular bed; the adaptive spectral-correction idea is transferable to PA/DOT venous inversion where spectral coloring is the dominant error (cf. §2.2).

### 2.5 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — scan 07-07; retinal venous sO₂)*
- **Authors:** Tran, … Fei et al. (UT Southwestern).
- **Year / Venue:** 2026 · *Journal of Biomedical Optics* 31(3):036006 (PMC12997856; accepted 2026-02-24). ⚠ unverified today (SPIE/PMC egress-blocked).
- **Link / DOI:** https://doi.org/10.1117/1.JBO.31.3.036006 · PMC12997856 ⚠ unverified today.
- **Relevance:** 8/10 — dual-camera HSI system that *simultaneously* extracts vessel diameter and per-vessel oxygenation, reporting **venule sO₂ ≈ 76 %** vs arteriole ≈ 96 %; directly measures retinal *venous* saturation.
- **Novelty:** Snapshot dual-camera hyperspectral retinal imager giving co-registered arteriole/venule sO₂ + caliber in one acquisition; a 2026 hardware validation of the retinal artery–vein oximetry approach.
- **Integration insights:** Complements the vis-OCT ceiling (§2.4) from the wide-field-snapshot direction; the retina remains the most accessible bed for benchmarking optical *venous* oximetry against a known physiological arteriovenous difference.

> **★ New this scan (Topic 2 hardware lead, not ranked in the top-5):**
> **Photoacoustics on the go: An Embedded Photoacoustic Sensing Platform** — **arXiv:2510.25256** (Oct 2025). ⚠ metadata search-derived (arXiv egress-blocked).
> - **Link:** https://arxiv.org/abs/2510.25256
> - **Relevance:** 6/10 — a Topic-2 *technique/hardware* advance that is **not venous-specific and reports no new oximetry result**; scored for direct transferability, not for a venous measurement.
> - **Novelty:** First compact, low-power **embedded** PA sensing platform: a LiDAR-inspired transmitter driving low-cost laser diodes from a general-purpose MCU, paired with an integrated ultrasound receiver and on-board processing, targeting non-invasive real-time monitoring of oxygenation / blood flow / glucose several centimeters below the skin — explicitly aimed at moving PA out of the benchtop into wearable/point-of-care form factors.
> - **Integration insights:** The missing hardware half of the wearable-venous-PA vision. The true-venous PA anchors (§2.1 IJV, §2.2 radial vein) prove the *measurement*; this proves the *form factor* could shrink. A credible near-term path is to marry an embedded transmitter like this with APM+-style fluence correction (§2.2) and the §1.2 Monte-Carlo/DNN calibration to build a wearable deep-venous PA oximeter. Watch for a follow-up that reports actual in-vivo sO₂ (esp. venous) from the platform.

---

## Standing context leads (not ranked in the top-5)

- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université / LIB), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Inorganic sulfate solutions reproduce both optical absorption and the Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm — a ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % range. **Previously surfaced** metrology lead; no change.
- **Simultaneous 3D co-registered perfusion + oxygenation with ULM + photoacoustic imaging (planar matrix array)** — Davenet, Gateau et al., arXiv:2608.19823 (Aug 2026). Co-registered volumetric sO₂ + microvascular flow from a single planar matrix array; vessel/tissue-level, small-animal. **Previously surfaced** (08-25); the oxygenation+flow co-registration theme that could label a vessel venous-vs-arterial from hemodynamics.
- **Hyperspectral retinal imaging system (per-vessel artery + vein sO₂), JBO 31(3):036006** — now promoted into the Topic-2 top-5 (§2.5); logged here historically.
- **Wearable FD-NIRS ASIC system (Feb 2026, PMC12904531)** — real-time multi-frequency wearable frequency-domain NIRS on a custom ASIC. *Tissue StO₂, not venous SvO₂* — wearable-hardware trajectory a venous method (§1.4) could ride. ⚠ metadata search-derived.
- **"Advancements in Photoacoustic Detection Techniques for Biomedical Imaging," *npj Acoustics* (2025), 10.1038/s44384-025-00005-w** — review of PA detection hardware (incl. non-contact/remote-sensing PARS); breadth context for the detection side of deep-vein PA oximetry, not venous-specific.
- **Capnodynamic non-invasive mixed-venous SvO₂ (NCT06632197, ongoing trial)** — non-optical, but among the most active *venous* clinical efforts; watch for first results.

---

## Cross-topic synthesis

1. **Today's signal is a form-factor advance, not a new venous measurement.** The one genuinely-new item (§2.5-adjacent *Photoacoustics on the go*, arXiv:2510.25256) says nothing about veins directly — but it is exactly the piece the venous-PA program lacks. Topic 2 has repeatedly proven the *measurement* (IJV PA at 72 %, radial-vein APM+ at 2.9 % error, human PACT flow); what has been missing is a *wearable, low-cost, embedded* front end. An embedded PA platform is the first concrete step toward the same "shrink it to skin-conformal hardware" endpoint that Topic 1's e-tattoo (§1.4) reaches from the PPG side.

2. **The two mature accuracy anchors still frame the field.** APM+ (§2.2, deep-tissue, artery-referenced fluence correction, 2.9 % error) and ADS-vis-OCT (§2.4, per-vessel retinal venous sO₂, ~2.3 % repeatability) bracket the state of the art from the deep-tissue and superficial-bed ends respectively. The 2026 hyperspectral retinal system (§2.5) adds a snapshot wide-field validation of retinal artery–vein oximetry. All three hinge on the same core fix — controlling **spectral coloring / unknown fluence** — which is also what §1.2's Monte-Carlo priors and the sulfate-phantom metrology target.

3. **Topic 1 (true human venous) remains genuinely thin.** The best non-invasive human venous work — jugular optical sensing (§1.1), IJV DNN/Monte-Carlo (§1.2), peripheral pulse-modulation (§1.3), the e-tattoo (§1.4), and jugular NIRS (§1.5) — is unchanged since June. This is a real publication-volume gap, not a search artifact; the imaging-technique side (Topic 2) is where 2026 momentum sits, and the near-term opportunity is porting Topic-2 advances (fluence correction, adaptive spectral removal, oxygenation-flow co-registration, and now embedded PA hardware) onto the Topic-1 clinical venous targets (IJV, radial/peripheral veins).

4. **Caveat on today's confidence:** because source-page fetching was blocked by the environment's egress policy, all metadata above is search-derived. The recurring anchors were fetch-verified in earlier scans; the one new item (arXiv:2510.25256) and the standing leads should be re-verified against arXiv/PMC on the next scan where fetching is available.

---
*Scan generated 2026-08-27. Sources located via web search; direct source-page verification unavailable today due to network egress restrictions (arXiv, PubMed/PMC, IOPscience, De Gruyter, Optica, Wiley, Semantic Scholar all egress-blocked). Metadata flagged ⚠ unverified where it could not be confirmed against the source this run.*
