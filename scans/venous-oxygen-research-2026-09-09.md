# Daily Venous-Oxygen Research Scan — 2026-09-09

## ⚠️ Read this first — day summary

- **Scan cadence:** 51st scan in the series (immediately prior run 2026-09-08). Emphasis on work published or first-surfacing after 09-08.
- **Verification caveat (today):** `WebSearch` was available and productive, but `WebFetch` to scholarly hosts remains **egress-blocked by the environment's network policy** — direct `WebFetch` of arXiv, PMC and ScienceDirect all returned `EGRESS_BLOCKED` this run, identical to the 08-29 → 09-08 runs. Every item below was therefore **cross-checked across ≥2 independent search-index snippets** rather than read on the publisher page. Items whose full metadata could not be page-verified are flagged **⚠ search-derived**.
- **This was a MODEST but genuinely productive run for Topic 2 — TWO new-to-corpus *Photoacoustics*-journal papers surfaced (a grep of all 50 prior scan files confirms neither was previously logged), plus a verification/indexing update on an existing standing lead:**
  1. **Topic 2 (NEW):** *Maximum fluence for accurate functional photoacoustic microscopy* — **2026**, *Photoacoustics*, **DOI 10.1016/j.pacs.2026.100851** (PMC13319516; PubMed 42389549). Establishes the safe-and-accurate laser-fluence ceiling for functional PAM sO₂ — and, critically, that ceiling is **set by the onset of a spurious *venous* sO₂ increase** (thermal bias appears first in the venous compartment). Directly relevant to the venous-PA error budget. Enters Topic-2 top-5 at **§2.5**.
  2. **Topic 2 (NEW):** *Frequency-domain photoacoustic microscopy with resonant transducer and interferometric modulation for high-reliability sO₂ imaging* — **2026**, *Photoacoustics*, **DOI 10.1016/j.pacs.2026.100834** (PMC13156710; PubMed 42111354). AOM-interferometric FD-PAM with a high-Q resonant transducer delivering **<2 % within-group sO₂ variation across oxygenated, mixed AND deoxygenated conditions** — reliability demonstrated *into the venous saturation range*. Logged as a standing lead (general PAM instrumentation, not venous-specific).
  3. **Topic 2 (UPDATE):** the *Novel Differential Pathlength Factor (DPF) model for NIR diffuse optical imaging* (arXiv:2602.00283) — previously a standing lead — is now **peer-reviewed and PMC/PubMed-indexed** (PMC13532703; PubMed 42687887; v2 posted 2026-08-25). Authors confirmed: **Kaiser Niknam, Mannu Bardhan Paul, Mini Das (University of Houston)**. Recorded as a genuinely-new-version update, not a fresh entry.
- **Topic 1 was quiet today — NO new true-venous paper surfaced.** Every Topic-1 candidate returned by search was already in the corpus (see confirmed list below). Honest assessment: genuine non-invasive *venous* (SvO₂/ScvO₂) work is a low-volume niche and today produced nothing new; the ranked Topic-1 five are carried forward unchanged with honest scores.
- **Candidates checked and confirmed already-in-corpus this run:** the sternal-PPG mixed-venous proof-of-concept (PubMed 42527850, first logged 09-08), the OPCAB jugular/cerebral-NIRS vs PA-catheter SvO₂ study (PubMed 42606675, first logged 09-08), the FD-NIRS single-ventricle pediatric StO₂/OEF study (PubMed 42476299, first logged 09-08), the EMBC flexible-neck IJV device (IEEE 11254941; PubMed 41335695), the Mespere VO100 jugular-NIRS validation (S1053-0770(23)00782-6; PubMed 37827917), the human IJV PAT anchor (arXiv:2303.10775), the IJV DNN/Monte-Carlo paper (Opt. Lett. 49(10):2669), the 2017 peripheral pulse-modulation proof-of-concept (BMEO s12938-017-0351-x), the Alqahtani jugular optical-sensing paper (CDBME 10.1515/cdbme-2024-2072), APM+ (Adv. Sci. 10.1002/advs.76366; PMC13334587), PACT intravascular flow (PMC11161372), ADS-vis-OCT (PMC10126115; s43856-023-00288-8), the serial-illumination fundus paper (BMC Ophthalmology 10.1186/s12886-026-05216-7; PMC13455296), the hyperspectral fundus system (J. Biomed. Opt. 31(3):036006; PMC12997856), Transmissive-Detected HSI single-vessel oxygen mapping (PMC12707973), the ISDC PA depth/spectral-compensation paper (10.1117/1.JBO.31.2.026002; PMC12869027), Hybrid-Net / DL-QSPA (arXiv:2512.15394; PMC13122505; PubMed 41990476), the Ghiasi transabdominal fetal diffuse-optics paper (arXiv:2509.21594; PMC12486049), and Apple's PPGen/HAI (arXiv:2510.02073) — all re-surfaced, all already logged.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*A quiet day for Topic 1 — no new true-venous paper surfaced; every candidate was already in the corpus. The ranked five are carried forward from 09-08 unchanged, with honest scores. This remains a genuine low-publication-volume niche, and today it produced nothing new-to-corpus.*

### 1.1 — Monitoring Changes in Mixed Venous Oxygen Saturation Using Photoplethysmography on the Sternum — A Proof of Concept Study *(previously surfaced — first logged 2026-09-08)*
- **Authors:** ⚠ search-derived — not page-confirmed (PubMed egress-blocked). Likely the Scandinavian intraosseous-sternal-PPG group behind the earlier porcine sternal-oximetry work (*J. Clin. Monit. Comput.* 10.1007/s10877-023-00980-z).
- **Year / Venue:** 2026 · venue **not page-confirmed** (⚠ search-derived; likely *Physiological Measurement* or *J. Clinical Monitoring and Computing*). PubMed 42527850.
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/42527850/ ⚠ egress-blocked; DOI not captured.
- **Relevance:** **8/10** — non-invasive, continuous **true mixed-venous SvO₂** with a pulmonary-artery-catheter reference; a genuinely new anatomical site (sternum) for venous oximetry.
- **Novelty:** Exploits **sternal intramedullary (intraosseous) blood**, whose saturation tracks central/mixed-venous saturation, read **transcutaneously with a PPG probe** on the sternum. In 15 anesthetized pigs, SvO₂ was driven down by stepwise hypoxia and staged hemorrhage while nSsO₂ was calibrated against pulmonary-artery SvO₂: **linear nSsO₂–SvO₂ correlation, 87 % concordance (95 % CI 79.1–95.0)** for tracking SvO₂ changes.
- **Integration insights:** A third distinct physical route to non-invasive venous sO₂, complementary to the IJV pulse-modulation device (§1.5) and jugular NIRS (§1.2, §1.4): the **bone marrow acts as a naturally venous-weighted optical reservoir**, sidestepping the artery–vein disambiguation problem. Trend-grade (87 %) performance sets a realistic accuracy bar; a natural fusion target for the pulse-modulation math of §1.5.

### 1.2 — Near-Infrared Spectroscopy for Estimating Mixed Venous Oxygen Saturation and Cardiac Output During Off-Pump Coronary Artery Bypass Grafting: A Prospective Observational Study *(previously surfaced — first logged 2026-09-08)*
- **Authors:** ⚠ search-derived — not page-confirmed (PubMed egress-blocked).
- **Year / Venue:** 2026 · venue **not page-confirmed** (⚠ search-derived; anesthesia/monitoring journal). PubMed 42606675.
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/42606675/ ⚠ egress-blocked; DOI not captured.
- **Relevance:** **7.5/10** — non-invasive SvO₂ surrogate via **jugular + cerebral NIRS**, validated head-to-head against **pulmonary-artery-catheter SvO₂** in adults.
- **Novelty:** Tests two non-invasive NIRS surrogates in 25 OPCAB patients — (a) **rSjvO₂** over the left IJV (bias 2.0 %, wide LoA −14.9/+18.9 %) and (b) **baseline-calibrated cerebral NIRS (cal-rScO₂)** on the forehead (bias 0.8 %, LoA −7.8/+9.4 %, excellent SvO₂ < 65 % discrimination, good trending). **NIRS-derived cardiac output failed** (33 % error).
- **Integration insights:** The most rigorous 2026 adult validation yet of jugular/cerebral NIRS as an SvO₂ *trend* monitor. Tellingly, **baseline-calibrated cerebral NIRS out-tracked a sensor placed right over the IJV** — a strong argument for the vessel-*resolving* imaging of Topic 2 (PA, vis-OCT) over surface averaging. Clean SvO₂ < 65 % discrimination is the clinically actionable low-SvO₂-alarm endpoint.

### 1.3 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — commercial NIRS device)*
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6); PubMed 37827917.
- **Link:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 ⚠ egress-blocked; metadata via index snippet.
- **Relevance:** 7/10 — non-invasive ScvO₂ surrogate via transcutaneous jugular NIRS; commercially fielded.
- **Novelty:** Clinical validation of the Mespere VO100 measuring SjvO₂ over the jugular as a non-invasive stand-in for catheter ScvO₂ in critically ill patients. Supporting evidence: pediatric-cardiac transcutaneous-jugular NIRS (PMC7491293, r = 0.91, bias 2.92 %).
- **Integration insights:** The commercial-maturity reference point for jugular venous NIRS; the accuracy bar (trend-monitoring, not absolute) that the newer §1.1/§1.2 methods and the optical/PA methods in Topic 2 must beat to displace catheters.

### 1.4 — Non-invasive, Continuous Venous Oxygen Saturation and Oxygen Extraction Estimation from the Internal Jugular Vein *(previously surfaced — the flagship new-generation true-venous device)*
- **Authors:** ⚠ search-derived (bioengineering group associated with the jugular-optical-sensing line).
- **Year / Venue:** 2025 · **IEEE EMBC 2025** proceedings. IEEE Xplore doc 11254941; PubMed 41335695; DOI 10.1109/EMBC58623.2025.11254941. ⚠ egress-blocked; metadata cross-checked on ≥2 snippets.
- **Link:** https://ieeexplore.ieee.org/document/11254941/
- **Relevance:** 8.5/10 — directly targets non-invasive, continuous **true venous** sO₂ at the IJV plus cerebral O₂ extraction.
- **Novelty:** Flexible/conformal neck sensor array reads the **IJV pulse + breathing-induced modulation** (peripheral veins being non-pulsatile) to estimate SvO₂ ≈ **65.7–80.9 %** and a per-subject **cerebral O₂-extraction ratio (O₂ER)** in 6 healthy adults; co-registers carotid artery and IJV at one site.
- **Integration insights:** The extraction-aware wearable endpoint of the whole Topic-1 program; the artery serves as an in-situ reference (same logic as APM+, §2.2). §1.1 (sternal-marrow reservoir) and §1.2 (jugular/cerebral NIRS) are the alternative-site and surface-NIRS counterparts to this vessel-targeted pulse device.

### 1.5 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (arterio-venous compliance pulse-modulation) *(previously surfaced — foundational method ancestor)*
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60; DOI 10.1186/s12938-017-0351-x; PMC5437414.
- **Link:** https://biomedical-engineering-online.biomedcentral.com/articles/10.1186/s12938-017-0351-x
- **Relevance:** 7/10 — the original non-invasive peripheral-venous (SpvO₂) optical concept.
- **Novelty:** Uses the **compliance difference between arteries and veins** to induce artificial respiration-like modulation that makes venous blood pulsatile, then reads the induced PPG to build a calibration model for regional venous sO₂; validated in healthy volunteers with arm-lift/occlusion maneuvers against arterial and venous blood-gas references.
- **Integration insights:** The method ancestor of the §1.1 sternal-PPG and §1.4 IJV-pulse devices — every "make the vein pulsatile, then read it like a pulse oximeter" approach traces here. Its modest accuracy is exactly what the deep-diffuse-optics pulsation-decomposition ideas in Topic 2 (EPR / multi-detector ML) aim to improve.

> **Dropped from the ranked five (still important, carried in lineage):** the FD-NIRS single-ventricle pediatric StO₂/OEF study (PubMed 42476299, first logged 09-08 — *tissue-level StO₂ + OEF, not true intravascular SvO₂*, but validated against invasive SVC saturation) and the Alqahtani 2024 jugular optical-sensing device (CDBME 10.1515/cdbme-2024-2072).
> **Device/regulatory anchor (not ranked):** *Noninvasix LIVOx optoacoustic central venous oxygenation monitor* (ScvO₂ for septic shock; FDA Breakthrough Device Designation, 2022). No 2026 peer-reviewed validation data yet; watch.
> **Clinical-trial anchors (not ranked, non-optical/reference):** *Capnodynamic non-invasive mixed-venous SvO₂* (NCT06632197); *Continuous jugular venous oxygen saturation after cardiac arrest* (NCT06511999); *Noninvasive Internal Jugular Venous Oximetry* (NCT06004466); *SjvO₂ NIRS* trials (NCT04624009, NCT04778150).

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*Two genuinely new PA-microscopy instrumentation/accuracy papers surfaced today (§2.5 new to the ranked five; FD-PAM as a standing lead), plus a peer-review/indexing update on the DPF standing lead. The human/venous PA and vis-OCT anchors (§2.1–§2.4) are unchanged.*

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — the Topic-2 anchor)*
- **Year / Venue:** 2023 · preprint arXiv:2303.10775 (+ SPIE lineage; SPIE 8943E precursor). ⚠ arXiv egress-blocked today; abstract re-confirmed on two index snippets.
- **Link:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9/10 — human, in vivo, PA, *venous* (IJV).
- **Novelty:** Dual-wavelength PAT + ultrasound images the IJV in **7 healthy volunteers** at 5 fps; average IJV sO₂ ≈ **72 ± 7 %**, with US co-registration enabling temporal sO₂ tracking — true venous oximetry at depth, non-invasively.
- **Integration insights:** Proof that PA reaches a clinically relevant central vein through intact tissue; the imaging counterpart to the §1.4 pulse-based IJV device — same vessel, different sensing physics.

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): In-Vivo Human Radial-Vein sO₂ *(previously surfaced)*
- **Authors:** Sastry, Olick-Gibson et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley), 10.1002/advs.76366; PMC13334587; PubMed 42397001. ⚠ egress-blocked today; abstract re-confirmed via index snippet.
- **Link:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9/10 — solves the fluence problem for deep-tissue PA sO₂; reports in-vivo human values on the radial artery–vein pair (n = 8).
- **Novelty:** Uses high, known arterial oxygenation as a local in-situ **fluence reference** to correct spectral coloring, cutting median sO₂ error to **2.9 %** (vs 9.8 % for linear unmixing); human **venous sO₂ median 72.3 %** on the radial vein, robust through ex-vivo tissue up to 1.5 cm.
- **Integration insights:** Directly attacks the single biggest barrier to quantitative deep venous PA — unknown local fluence — using the artery as a self-calibrator, the same artery-as-reference logic §1.4 applies in the pulse domain. Today's §2.5 (fluence ceiling) is the microscopy-scale accuracy counterpart to APM+'s macroscopic fluence correction.

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced)*
- **Year / Venue:** 2024 · PACT venue; PMC11161372; PubMed 38855671. ⚠ egress-blocked; abstract re-confirmed via snippet.
- **Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** 8/10 — human, intravascular sO₂ heterogeneity and flow, PACT; recovers the parabolic laminar-flow wavefront inside a deep vein in vivo.
- **Novelty:** Turns intravascular oxygenation heterogeneity into a *contrast mechanism* for visualizing flow inside human vessels with PACT — oxygenation as a tracer — and demonstrates dynamic sO₂ imaging in a deep vein.
- **Integration insights:** Supports vessel-type discrimination from hemodynamics (the core unsolved venous problem — "which vessel is the vein?") and confirms human-scale PACT sensitivity to venous-range sO₂ gradients.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature), s43856-023-00288-8; PubMed 37095177; PMC10126115. ⚠ egress-blocked; metadata via snippet.
- **Link:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10126115/
- **Relevance:** 8/10 — resolves *per-vessel arterial and venous* retinal sO₂ non-invasively.
- **Novelty:** Adaptively removes vessel-specific spectral contaminants; RMSE ≈ 2.1 % vs pulse oximeter in major arteries, repeatability SD ≈ 2.3 % in *veins*; ex-vivo phantom agreement within 1 % bias across 0–100 % sO₂. Demonstrated across glaucoma, ischemia, DR, CRVO, sickle-cell retinopathy.
- **Integration insights:** Sets the accuracy ceiling for optical venous oximetry in an accessible vascular bed; the adaptive spectral-correction idea is transferable to PA/DOT venous inversion where spectral coloring dominates error (cf. §2.2).

### 2.5 — Maximum Fluence for Accurate Functional Photoacoustic Microscopy *(⭐ NEW to corpus this scan — first logged 2026-09-09 · PAM accuracy, venous-compartment-limited)*
- **Authors:** ⚠ search-derived — not fully page-confirmed (PMC/ScienceDirect egress-blocked). Associated with **Lidai Wang's group** (Lidai Wang appears as an author on the journal's author index for this article); full author list flagged for verification.
- **Year / Venue:** 2026 · ***Photoacoustics*** (Elsevier). **DOI 10.1016/j.pacs.2026.100851**; PMC13319516; PubMed 42389549; ScienceDirect PII S2213597926000571. Received 2026-04-22, accepted 2026-06-20, online 2026-06-24, collection Aug 2026. Metadata cross-checked on ≥3 snippets (PubMed + PMC + ScienceDirect).
- **Link / DOI:** https://doi.org/10.1016/j.pacs.2026.100851 · https://pubmed.ncbi.nlm.nih.gov/42389549/ ⚠ pages egress-blocked; metadata search-derived.
- **Relevance:** **7/10** — not a venous *measurement* paper, but the accuracy limit it establishes is **defined by the venous compartment**, making it directly load-bearing for any quantitative venous PA oximetry; included per the task's "technique directly transferable to venous" rule.
- **Novelty:** Establishes, for the first time rigorously, that in fast functional PAM **transient local thermal accumulation biases sO₂ even when laser power is within the ANSI safety limit**, and builds a numerical model for the **maximum accurate fluence** (~**0.41 mJ·cm⁻²** at 532/558 nm), validated in a blood phantom and mouse brain under long-term scanning. The striking venous-specific finding: the fluence ceiling **was set by the onset of a spurious *venous* sO₂ increase** — because veins' **lower flow velocity and longer blood-residence time** make transient thermal effects (and the associated measurement bias) appear *first and most strongly in the venous compartment*.
- **Integration insights:** This is a quiet but important result for the whole venous-PA program. It says the deoxygenated/venous compartment is not just harder to unmix (low absorption contrast, §2.2's spectral-coloring problem) but is also **the first place thermal-fluence artifact corrupts sO₂** — so venous PA oximetry has a *tighter* fluence budget than arterial. Any deep-vein PA method (§2.1 IJV PAT, §2.2 APM+, §2.3 PACT) that pushes fluence to gain depth/SNR must respect a venous-limited ceiling or it will systematically *over-read* venous sO₂. Concretely: pairs with APM+'s fluence-reference correction (§2.2) — one bounds the input fluence, the other corrects for the fluence that does get through.

> **Standing lead — NEW this run:** *Frequency-domain photoacoustic microscopy with resonant transducer and interferometric modulation for high-reliability sO₂ imaging* (Yong-Jae Lee, Tae Joong Eom [Pusan National Univ.], Lihong V. Wang [Caltech]; ***Photoacoustics*** 2026, **DOI 10.1016/j.pacs.2026.100834**; PMC13156710; PubMed 42111354; PII S2213597926000406). AOM-based interferometric modulation lets FD-PAM use a **high-Q resonant transducer** for simultaneous dual-wavelength sO₂, achieving clean spectral separation (SSIM 0.97) and **<2 % within-group sO₂ variation across oxygenated, mixed AND deoxygenated conditions** — i.e., reliability demonstrated *into the venous saturation range*, where absorption contrast is weakest. General PAM instrumentation (not venous-specific), so logged as a standing lead rather than ranked; a candidate front-end for the low-sO₂ regime venous imaging must nail.
> **Standing lead — UPDATED this run:** *A Novel Differential Pathlength Factor Model for Near-Infrared Diffuse Optical Imaging* (Kaiser Niknam, Mannu Bardhan Paul, Mini Das, Univ. Houston; arXiv:2602.00283, submitted 2026-01-30, v2 2026-08-25) is now **peer-reviewed and PMC/PubMed-indexed** (PMC13532703; PubMed 42687887). Monte-Carlo-derived distance/property-dependent DPF formulations reduce modified-Beer–Lambert error at small source–detector separations — underpinning every transcutaneous-NIRS venous method (§1.2, §1.4). Previously logged as a standing lead (07-25 / 08-03); recorded here as a genuinely-new-version/indexing update.

---

## Standing context leads (not ranked in the top-5)

- **Frequency-domain PAM with resonant transducer + interferometric modulation** (*Photoacoustics* 2026, 10.1016/j.pacs.2026.100834; PMC13156710; PubMed 42111354). *NEW this run — see §2.5 box.* High-reliability dual-wavelength sO₂ into the deoxygenated/venous range.
- **Novel Differential Pathlength Factor (DPF) model for NIR diffuse optical imaging** (arXiv:2602.00283; now PMC13532703 / PubMed 42687887, v2 2026-08-25). *Updated this run — peer-reviewed + PMC-indexed.* Underpins transcutaneous-NIRS venous methods (§1.2, §1.4).
- **Serial Dual-Wavelength Illumination for Retinal Vessel Oximetry Using a Conventional Fundus Camera** (*BMC Ophthalmology* 2026, 10.1186/s12886-026-05216-7; PMC13455296; PubMed 42576210). Stock fundus camera + serial 548/605 nm illumination measures per-vessel arterial and venous retinal sO₂ (venous MAD 8.4 ± 9.3 %, flagged as needing optimization). Low-cost camera-retrofit route to per-vessel venous readout.
- **Hyperspectral fundus system — High-Resolution Hyperspectral Imaging System for the Retina** (Tran M.H. et al.; *J. Biomed. Opt.* 31(3):036006, 2026; PMC12997856; PubMed 41858558). Snapshot hyperspectral + RGB + deep-learning pansharpening recovering per-vessel venule sO₂ (≈58 %) and diameter.
- **Transmissive-Detected Hyperspectral Imaging for Single-Vessel-Resolution Blood Oxygen Mapping** (*Photonics Research*/ScienceDirect S2765803125000343; PMC12707973, May 2026). TD-HSI dynamically monitors hypoxia-induced sO₂ changes across mouse ear/dorsal skin at single-vessel resolution — small-animal, tissue/vessel-level; relevant to arterio-venous vessel discrimination.
- **ISDC — Integrated Spectral and Depth Compensation for PA sO₂/THb** (*J. Biomed. Opt.* 31(2):026002, 2026; DOI 10.1117/1.JBO.31.2.026002; PMC12869027). Depth + spectral fluence correction, transferable to deep-vein PA oximetry.
- **Transabdominal Fetal Oximetry via Diffuse Optics** (Ghiasi Lab, UC Davis; arXiv:2509.21594; PMC12486049; PubMed 41040802). Deep diffuse-optics pulsatile oximetry; the **Exponential Pulsation Ratio (EPR)** + multi-detector ML is directly transferable to a respiration-modulated venous compartment.
- **Hybrid-Net / DL-driven quantitative spectroscopic PA** (arXiv:2512.15394; PMC13122505; PubMed 41990476). Joint vessel segmentation + sO₂ without explicit fluence estimation; general PA method.
- **Apple ML: PPGen + Hybrid Amortized Inference** (arXiv:2510.02073, 2025; *IOP* 10.1088/3049-477X/ae4a96). Technique-transfer lead — arterial/general PPG; extending PPGen's dynamic term to an explicit venous compartment is a concrete route to model-based SpvO₂.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood** (*Applied Optics* 65(6):1974, 2026; arXiv:2512.01458). Injectable ground-truth for validating multi-wavelength PA venous oximetry.
- **SFDI / wearable NIRS (tissue-level, not venous SvO₂):** *SFDI-net* (PMC12014942); *Advances in fully integrated wearable NIRS* (IOP 10.1088/2515-7647/ae6ae4, 2026). Superficial tissue StO₂ / venous-occlusion contrast, not intravascular venous sO₂.

---

## Cross-topic synthesis

1. **A modest but real cycle: two new *Photoacoustics* papers and a peer-review update, all in Topic 2; nothing new in Topic 1.** After the strongly-productive 09-08 run (four new papers, three true-venous), today reverted to the field's baseline: no new non-invasive *venous* measurement paper surfaced, and the two new items are PA-microscopy **accuracy/instrumentation** contributions rather than venous measurements. This is the honest texture of the niche — true venous work arrives in bursts, and most days the frontier moves on the *enabling* side (fluence, spectral separation, pathlength).

2. **The headline finding is subtle and venous-specific: the venous compartment sets the accuracy ceiling for functional PAM (§2.5).** The fluence-ceiling paper shows that transient thermal bias corrupts sO₂ *first in veins* — because low venous flow velocity and long blood-residence time let heat accumulate. Combined with the long-standing fact that veins are also the hardest compartment to *unmix* (low absorption contrast, §2.2's spectral-coloring problem), this means **venous PA oximetry is doubly disadvantaged**: tighter fluence budget AND weaker signal. Every deep-vein PA method (§2.1–§2.3) must respect a venous-limited fluence ceiling or systematically over-read venous sO₂.

3. **Three enabling threads are now converging on the low-sO₂/venous regime specifically.** (a) §2.5's fluence ceiling *bounds the input*; (b) the new FD-PAM instrument delivers **<2 % sO₂ reliability into the deoxygenated range** where contrast is weakest; (c) APM+ (§2.2) and the updated DPF model correct the *fluence/pathlength that does propagate*. Read together, the 2026 literature is quietly assembling a full error-budget toolkit for the exact regime — low saturation, deep tissue, weak contrast — that venous oximetry lives in.

4. **Accuracy anchors still frame the ceiling.** APM+ (§2.2, 2.9 % deep-tissue error, venous 72.3 %) and ADS-vis-OCT (§2.4, ~2.3 % venous repeatability) bracket the state of the art; the Topic-1 clinical methods (§1.1's 87 % concordance, §1.2's wide rSjvO₂ LoA) remain trend-grade. The consistent gap — non-invasive *venous* measurement is systematically harder than arterial — is exactly what today's enabling papers chip at.

5. **The near-term opportunity is unchanged: port Topic-2 machinery onto Topic-1 venous targets, now respecting a venous-tighter fluence budget.** The highest-leverage moves remain (a) EPR-style pulsation decomposition (fetal-diffuse-optics standing lead) applied to a respiration-modulated venous compartment, and (b) artery-as-reference fluence correction (APM+, §1.4) — but §2.5 adds a constraint every one of these must honor: keep fluence under the *venous* ceiling, not the arterial or ANSI one.

6. **Confidence caveat.** `WebFetch` to arXiv, PMC and ScienceDirect was egress-blocked today (all confirmed `EGRESS_BLOCKED`), so all metadata is search-snippet-derived (each item cross-checked on ≥2 snippets, the two new *Photoacoustics* items on ≥3 including DOI). For the new §2.5: title, DOI (10.1016/j.pacs.2026.100851), PMC/PubMed IDs, dates and the venous-fluence finding are corroborated across PubMed + PMC + ScienceDirect snippets; the **full author list could not be page-verified** (associated with Lidai Wang's group per the journal author index) — flagged ⚠. The FD-PAM standing lead's authors (Lee, Eom, L.V. Wang) and DOI (10.1016/j.pacs.2026.100834) are snippet-confirmed. Publisher-page verification of author lists should be repeated on the next scan where direct fetching is permitted.

---
*Scan generated 2026-09-09. Sources located and cross-verified via web search (≥2 independent index snippets per item; ≥3 for the two new Photoacoustics papers); direct publisher/preprint-page fetching unavailable this run due to the environment's network egress policy (arXiv, PMC and ScienceDirect all confirmed `EGRESS_BLOCKED` via direct WebFetch; IEEE Xplore, Optica, Wiley, De Gruyter, SPIE historically blocked). Metadata flagged ⚠ where it could not be confirmed on the source page.*
