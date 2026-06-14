# Venous Oxygen Research Scan — 2026-06-14

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.
**Prior scans in this repository:** 2026-06-10 (10 papers) and 2026-06-11 (10 papers). All 20 prior entries are excluded from this scan unless a genuinely newer version or finding warrants re-entry; none did. One paper (Hill et al. 2024, jugular optical SvO₂ sensor — prior scan 2026-06-10 Paper 1.1) re-surfaced in today's search and is noted here as **previously surfaced** rather than re-entered.
**Search window:** Emphasis on October 2025 – June 2026 publications not covered in prior scans. Sources searched: PubMed/PMC, arXiv, Optica (Biomedical Optics Express, Optics Letters, Applied Optics), SPIE / J. Biomed. Opt., *Photoacoustics*, Wiley (*J. Biophotonics*), Nature / *Eye*, MDPI (*Biosensors*, *Bioengineering*), Frontiers, Springer, AJP-Heart, ResearchGate, Semantic Scholar.
**Verification caveat:** Nature.com, PMC/PubMed, Wiley, Frontiers, SPIE, De Gruyter and journals.physiology.org all returned HTTP 403 to direct page fetches during this scan. Every entry below was therefore cross-checked across **at least two independent search-index sources**; per-entry verification notes state what was confirmed and what could not be directly read on a publisher page.

**Note on sparseness (read this first):** Genuinely new (2025–2026), *venous-specific*, non-invasive oxygen work remains a low-volume niche. After excluding the 20 papers from the two prior scans, **Topic 1 yielded only two solid new venous-specific entries** — the field's strongest recent results were already captured in earlier scans (jugular optical SvO₂, Mespere VO100, cardiac-MRI T₂ iSvO₂, wearable FD-NIRS). Topic 1 is reported honestly as sparse rather than padded with arterial-only SpO₂ or generic tissue-StO₂ work. The strongest *new* venous-specific optical work this cycle sits in Topic 2 (retinal SP-SFDI venous oximetry and fresh photoacoustic technique/calibration papers).

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

> **Sparseness flag:** Only two new entries meet the bar this scan. Both are reported with honest relevance scores. A handful of 2025 items were reviewed and rejected as out of scope (see "Reviewed and excluded" below).

### Paper 1.1
**Title:** Validation of Magnetic Resonance Imaging-Derived Venous Oxygen Saturation and Oxygen Consumption Measurements During Exercise
**Authors:** Rachel J. Skow, Stephen J. Foulkes, Dean R. Perkins, Justin S. Lawley, Corey R. Tomczak, Michael D. Nelson, Mark J. Haykowsky, Richard B. Thompson
**Year:** 2025 (published online May 6, 2025)
**Venue:** *American Journal of Physiology – Heart and Circulatory Physiology*, vol. 328, no. 6
**Link / DOI:** https://doi.org/10.1152/ajpheart.00134.2025
**Metadata verified:** Title, journal, year, volume/issue (328(6)), publication date, DOI, study design and sample sizes cross-confirmed across the AJP-Heart listing and a companion ISMRM 2025 abstract (#0349). Full author list recovered from a secondary search index. Publisher page returned HTTP 403 — author list and exact page/article number not directly read on source (*flagged*).
**Relevance score:** 8 / 10
⚠️ *Non-optical method (cardiac/peripheral MRI susceptometry-based oximetry); included because Topic 1 covers non-invasive venous oxygen monitoring broadly.*

**Novelty:** Validates MRI **susceptometry-based oximetry (SBO)** for measuring true intravascular **venous** O₂ saturation *during dynamic exercise* — a regime where motion normally defeats MRI oximetry. Venous saturation was measured directly in the antecubital vein (handgrip protocol, n = 14) and the inferior vena cava (incremental step-ergometry protocol, n = 21), validated against direct blood-gas sampling (iSTAT) and against pulmonary VO₂ via the Fick principle. Reports excellent repeatability and validity, and derives whole-body VO₂ from non-invasively measured Fick determinants.

**Integration insights:** This is the cleanest *new* true-venous-blood result of the scan and a direct intellectual sibling of the cardiac-MRI T₂ iSvO₂ work entered on 2026-06-11 (McDiarmid et al., JACC Advances): both exploit haemoglobin-deoxygenation physics (magnetic susceptibility / T₂ relaxation) to recover absolute venous saturation non-invasively. The exercise paradigm parallels the venous-occlusion and fist-clench perturbations used by optical groups (Zachia Alan 2022; Kong/PACT 2024) to amplify venous signal. As an absolute, blood-sample-validated venous SvO₂ reference obtainable in a moving subject, SBO-MRI is a strong calibration anchor against which wearable optical venous oximeters (NIRS, PA) can be cross-validated — particularly because it delivers regional venous saturation at a defined vessel (IVC, antecubital) rather than a tissue average.

---

### Paper 1.2
**Title:** Machine Learning-Based VO₂ Estimation Using a Wearable Multiwavelength Photoplethysmography Device
**Authors:** Chin-To Hsiao, Carl Tong, Gerard L. Coté
**Year:** 2025 (published March 24, 2025)
**Venue:** *Biosensors* (MDPI), vol. 15, no. 4, article 208
**Link / DOI:** https://doi.org/10.3390/bios15040208
**Metadata verified:** Title, full author list, journal, volume/issue/article number, DOI, and publication date confirmed via MDPI listing and Semantic Scholar; PMC mirror (PMC12024819) corroborates. PMC/MDPI direct fetch blocked (403); content summary from search-index text.
**Relevance score:** 5 / 10
*(Tissue-level / whole-body oxygen-consumption surrogate — NOT a direct venous SvO₂ measurement. Included as the best new wearable-optical entry with an explicit venous link via the Fick relationship.)*

**Novelty:** A wearable multiwavelength PPG device plus machine-learning models to estimate oxygen consumption (VO₂) non-invasively and continuously. The work targets the same form-factor trajectory as the wearable FD-NIRS papers entered on 2026-06-11, but aims at a metabolic readout (VO₂) rather than a hemoglobin saturation per se.

**Integration insights:** VO₂ connects to venous oxygenation through the Fick principle — VO₂ = CO × (CaO₂ − CvO₂) — so any accurate non-invasive VO₂ estimate constrains the arterio-venous oxygen-content difference and, given arterial saturation, the venous content. The relevance is therefore indirect: this is not vessel-specific venous oximetry, but it advances the wearable multiwavelength-PPG hardware/algorithm stack that a future venous-selective oximeter would share. The honest limitation is that PPG samples a mixed (predominantly arterial-pulsatile) bed; extracting a venous-specific component would require the respiration-frequency / venous-pulse isolation strategies seen in the jugular-sensor and spiroximetry literature (prior-scan Hill et al. 2024).

---

**Reviewed and excluded from Topic 1 (with reasons):**
- *Hill, Campbell, Chase & Pretty (2024), "Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins"* (De Gruyter, *Curr. Dir. Biomed. Eng.* 10(4):295–298) — **previously surfaced**; already entered as Paper 1.1 in the 2026-06-10 scan. Re-confirmed during today's search but not re-entered (no new version or finding).
- *Near-infrared "spiroximetry" (respiration-frequency-filtered NIRS) for cerebral venous SvO₂* — a genuinely venous-specific optical method, but the substantive papers are 2002/2013; no new 2025–2026 publication surfaced. Noted in synthesis as a methodological lead.
- *Pediatric goal-directed care using continuous superior-caval venous O₂ saturation (2025 RCT) and a 2025 editorial "the body wants oxygen!"* — venous saturation is **invasively** measured (catheter); out of non-invasive scope.
- *SPIE "Diffuse Optical Spectroscopy and Imaging X" (Vol. 13935, 2025)* — likely venue for new venous-DOSI work, but no individual venous-specific paper, author list, or DOI could be isolated (volume page 403). Flagged as a lead to chase, not a confirmed entry.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

### Paper 2.1
**Title:** Assessing and Monitoring Abnormal Retinal Blood Circulation for Early Detection of Pre-Structural Damage and Enhanced Diabetic Retinopathy Staging Using Non-Invasive, High-Resolution Biophotonic Imaging Technology
**Authors:** A. Basiri, C. Luo, M. Shokoohi-Yekta, et al.
**Year:** 2025
**Venue:** *Eye* (Nature Publishing Group), vol. 39, pp. 2872–2883
**Link / DOI:** https://doi.org/10.1038/s41433-025-04032-5 (PMID 41015611)
**Metadata verified:** Title, journal (*Eye*), year, volume (39), page range (2872–2883), DOI, PMID, lead authors, the SP-SFDI/BioxyDR method, cohort (63 DR + 60 DM-no-DR + 18 controls), and the venous-specific result (**retinal venous αSO₂ differed significantly between controls and patient groups, p = 0.007**) cross-confirmed across two independent search indices. Nature page returned 403 — full author list and exact venous αSO₂ numeric values not directly read on source (*flagged*).
**Relevance score:** 8 / 10
*(Vessel-resolved retinal oximetry that explicitly reports a venous saturation analogue (αSO₂); it is a tissue/vasculature αSO₂ rather than a blood-gas-calibrated venous sO₂, so partly surrogate — but venous-vessel-attributed.)*

**Novelty:** Introduces **Saccadic-Phase Spatial Frequency Domain Imaging (SP-SFDI)**, a physics-based retinal-oximetry algorithm that recovers an oxygen-saturation analogue (αSO₂) from just two snapshots capturing phase shifts in spatially modulated light, claiming sensitivity to oxygenation changes < 3%. Its first clinical application, "BioxyDR," stages diabetic retinopathy from superficial retinal-vasculature αSO₂, and crucially reports a *venous-specific* difference across DR severity.

**Integration insights:** This is the strongest *new* optical, venous-attributed result of the scan and extends the SFDI thread from prior scans (SFDI-net, 2026-06-10 Paper 2.5; multimodal SFDI benchmarking, 2026-06-11 Paper 1.5) from tissue-average StO₂ toward *single-vessel, venous-resolved* saturation. It joins visible-light OCT (Paper 2.4 below; prior-scan vis-OCT review) as evidence that the retina is the one human bed where vessel-specific venous oximetry is routinely tractable non-invasively. The open translational question is identical to vis-OCT's: the spatial-frequency-domain venous separation demonstrated in the thin, transparent retina must be adapted to thicker, opaque peripheral beds (external jugular, basilic, cephalic) before it informs systemic venous monitoring. The snapshot (two-frame) acquisition is attractive for motion-robust dynamic imaging.

---

### Paper 2.2
**Title:** Improved Sensitivity in Large Field-of-View Multispectral Laser-Scanning Photoacoustic Microscopy for Measuring Oxygen Saturation In Vivo
**Authors:** Mohsin Zafar, Amir Khansari, Rayyan Manwar, Kamran (Mohammad R. N.) Avanaki
**Year:** 2026
**Venue:** *Journal of Biophotonics* (Wiley), vol. 19, no. 3, article e202500378
**Link / DOI:** https://doi.org/10.1002/jbio.202500378
**Metadata verified:** Title, full author list, journal, volume/issue (19(3)), article number (e202500378), DOI, and NIH funding cross-confirmed across the Wiley listing and the author's profile. Wiley page returned 403 — venous-specific in-vivo numbers not directly read (*flagged*). One index ambiguously rendered the 2026 designation; volume 19(3) is the best-supported reading.
**Relevance score:** 6 / 10
*(Vessel-resolved label-free sO₂ imaging — not venous-exclusive, but PAM distinguishes arteries from veins by definition; directly transferable to venous sO₂.)*

**Novelty:** Addresses a core hardware limitation of laser-scanning photoacoustic microscopy (PAM): low detection sensitivity from a flat transducer in non-coaxial alignment with the optical scan. The work presents a large-field-of-view multispectral PAM (with stimulated-Raman-scattering-generated wavelengths) that recovers in-vivo sO₂ at improved sensitivity over a wider area.

**Integration insights:** Fresh (2026) photoacoustic technique work in the same family as the prior scans' PA papers (IJV PA, PACT flow, PAVT). The sensitivity and field-of-view gains are exactly the levers needed to image larger and deeper vessels — i.e., to move PA sO₂ from microvasculature toward named veins. Because PAM's sO₂ contrast is inherently vessel-resolved (an artery and an adjacent vein are separable by their spectra), improving its sensitivity and coverage is a prerequisite for label-free venous sO₂ mapping; the SRS-multiwavelength front end also complements the spectral-unmixing/fluence-correction work entered on 2026-06-11 (Feng spectral-coloring correction; SPOI-AE).

---

### Paper 2.3
**Title:** Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations
**Authors:** Léa Davenet, Arthur Billon, Jacques Battaglia, S. Lori Bridal, Jérôme Gateau
**Year:** 2026 (arXiv preprint December 1, 2025; journal version 2026)
**Venue:** *Applied Optics* (Optica), vol. 65, no. 6, pp. 1974–1982 — also arXiv:2512.01458
**Link / DOI:** https://opg.optica.org/ao/abstract.cfm?uri=ao-65-6-1974 ; preprint https://arxiv.org/abs/2512.01458
**Metadata verified:** Title, full 5-author list, dual venue (*Applied Optics* 65(6):1974–1982 and arXiv:2512.01458), arXiv submission date, and the methodology cross-confirmed across the arXiv listing and the Optica abstract URL. Both pages returned 403 — exact Optica DOI string not directly read; AO citation taken from the canonical opg.optica.org path (*flagged*). Affiliation: Sorbonne Université / Laboratoire d'Imagerie Biomédicale (LIB), Paris.
**Relevance score:** 6 / 10
*(Calibration/phantom methodology — not venous imaging itself, but directly enables validation of venous-range PA sO₂.)*

**Novelty:** A practical recipe for inorganic (sulfate-based) aqueous solutions that mimic whole blood's photoacoustic response at *selected* oxygenation levels across 700–850 nm — matching both optical absorption *and* the Grüneisen coefficient. These stable, injectable phantoms let multi-wavelength PA systems be tested for their sensitivity and spectral capability to estimate blood oxygenation, without the handling instability of real blood.

**Integration insights:** Quantitative venous PA oximetry lives or dies on validation, and venous saturations (typically ~60–75%) sit in a range where spectral-unmixing errors and fluence/spectral-coloring artifacts are most consequential. A stable phantom tunable to *chosen* sO₂ values — including the venous band — is exactly the ground-truth target the deep-learning inversion papers from prior scans (Hybrid-Net, SPOI-AE) and the spectral-coloring correction (Feng et al.) need for objective benchmarking. This is plumbing, but essential plumbing: it provides the venous-range calibration standard against which any "non-invasive venous sO₂ via PA" claim should be measured.

---

### Paper 2.4
**Title:** The Path to Clinical Translation for Visible-Light Optical Coherence Tomography in Retinal Imaging
**Authors:** Not independently verified (vis-OCT retinal-oximetry group; author list not confirmed — *flagged*)
**Year:** 2025 (July)
**Venue:** *Taiwan Journal of Ophthalmology*
**Link / DOI:** https://doi.org/10.4103/tjo.tjo-d-25-00078 (PMC12456912)
**Metadata verified:** Title, year, venue, DOI stem and PMC ID cross-confirmed across PMC and LWW/Ovid listings. Author names could NOT be verified (PMC/LWW pages 403) — *flagged*. This is a **review**, distinct in journal, authorship and title from the MDPI *Bioengineering* vis-OCT review entered on 2026-06-11 (Paper 2.5).
**Relevance score:** 5 / 10
*(Review article; covers vessel-resolved retinal arterial AND venous sO₂ via vis-OCT, down to capillary level.)*

**Novelty:** A 2025 synthesis specifically framed around *clinical translation* of vis-OCT retinal oximetry — light sources, balanced detection, spectroscopic processing, and the engineering needed to move from lab to clinic. It updates and complements the broader vis-OCT review captured last scan, with a translation (not just technology) emphasis.

**Integration insights:** Vis-OCT remains the most mature vessel-specific non-invasive venous-oximetry modality in humans (retinal veins routinely measured at ~60–70% sO₂). This review consolidates what the field still needs for the clinic and, read alongside the new SP-SFDI paper (2.1), shows two convergent optical routes to retinal *venous* saturation. The transferable assets — spectroscopic backscatter modeling, adaptive spectral-contaminant removal, capillary-level vessel resolution — are the methodological reference for any attempt to bring vessel-specific venous oximetry to accessible peripheral veins.

---

### Paper 2.5
**Title:** Emerging Photoacoustic Imaging Techniques for Peripheral Arterial Disease
**Authors:** Yide Zhang, Lihong V. Wang
**Year:** 2025
**Venue:** *Current Treatment Options in Cardiovascular Medicine*, vol. 27, article 56
**Link / DOI:** https://doi.org/10.1007/s11936-025-01113-2 (PMC12394336)
**Metadata verified:** Title, authors (Yide Zhang, Lihong V. Wang), year, venue, volume/article number, DOI and PMC ID cross-confirmed across Springer and PMC listings. Pages 403 — venous-specific passages not directly read (*flagged*).
**Relevance score:** 5 / 10
*(Review framed around peripheral ARTERIAL disease; included because its PA sO₂ / blood-volume techniques are directly transferable to veins — the Wang group's PAVT, cited here, already images deep veins.)*

**Novelty:** An authoritative 2025 review of the PA imaging toolkit for peripheral vasculature — quantitative sO₂, regional blood volume, and deep haemodynamics — from the group behind the deep-vein PAVT and IJV-PA work surfaced in prior scans.

**Integration insights:** Although framed for arterial disease, the technique inventory (multi-wavelength sO₂ quantification, deep-flow PAVT, fluence handling) is medium-agnostic: the same contrast that maps an arterial sO₂ deficit maps venous sO₂. Included specifically because it extends the Wang-lab PA lineage (IJV PA → PACT flow → PAVT) that this project tracks as the most direct route to clinical deep-vein optical oximetry, and because it surveys the depth-reaching hardware (>5 mm) that systemic venous monitoring requires. Honest caveat: this is transferable-context, not venous-specific primary data.

---

**Honorable mentions (verified, lower venous-relevance, not ranked):**
- *"Photoacoustic Imaging: a Unique Imaging Examination for the Assessment of Diabetic Vascular Disease"* — Chen & Xia, *Frontiers in Clinical Diabetes and Healthcare* (Nov 7, 2025), DOI 10.3389/fcdhc.2025.1651868 (PMC12634374). PA review covering arterial + venous vessel sO₂ in diabetic micro/peripheral vasculature.
- *"Advancements in Photoacoustic Detection Techniques for Biomedical Imaging"* — *npj Acoustics* (2025), DOI 10.1038/s44384-025-00005-w. Reviews PA detection hardware (incl. optical sensing / PARS for in-vivo sO₂); not venous-specific.

---

## Cross-Topic Synthesis

### What changed this scan
The two prior scans had already captured the field's headline venous-specific results (jugular optical SvO₂, Mespere VO100 ICU validation, cardiac-MRI T₂ iSvO₂, wearable FD-NIRS, transmissive HSI, deep-tissue PA thrombosis oximetry, vis-OCT). Today's new, verifiable additions cluster into three movements:

**1. A second non-optical "absolute venous reference" matures.** Paper 1.1 (MRI susceptometry-based oximetry during exercise) joins last scan's cardiac-MRI T₂ iSvO₂ as a blood-sample-validated, vessel-specific, *absolute* venous SvO₂ obtainable non-invasively — now even in a moving subject. Two independent MRI physics routes (susceptibility, T₂) to absolute venous saturation now exist. For the optical program, these are not competitors but calibration anchors: they define the venous-saturation ground truth (at the IVC, antecubital, RV) against which wearable NIRS/PA devices should be cross-validated, at scale, in patients already undergoing MRI.

**2. Retinal vessel-resolved venous oximetry gains a second optical modality.** SP-SFDI (Paper 2.1) reports a *venous-specific* αSO₂ DR-staging signal, sitting alongside the maturing vis-OCT translation effort (Paper 2.4). The retina remains the one human bed where vessel-specific venous saturation is routinely measured non-invasively, and it now has two convergent optical approaches (spatial-frequency-domain phase imaging and visible-light OCT spectroscopy). The recurring translational gap is unchanged: extending single-vessel venous separation from the thin, transparent retina to thick, opaque peripheral beds.

**3. Photoacoustic venous oximetry is being de-risked from both the hardware and the validation ends.** Paper 2.2 attacks PAM's sensitivity/field-of-view limits (a prerequisite for imaging named veins), and Paper 2.3 supplies tunable, venous-range blood-mimicking phantoms (the ground truth needed to benchmark the deep-learning unmixing/fluence-correction methods entered last scan). Together with the transferable PA-for-PAD review (Paper 2.5), the PA pipeline is advancing on technique, calibration, and clinical framing simultaneously — even though no *new* in-vivo human venous-PA sO₂ result appeared this cycle.

### Persisting gaps (carried forward, still open)
- **No new in-vivo human venous-PA sO₂ result this scan.** The 2023 IJV-PA proof-of-concept (prior scan) remains the reference; clinical-scale validation (cf. the 79-patient VO100 study and the 628-patient MRI cohort) does not yet exist for photoacoustic venous oximetry.
- **The MRI validation-scale gap widens.** With two MRI venous-SvO₂ methods now validated against blood gases, the bar for optical methods rises; embedding wearable NIRS/PA alongside routine MRI venous oximetry is the obvious — and still untaken — large-cohort validation design.
- **Retinal-to-peripheral transfer remains unproven.** Both new optical venous results (SP-SFDI, vis-OCT) are retinal. No 2025–2026 feasibility study extends vessel-specific venous separation to an accessible systemic vein.
- **Calibration standards are arriving before the venous imaging that needs them.** Paper 2.3's venous-range phantoms are ready; the field should now use them to publish *like-for-like* venous-sO₂ accuracy numbers across PA inversion methods (Hybrid-Net, SPOI-AE, spectral-coloring correction) rather than reporting accuracy on heterogeneous, non-comparable targets.

### Bottom line
A modest but honest scan: **one strong new true-venous paper (MRI SBO, 1.1)**, **one strong new optical venous-attributed paper (SP-SFDI retinal, 2.1)**, and a useful cluster of PA technique/calibration and vis-OCT translation work. Topic 1 is genuinely sparse this cycle and is reported as such; the most actionable near-term venous-oximetry signal continues to come from (a) MRI as the absolute-reference calibrator and (b) the retina as the proving ground for vessel-specific optical venous saturation.
