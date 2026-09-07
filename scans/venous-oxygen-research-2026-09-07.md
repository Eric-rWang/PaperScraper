# Daily Venous-Oxygen Research Scan — 2026-09-07

## ⚠️ Read this first — day summary

- **Scan cadence:** 49th scan in the series (immediately prior run 2026-09-05; no run on 09-06). Emphasis on work published or first-surfacing after 09-05.
- **Verification caveat (today):** `WebSearch` was available and productive, but `WebFetch` to scholarly hosts remains **egress-blocked by the environment's network policy** — direct `WebFetch` of PubMed, PMC, IEEE Xplore, and Europe PMC (EBI) each returned `EGRESS_BLOCKED` this run, identical to the 08-29 → 09-05 runs. Every item below was therefore **cross-checked across ≥2 independent search-index snippets** rather than read on the publisher page. Items whose full metadata could not be page-verified are flagged **⚠ search-derived**.
- **This was a PRODUCTIVE run — TWO genuinely new-to-corpus papers surfaced, one per topic, and both are venous-relevant** (a grep of all 48 prior scan files confirms neither was previously logged):
  1. **Topic 1 (NEW):** *Non-invasive, Continuous Venous Oxygen Saturation and Oxygen Extraction Estimation from the Internal Jugular Vein* — **2025 IEEE EMBC** conference paper (IEEE Xplore doc 11254941; PubMed 41335695; DOI 10.1109/EMBC58623.2025.11254941). A **flexible neck sensor array** that reads the IJV pulse + breathing modulation to estimate **true SvO₂ (65.7–80.9 %)** and cerebral **O₂ extraction ratio** in 6 healthy adults. This is a real new true-venous device paper and enters the Topic-1 top-5 at **§1.1**.
  2. **Topic 2 (NEW):** *Serial dual-wavelength illumination for retinal vessel oximetry using a conventional fundus camera: a proof-of-concept study* — **2026** (PubMed 42576210; PMC13455296; received Apr 2026 / accepted Aug 2026). Serial 548 nm/605 nm LED illumination on a stock fundus camera measuring **per-vessel arterial AND venous** retinal sO₂ in 9 participants vs a commercial oximeter. Enters Topic-2 at **§2.5**.
- **Candidates checked and confirmed already-in-corpus this run:** the jugular optical-sensing paper (De Gruyter CDBME 10.1515/cdbme-2024-2072), the IJV DNN/Monte-Carlo paper (Opt. Lett. 49(10):2669), the peripheral pulse-modulation proof-of-concept (BMEO s12938-017-0351-x), the Mespere VO100 jugular NIRS validation (S1053-0770(23)00782-6; PubMed 37827917), the e-tattoo paper (IEEE 10340010 / PubMed 38083768) and its patent (US 2025/0025074 A1), the human IJV PAT anchor (arXiv:2303.10775), APM+ (Adv. Sci. 10.1002/advs.76366; PMC13334587; PubMed 42397001), PACT intravascular flow (PMC11161372), ADS-vis-OCT (PMC10126115), the hyperspectral fundus system (PMC12997856 / PubMed 41858558), 3D-PAULMprior (bioRxiv 722751), the Davenet/Gateau ULM+PA planar-matrix platform (arXiv:2608.19823), the sulfate-phantom metrology paper (Appl. Opt. 65(6):1974 / arXiv:2512.01458), Hybrid-Net (arXiv:2512.15394), and Apple's PPGen/HAI (arXiv:2510.02073) — all re-surfaced, all already logged.
- The strongest previously-surfaced true-venous entries are carried forward below with honest scores; the two new items are marked **⭐ NEW to corpus**.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*One genuinely new true-venous paper surfaced today (§1.1). The remaining four strongest true-venous entries — all previously surfaced — are carried forward with honest scores. This remains a genuine low-publication-volume niche.*

### 1.1 — Non-invasive, Continuous Venous Oxygen Saturation and Oxygen Extraction Estimation from the Internal Jugular Vein *(⭐ NEW to corpus this scan — first logged 2026-09-07)*
- **Authors:** ⚠ search-derived — index snippets attribute the work to **Jordan F. Hill, Aaron S. Hess, Christopher G. Pretty, J. Geoffrey Chase** (bioengineering group associated with the jugular-optical-sensing line, cf. §1.2). IEEE page egress-blocked, so treat the exact author list as tentative until page-verified.
- **Year / Venue:** 2025 · **IEEE Engineering in Medicine & Biology Conference (EMBC 2025)** proceedings.
- **Link / DOI:** https://ieeexplore.ieee.org/document/11254941/ · DOI 10.1109/EMBC58623.2025.11254941 · PubMed 41335695. ⚠ IEEE/PubMed egress-blocked today; metadata cross-checked on ≥2 index snippets.
- **Relevance:** **8.5/10** — directly targets non-invasive, continuous **true venous** sO₂ at the internal jugular vein, plus derived cerebral O₂ extraction. Among the strongest new true-venous device results the series has caught in months.
- **Novelty:** A **flexible/conformal sensor array** placed on the right side of the neck detects pulsatile signals from **both the carotid artery and the IJV**. Because peripheral veins are non-pulsatile (defeating conventional pulse oximetry), the method exploits the **IJV pulse plus breathing-induced modulation** to render venous blood detectably variable, then extracts SvO₂ optically. Evaluated in **6 healthy adults**: SaO₂ from a commercial pulse oximeter, SvO₂ estimated from the IJV pulse; reported average **SvO₂ ≈ 65.7–80.9 %** (physiologically plausible venous band) and a per-subject **cerebral oxygen-extraction ratio (O₂ER)** — a step beyond single-point sO₂ toward a metabolic readout.
- **Integration insights:** This is the continuous, extraction-capable successor to the flagship jugular optical-sensing device (§1.2, Alqahtani 2024) and shares the arterio-venous-compliance/breathing-modulation principle of the peripheral pulse-modulation line (§1.3). Two things make it notable for the broader goal: (1) it co-registers artery **and** vein at the same neck site, so the artery can serve as an in-situ reference — the same self-calibration logic APM+ (§2.2) uses in photoacoustics; (2) reporting **O₂ER**, not just sO₂, aligns the wearable-optical branch with the clinical endpoint (cerebral/global oxygen consumption) that jugular catheters are actually used for. The obvious next step is fusing this pulse-based extraction with the Monte-Carlo/DNN calibration layer of §1.2 to handle inter-subject neck-anatomy variability.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10)*
- **Year / Venue:** 2024 · *Optics Letters* **49**(10):2669 (opg.optica.org/ol) — venue re-confirmed via Optica index snippet today.
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 ⚠ full text egress-blocked today.
- **Relevance:** 8/10 — IJV-specific, non-invasive, venous.
- **Novelty:** Couples subject-specific 3-D Monte-Carlo light-transport modeling with a DNN to map multi-channel surface NIRS reflectance to IJV sO₂ *changes*, handling anatomical variability that defeats fixed calibration.
- **Integration insights:** The modeling/ML calibration layer the new §1.1 pulse device needs to generalize across patients; the Monte-Carlo prior is reusable for PA and DOT venous inversion in Topic 2.

### 1.3 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:126 (s12938-017-0351-x).
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x · PMC5437414. ⚠ PMC full text egress-blocked; abstract re-confirmed via index snippet today.
- **Relevance:** 8/10 — foundational peripheral venous method.
- **Novelty:** Induces artificial respiration-like modulation of the peripheral vasculature (exploiting arterio-venous compliance contrast) to make venous blood pulsatile, then extracts a venous PPG for regional venous sO₂ (SpvO₂) — the conceptual root of the modulation-based venous-oximetry line that the new §1.1 IJV device extends to the neck.
- **Integration insights:** Method ancestor of the jugular devices (§1.1, §1.2 lineage) and the e-tattoo (§1.4); establishes arterio-venous compliance contrast as an exploitable, reproducible signal source.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01; patent US 2025/0025074 A1 logged 09-05)*
- **Authors / Venue:** Lu group (UT Austin) · 2023 IEEE conference (EMBC-style), IEEE Xplore doc 10340010; PubMed 38083768. Re-confirmed via IEEE + PubMed snippets today.
- **Relevance:** 8/10 — explicitly separates arterial *and* venous oxygenation in a conformal wearable.
- **Novelty:** Ultrathin conformal optical "e-tattoo" measuring arterial and venous pulses at the wrist; identifies artery–vein **crosstalk** (from their close proximity) as the key obstacle to simultaneous SaO₂/SvO₂ extraction and proposes **spatial filtering** to suppress it, characterized in simulation, in vitro, and in vivo. Its IP filing (US 2025/0025074 A1) was logged 09-05.
- **Integration insights:** The wrist-scale, skin-conformal endpoint for the same artery+vein co-registration principle the new §1.1 neck device demonstrates at the IJV; the crosstalk-suppression framing is the practical bridge from bench to ambulatory wearable.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6); PubMed 37827917.
- **Link:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 ⚠ egress-blocked; metadata via index snippet.
- **Relevance:** 7/10 — non-invasive ScvO₂ surrogate via transcutaneous jugular NIRS; commercially fielded.
- **Novelty:** Clinical validation of the Mespere VO100 measuring SjvO₂ over the jugular as a non-invasive stand-in for catheter ScvO₂ in critically ill patients. Supporting evidence: the pediatric-cardiac transcutaneous-jugular NIRS cohort (PMC7491293, r = 0.91, bias 2.92 %).
- **Integration insights:** The commercial-maturity reference point for jugular venous NIRS; benchmarks the accuracy bar (trend-monitoring, not absolute) that the new §1.1 pulse device and the optical/PA methods in Topic 2 must beat to displace catheters.

> **Dropped from the ranked five this run:** the Alqahtani 2024 jugular optical-sensing device (CDBME 10.1515/cdbme-2024-2072, prior §1.1) — still a landmark, but the new §1.1 EMBC 2025 IJV paper is its continuous, extraction-capable successor and now leads the topic. Alqahtani 2024 remains the flagship *first* optical-venous-device proof and is retained here as the anchor of the lineage.
> **Device/regulatory anchor (not ranked):** *Noninvasix LIVOx optoacoustic central venous oxygenation monitor* (ScvO₂ for septic shock; FDA Breakthrough Device Designation, 2022) — previously surfaced 08-11. No 2026 peer-reviewed validation data has yet appeared; watch for it.
> **Clinical-trial anchors (not ranked, non-optical/reference):** *Capnodynamic non-invasive mixed-venous SvO₂* (NCT06632197); *Continuous jugular venous oxygen saturation after cardiac arrest* (NCT06511999); *Noninvasive Internal Jugular Venous Oximetry* (NCT06004466); *SjvO₂ NIRS* trials (NCT04624009, NCT04778150). A ScvO₂-vs-SvO₂ correlation meta-analysis (PMC13195361, rev. May 2026) re-surfaced — catheter-based reference, not optical.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*One genuinely new per-vessel retinal-venous paper surfaced today (§2.5). The PA/vis-OCT venous anchors (§2.1–§2.4) are unchanged; the 08-13 hyperspectral fundus system remains the most recent prior intravascular-venular result and is retained as a standing lead.*

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Year / Venue:** 2023 · preprint arXiv:2303.10775 (+ SPIE lineage). ⚠ arXiv egress-blocked today; abstract re-confirmed on two index snippets.
- **Link:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9/10 — human, in vivo, PA, *venous* (IJV).
- **Novelty:** Dual-wavelength PAT + ultrasound images the internal jugular vein in **7 healthy volunteers** at 5 fps; reported average IJV sO₂ ≈ **72 ± 7 %**, with fast US co-registration enabling temporal sO₂ tracking under physiologic challenges — true venous oximetry at depth, non-invasively.
- **Integration insights:** The proof that PA reaches a clinically relevant central vein through intact tissue; the imaging counterpart to the new §1.1 pulse-based IJV device — same vessel, different sensing physics (absorption spectroscopy at depth vs surface pulse modulation).

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): In-Vivo Human Radial-Vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry, Olick-Gibson et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley), 10.1002/advs.76366; PMC13334587; PubMed 42397001. ⚠ Wiley/PMC egress-blocked today; abstract re-confirmed via index snippet.
- **Link:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9/10 — solves the fluence problem for deep-tissue PA sO₂ and reports in-vivo human values on the radial artery–vein pair (n = 8).
- **Novelty:** Uses high, known arterial oxygenation as a local in-situ **fluence reference** to correct spectral coloring, cutting median sO₂ error to **2.9 %** (vs 9.8 % for linear unmixing); human **venous sO₂ median 72.3 % (IQR 8.9 %)** on the radial vein, robust through ex-vivo tissue up to 1.5 cm.
- **Integration insights:** Directly attacks the single biggest barrier to quantitative deep venous PA — unknown local fluence — using the artery as a self-calibrator, the same artery-as-reference logic the new §1.1 neck device applies in the PPG/pulse domain. Pairs naturally with §2.1's IJV geometry and §1.2's Monte-Carlo priors.

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2024 · PACT venue; PMC11161372; PubMed 38855671. ⚠ PMC egress-blocked; abstract re-confirmed via snippet.
- **Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** 8/10 — human, intravascular sO₂ heterogeneity and flow, PACT; recovers the parabolic laminar-flow wavefront inside a deep vein in vivo.
- **Novelty:** Shows intravascular oxygenation heterogeneity can be turned into a *contrast mechanism* for visualizing flow patterns inside human vessels with PACT — oxygenation as a tracer, not just an endpoint — and demonstrates dynamic sO₂ imaging in a deep vein.
- **Integration insights:** Supports vessel-type discrimination from hemodynamics (the core unsolved venous problem — "which vessel is the vein?") and confirms human-scale PACT sensitivity to venous-range sO₂ gradients.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature), s43856-023-00288-8; PubMed 37095177; PMC10126115. ⚠ egress-blocked; metadata via snippet.
- **Link:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10126115/
- **Relevance:** 8/10 — resolves *per-vessel arterial and venous* retinal sO₂ non-invasively.
- **Novelty:** Adaptively removes vessel-specific spectral contaminants; RMSE ≈ 2.1 % vs pulse oximeter in major arteries, repeatability SD ≈ 2.3 % in *veins*; ex-vivo blood-phantom agreement within 1 % bias across 0–100 % sO₂. Demonstrated across glaucoma, ischemia, DR, CRVO, sickle-cell retinopathy.
- **Integration insights:** Sets the accuracy ceiling for optical venous oximetry in an accessible vascular bed; the adaptive spectral-correction idea is the high-end counterpart to the low-cost serial-illumination approach newly surfaced at §2.5, and is transferable to PA/DOT venous inversion where spectral coloring dominates error (cf. §2.2).

### 2.5 — Serial Dual-Wavelength Illumination for Retinal Vessel Oximetry Using a Conventional Fundus Camera: A Proof-of-Concept Study *(⭐ NEW to corpus this scan — first logged 2026-09-07)*
- **Authors:** ⚠ not page-verifiable today (PMC/PubMed egress-blocked); author list not confirmed on index snippets — flagged for verification next run.
- **Year / Venue:** 2026 · journal name **not confirmed** on the source page (⚠ search-derived; ophthalmology/vision-science venue, received Apr 2026 / accepted Aug 2026). PubMed 42576210; PMC13455296.
- **Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC13455296/ · PubMed https://pubmed.ncbi.nlm.nih.gov/42576210/ ⚠ both egress-blocked; metadata cross-checked on ≥2 snippets.
- **Relevance:** **7/10** — measures **per-vessel arterial AND venous** retinal sO₂ non-invasively; a true intravascular venular optical readout, though retinal per-vessel (not systemic SvO₂) and venous accuracy is still modest (see below).
- **Novelty:** Retrofits a **stock (conventional) fundus camera** with a custom fiber-coupled LED unit delivering **serial** illumination at **548 nm** (hemoglobin isosbestic) and **605 nm** (oxygen-sensitive), each 250 ms, then registers the sequential frames and applies standard retinal-oximetry algorithms. The key methodological point: **serial** (time-multiplexed) illumination **avoids the detector-level spectral crosstalk** that plagues simultaneous dual-wavelength capture on one-chip color cameras. In 9 participants vs a commercial oximeter, arterial agreement was good (mean absolute difference **3.6 ± 2.7 %**; 99.4 ± 5.7 % vs 100.4 ± 3.0 %) but **venous agreement was markedly worse (8.4 ± 9.3 %)** — the authors flag venous measurement as needing further optimization.
- **Integration insights:** A **low-cost, camera-retrofit** route to the same per-vessel venous readout that vis-OCT (§2.4) and hyperspectral fundus imaging (standing lead) reach with far more elaborate instrumentation — important for accessibility/screening. But its honest venous error bar (~8–9 %) quantifies exactly why venules are harder than arterioles for reflectance oximetry (lower contrast, diameter/pigmentation confounds), reinforcing that the spectral-decoloring advances in §2.2/§2.4 are the missing ingredient. The serial-vs-simultaneous crosstalk insight is directly portable to any multi-wavelength venous-imaging front end.

---

## Standing context leads (not ranked in the top-5)

- **Hyperspectral fundus system — *Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina*** (Tran M.H. et al., UT Southwestern/UT Dallas; *J. Biomed. Opt.* **31**(3):036006, 2026; PMC12997856; PubMed 41858558). *Previously surfaced 08-13; was the most recent prior intravascular-venular result.* Snapshot hyperspectral + RGB + deep-learning pansharpening recovering per-vessel venule sO₂ (≈58 %) and diameter simultaneously. The higher-end sibling of the new §2.5 serial-illumination fundus method.
- **Davenet, … Gateau — Simultaneous 3D Co-Registered Perfusion and Oxygenation with ULM, Photoacoustic Imaging, and a Planar Matrix Array** (arXiv:2608.19823, Aug 2026). Multispectral PA sO₂ across ≈60–95 % at 5 % accuracy using only five wavelengths, co-registered with ULM microvascular perfusion on a single planar matrix array; phantom + in-vivo mice. *Tissue/vessel-level, small-animal.* Its promise for venous work is **hemodynamic vessel-type discrimination**.
- **3D-PAULMprior — Three-Dimensional Photoacoustic Tomography with Ultrasound Localization Priors** (bioRxiv 10.64898/2026.05.04.722751, May 2026). *First logged 09-04; ULM-prior model-based PA reconstruction that improves blood-oxygen-saturation estimation; small-animal.* Attacks the limited-view/ill-posedness side of the deep-vessel PA error budget.
- **APM+ verification note:** APM+ (§2.2) now also indexed at **PMC13334587 / PubMed 42397001** — additional publisher-side confirmation of the *Advanced Science* record (previously only Wiley DOI).
- **Apple ML: PPGen + Hybrid Amortized Inference** (arXiv:2510.02073, Oct 2025; peer-reviewed at *IOP* 10.1088/3049-477X/ae4a96). *Technique-transfer lead — arterial/general PPG, NOT a venous measurement (~4/10 to true venous).* Extending PPGen's dynamic term to an explicit *venous* compartment is a concrete route to model-based SpvO₂ — directly relevant to the new §1.1 pulse/breathing-modulation IJV device.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood** (*Applied Optics* **65**(6):1974, 2026; arXiv:2512.01458). Injectable ground-truth for validating multi-wavelength PA venous oximetry.
- **Hybrid-Net — Deep-Learning Quantitative Spectroscopic PA for Segmentation + sO₂** (arXiv:2512.15394, Dec 2025). Joint vessel segmentation + sO₂ without explicit fluence estimation; general PA method, not venous-specific.
- **Melanin-corrected absolute tissue oxygen saturation via hybrid transmittance–reflectance spectroscopy** (PMC13271197, 2026). *Tissue StO₂, not intravascular venous sO₂* — logged for the decoloring/melanin-correction toolkit that per-vessel venous methods (§2.5) need.
- **SFDI / wearable NIRS (tissue-level, not venous SvO₂):** *SFDI-net* (PMC12014942) and venous-vs-arterial-occlusion discrimination; *Advances in fully integrated wearable NIRS* (IOP 10.1088/2515-7647/ae6ae4, 2026). Superficial tissue StO₂ / venous-occlusion contrast, not intravascular venous sO₂.

---

## Cross-topic synthesis

1. **A productive cycle — the dry spell breaks with TWO new venous-relevant papers, one per topic.** After the 08-23 → 09-05 run of "no new true-venous paper" reports, this scan surfaced (a) a **2025 IEEE EMBC** flexible-neck-sensor IJV device that reports **true SvO₂ (65.7–80.9 %) and cerebral O₂ extraction ratio** (§1.1), and (b) a **2026** serial-illumination fundus-camera method measuring **per-vessel arterial and venous** retinal sO₂ (§2.5). Both were absent from all 48 prior scan files. The field is still low-volume, but it is not static.

2. **The two new items sit at opposite ends of the same design space and rhyme with each other.** §1.1 (surface pulse/breathing modulation, deep central vein, metabolic O₂ER endpoint) and §2.5 (per-vessel reflectance imaging, superficial retinal bed, screening-grade hardware) both (a) co-measure artery and vein together, and (b) report **honest venous limitations** — §1.1 a plausible-but-wide 65–81 % band from n = 6, §2.5 an explicit **8.4 ± 9.3 % venous error** vs a commercial oximeter. Veins remain systematically harder than arteries in both domains, for the same underlying reason: lower/variable venous signal contrast and the artery–vein disambiguation problem.

3. **Where 2026 momentum sits is now visible on both topics.** Topic 1's momentum is **artery-referenced, extraction-aware wearable venous sensing** (§1.1 EMBC device → §1.4 e-tattoo → PPGen forward-model lead). Topic 2's momentum remains **ULM + photoacoustic co-registration** (Davenet/Gateau, 3D-PAULMprior) plus **spectral-decoloring per-vessel imaging** (§2.2 APM+, §2.4 vis-OCT, §2.5 serial-illumination). The unifying thread across both: **use the artery as an in-situ reference to pin down the harder venous measurement** — APM+ does it with fluence, §1.1 does it with the co-located carotid pulse.

4. **Accuracy anchors still frame the ceiling.** APM+ (§2.2, 2.9 % deep-tissue error, venous median 72.3 %) and ADS-vis-OCT (§2.4, ~2.3 % venous repeatability, 1 % phantom bias) bracket the state of the art. The new §2.5 method's ~8–9 % venous error shows how much headroom cheaper hardware still has — and that closing it means importing the decoloring/fluence-correction ideas the anchors pioneered.

5. **The near-term opportunity is still porting, now with a concrete new target.** The highest-leverage move is transferring Topic-2 advances (fluence correction, adaptive spectral decoloring, ULM-prior reconstruction, serial-illumination crosstalk suppression, PPGen compartment modeling) onto Topic-1 venous targets — and the new §1.1 IJV device is an ideal recipient: a wearable that already co-registers artery and vein and reports O₂ER, waiting for a Monte-Carlo/DNN calibration layer (§1.2) and an artery-as-reference decoloring step (§2.2) to move it from n = 6 proof-of-concept toward clinical accuracy.

6. **Confidence caveat.** `WebFetch` to all scholarly hosts was egress-blocked today (PubMed, PMC, IEEE Xplore, EBI/Europe PMC each confirmed `EGRESS_BLOCKED`), so all metadata is search-snippet-derived (each item cross-checked on ≥2 snippets). For the two new items specifically: §1.1's author list is search-derived and tentative; §2.5's journal name and authors could not be confirmed on the source page. Both new items' abstracts/quantitative results (SvO₂ range and O₂ER for §1.1; the 548/605 nm serial scheme and 3.6 %/8.4 % arterial/venous error for §2.5) were each corroborated across multiple independent snippets. Publisher-page verification should be repeated on the next scan where direct fetching is permitted.

---
*Scan generated 2026-09-07. Sources located and cross-verified via web search (≥2 independent index snippets per item); direct publisher/preprint-page fetching unavailable this run due to the environment's network egress policy (PubMed, PMC, IEEE Xplore, and EBI/Europe PMC confirmed `EGRESS_BLOCKED` via direct WebFetch; arXiv, Optica, Wiley, De Gruyter, SPIE historically blocked). Metadata flagged ⚠ where it could not be confirmed on the source page.*
