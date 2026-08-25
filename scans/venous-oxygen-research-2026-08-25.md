# Daily Venous-Oxygen Research Scan — 2026-08-25

## ⚠️ Read this first — day summary

- **Environment limitation (today):** the session's network egress allowlist blocked all `WebFetch`/`curl` access to primary sources (arXiv, PubMed/PMC, De Gruyter, Optica, IOPscience, Wiley, doi.org all returned egress-blocked / 403). Metadata below is therefore **search-derived and could not be re-verified against the source page today.** Items I could not independently confirm are flagged **⚠ unverified metadata**. Titles/venues for the recurring anchor papers are carried from earlier scans where they *were* fetch-verified (dates noted).
- **One genuinely-new lead today (Topic 2):** *Simultaneous 3D co-registered perfusion and oxygenation with ULM, photoacoustic imaging, and a planar matrix array* (Davenet, Gateau et al., **arXiv 2608.19823, Aug 2026**). Co-registered volumetric sO₂ + microvascular flow from a single planar matrix array; validated in phantoms and in vivo in mice. Not true SvO₂ (tissue/vessel-level, small-animal), but a directly transferable Topic-2 imaging advance — surfaced here for the first time.
- **The true-venous field remains sparse**, exactly as the last several scans reported. No new *human, venous-specific, non-invasive* SvO₂/ScvO₂ paper surfaced today. The strongest true-venous work is unchanged since the 06-10 corpus; those anchors recur below and are marked *previously surfaced*. I am **not** padding with arterial-only SpO₂ work.
- Two further recent-but-adjacent items (wearable FD-NIRS ASIC system, Feb 2026; 3D-PAULM PAT+ULM brain/tumor, bioRxiv Apr 2026) are logged under **Standing context leads** rather than the ranked top-5, because they measure tissue StO₂ / small-animal vasculature, not venous SvO₂.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new human venous-specific paper today. The five strongest true-venous entries — all previously surfaced — are carried forward with honest scores. This reflects genuine low publication volume in this niche, not an incomplete search.*

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** (as fetch-verified 06-10) research group publishing in *Current Directions in Biomedical Engineering*.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter), CDBME.
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072 ⚠ unverified today (De Gruyter egress-blocked)
- **Relevance:** 9/10 — directly targets non-invasive *venous* sO₂ at the jugular via a pulse-oximeter-style optical sensor.
- **Novelty:** Pulse-oximeter-analogue sensor placed over the external/internal jugular; exploits arterio-venous compliance differences to render venous blood detectably pulsatile, estimating SvO₂ in the healthy 60–90% band across a small subject cohort.
- **Integration insights:** The cleanest "wearable optical → true venous sO₂" proof point; the reference design for a low-cost venous analogue to SpO₂. Complements the deep-tissue PA and imaging methods in Topic 2 (which localize the vessel but need bulkier hardware).

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year / Venue:** 2023–2024 · biomedical-optics / biophotonics venue (fetch-verified 06-10). ⚠ metadata unverified today.
- **Link / DOI:** carried from 06-10 file. ⚠ unverified today.
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
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6). ⚠ unverified today.
- **Link:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 ⚠ unverified today.
- **Relevance:** 7/10 — non-invasive ScvO₂ surrogate via transcutaneous jugular NIRS; commercially fielded.
- **Novelty:** Clinical validation of the Mespere VO100 measuring SjvO₂ over the jugular as a non-invasive stand-in for catheter ScvO₂ in critically ill patients.
- **Integration insights:** The commercial-maturity reference point for jugular venous NIRS; benchmarks the accuracy bar (trend-monitoring, not absolute) that optical/PA methods in Topic 2 must beat to displace catheters.

> **Device/regulatory anchor (not ranked):** *Noninvasix LIVOx optoacoustic central venous oxygenation monitor* (ScvO₂ for septic shock) — previously surfaced scan 08-11. Optoacoustic ScvO₂ device milestone; watch for peer-reviewed validation data.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Year / Venue:** 2023 · preprint arXiv:2303.10775 (+ associated SPIE lineage). ⚠ unverified today (arXiv egress-blocked).
- **Link:** https://arxiv.org/abs/2303.10775 ⚠ unverified today.
- **Relevance:** 9/10 — human, in vivo, PA, *venous* (IJV).
- **Novelty:** Dual-wavelength PAT + ultrasound images the internal jugular vein in healthy volunteers; reported average IJV sO₂ ≈ 72 ± 7%, demonstrating true venous oximetry at depth non-invasively.
- **Integration insights:** The proof that PA reaches a clinically relevant central vein through intact tissue; the benchmark every new PA-oximetry method (2.2–2.4) is implicitly measured against for venous applicability.

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley), 10.1002/advs.76366. ⚠ unverified today (Wiley/doi egress-blocked).
- **Relevance:** 9/10 — solves the fluence problem for deep-tissue PA sO₂ and reports in-vivo human radial-vein values.
- **Novelty:** Uses high, known arterial oxygenation as a local in-situ fluence reference to correct spectral coloring, cutting median sO₂ error to **2.9%** (vs 9.8% for linear unmixing); demonstrated on human radial vein.
- **Integration insights:** Directly attacks the single biggest barrier to quantitative deep venous PA — unknown local fluence — using the artery as a self-calibrator. Pairs naturally with §2.1's IJV geometry and §1.2's Monte-Carlo priors.

### 2.3 — ★ NEW — Simultaneous 3D Co-Registered Perfusion and Oxygenation with ULM, Photoacoustic Imaging, and a Planar Matrix Array *(first surfaced today)*
- **Authors:** Léa Davenet, Jacques Battaglia, Franck Lager, Pascal Dargent, Charlotte Lussey-Lepoutre, Bertrand Tavitian, Olivier Couture, Lori Bridal, Jérôme Gateau (LIB / PARCC / CRC, Paris).
- **Year / Venue:** 2026 (August) · preprint **arXiv:2608.19823**. ⚠ unverified today (arXiv egress-blocked; authors/title/abstract are search-derived).
- **Link:** https://arxiv.org/abs/2608.19823 ⚠ unverified today.
- **Relevance:** 7/10 — a Topic-2 imaging technique that yields co-registered vessel-level sO₂; **tissue/vessel-level and small-animal, not human SvO₂** (score capped accordingly).
- **Novelty:** Integrates **multispectral photoacoustic oximetry** with **ultrasound localization microscopy (ULM)** on a *single planar ultrasonic matrix array*, producing spatially co-registered 3-D volumetric maps of blood oxygenation *and* sub-diffraction microvascular perfusion at once. Validated in vessel-mimicking phantoms and in vivo in mice.
- **Integration insights:** Co-registering oxygenation with ULM flow directions is a plausible route to *label a vessel as venous vs arterial from its hemodynamics* rather than from sO₂ alone — a recurring gap in PA venous oximetry (distinguishing the target vein from neighboring arteries). The shared planar matrix array also points toward a single-probe deep venous imager. Watch for a human/large-vessel follow-up; a peer-reviewed version should be tracked.

### 2.4 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2023–2024 · photoacoustic-computed-tomography venue. ⚠ metadata unverified today.
- **Relevance:** 8/10 — human, intravascular sO₂ heterogeneity and flow, PACT.
- **Novelty:** Shows intravascular oxygenation heterogeneity can be turned into a *contrast mechanism* for visualizing flow patterns inside human vessels with PACT — oxygenation as a tracer, not just an endpoint.
- **Integration insights:** Conceptual sibling of §2.3 (oxygenation + flow together); supports vessel-type discrimination and confirms human-scale PACT sensitivity to venous-range sO₂ gradients.

### 2.5 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature), s43856-023-00288-8. ⚠ unverified today.
- **Link:** https://www.nature.com/articles/s43856-023-00288-8 ⚠ unverified today.
- **Relevance:** 8/10 — resolves *per-vessel arterial and venous* retinal sO₂ non-invasively.
- **Novelty:** Adaptively removes vessel-specific spectral contaminants; RMSE ≈ 2.1% vs pulse oximeter in major arteries, and repeatability SD ≈ 2.3% in *veins* — among the most accurate non-invasive per-vessel venous sO₂ figures reported. Demonstrated in glaucoma, ischemia, DR, CRVO, sickle-cell retinopathy.
- **Integration insights:** Sets the accuracy ceiling for optical venous oximetry in an accessible vascular bed; the adaptive spectral-correction idea is transferable to PA/DOT venous inversion where spectral coloring is the dominant error (cf. §2.2).

---

## Standing context leads (not ranked in the top-5)

- **Wearable FD-NIRS ASIC system (Feb 2026, PMC12904531)** — real-time multi-frequency (50–350 MHz) wearable frequency-domain NIRS on a custom ASIC (685/850 nm laser diodes, SiPM detector; μ_a accuracy ~0.0007 mm⁻¹ at 14.7 Hz). *Tissue StO₂, not venous SvO₂* — logged for the wearable-hardware trajectory that a venous method (§1.4) could ride. ⚠ metadata search-derived.
- **3D-PAULM: Integrated Photoacoustic Tomography and Ultrasound Localization Microscopy for Multiparametric Brain and Tumor Imaging (bioRxiv, 30 Apr 2026)** — sibling of §2.3 combining PAT + ULM for oxygenation + microvascular flow; small-animal brain/tumor. Reinforces the "oxygenation + flow co-registration" theme. ⚠ metadata search-derived.
- **Hyperspectral retinal imaging system (per-vessel artery + vein sO₂)** — first surfaced 08-13; still the most recent genuinely-new retinal-oximetry hardware entry. No update today.
- **Capnodynamic non-invasive mixed-venous SvO₂ (NCT06632197, ongoing trial)** — non-optical, but the most active *venous* clinical effort; watch for first results.

---

## Cross-topic synthesis

1. **Today's signal is convergence of oxygenation + flow imaging, not a new venous-specific paper.** The one fresh lead (§2.3 Davenet/Gateau, arXiv Aug 2026), together with the bioRxiv 3D-PAULM standing lead, marks a clear 2026 trend: pairing **photoacoustic sO₂** with **ULM/Doppler perfusion** on a shared array. For *venous* monitoring this matters because the hardest unsolved problem is not measuring sO₂ but **knowing which vessel is the vein** — hemodynamic co-registration offers a physics-based discriminator that pure spectral methods lack.

2. **The two mature accuracy anchors still frame the field.** APM+ (§2.2, deep-tissue, artery-referenced fluence correction, 2.9% error) and ADS-vis-OCT (§2.5, per-vessel retinal venous sO₂, ~2.3% repeatability) bracket the state of the art from the deep-tissue and superficial-bed ends respectively. Any new venous method should be benchmarked against these, and both hinge on the same core fix — controlling **spectral coloring / unknown fluence** — which is exactly what §2.3's co-registration and §1.2's Monte-Carlo priors also target.

3. **Topic 1 (true human venous) remains genuinely thin.** The best non-invasive human venous work — jugular optical sensing (§1.1), IJV DNN/Monte-Carlo (§1.2), peripheral pulse-modulation (§1.3), the e-tattoo (§1.4), and jugular NIRS (§1.5) — is unchanged since June. This is a real publication-volume gap, not a search artifact; the imaging-technique side (Topic 2) is where 2026 momentum sits, and the near-term opportunity is porting Topic-2 advances (fluence correction, adaptive spectral removal, oxygenation-flow co-registration) onto the Topic-1 clinical venous targets (IJV, radial/peripheral veins).

4. **Caveat on today's confidence:** because source-page fetching was blocked by the environment's egress policy, all metadata above is search-derived. The recurring anchors were fetch-verified in earlier scans; the one new item (§2.3) and the standing leads should be re-verified against arXiv/PMC on the next scan where fetching is available.

---
*Scan generated 2026-08-25. Sources located via web search; direct source-page verification unavailable today due to network egress restrictions (arXiv, PubMed/PMC, De Gruyter, Optica, IOPscience, Wiley, doi.org all egress-blocked). Metadata flagged ⚠ unverified where it could not be confirmed against the source this run.*
