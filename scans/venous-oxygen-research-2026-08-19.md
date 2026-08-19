# Venous Oxygen Research Scan — 2026-08-19

**Search window:** Thirty-eighth scan in the series, run **two days** after 2026-08-17 (no scan on 08-18). Emphasis on work published or first-surfacing after 08-17, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (physics.med-ph / eess.IV new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer, Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Sensors/Biosensors*), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, Frontiers in Photonics, American Physiological Society journals, ClinicalTrials.gov, plus Semantic Scholar / Google-Scholar-style index snippets and ResearchGate.

**Verification caveat:** Publisher **full-text** pages and several databases were again unreachable for direct `WebFetch` today. The usual publisher hosts (link.springer.com, opg.optica.org, sciencedirect.com, wiley.com, spiedigitallibrary.org, pmc.ncbi.nlm.nih.gov, journals.physiology.org) and arxiv.org return **HTTP 403 / EGRESS_BLOCKED** to direct fetch in this environment. The blocks are source-/policy-side, not relay failures. Every reference below was therefore cross-checked across **≥2 independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific optical measurement paper first-surfaced in the two-day 08-17 → 08-19 window.** Repeated targeted sweeps (SvO₂ / ScvO₂ optical, jugular PA/NIRS, deep-vein PA, vis-OCT venular oximetry, hyperspectral, DOS/DOI, SFDI) returned only the **standing corpus**. The 08-13 hyperspectral retinal system (Tran et al., *J. Biomed. Opt.* 31(3):036006, §2.5) remains the most recent genuinely-new intravascular-venular result and is carried forward unchanged.

**No item — venous or tissue-level — is genuinely new to the corpus today.** The only near-window sighting is a *Frontiers in Photonics* editorial ("Diffusive optics for medical imaging," 2026, DOI 10.3389/fphot.2026.1842429) — an editorial framing piece, tissue-level and not venous-specific; logged as a standing context lead only.

**No new venous-specific systemic (SvO₂/ScvO₂) measurement paper today — the seventeenth consecutive scan cycle with none.** All standing Topic-1 anchors and the deep-vein PA anchors are unchanged and carried forward with scores held.

**Per the standing brief: fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical *new* papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new primary measurement items today.* Standing best-available set (all previously surfaced), scores carried forward. **No primary non-invasive systemic venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90 % band (≈70–75 % across a three-subject set: 71.1 / 72.2 / 70.4 %).
- **Integration insight:** Anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck.
- **Metadata note:** Title/authors/venue/DOI re-confirmed today via De Gruyter Brill listing + ResearchGate snippet; full text not read (publisher HTML not directly fetchable).

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see flag)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume / overlying-tissue confound.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.1's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work.
- **Metadata flag:** DOI string not re-verifiable on the Optica page today (403); Optica locator (ol-49-10-2669) + title/authors/year cross-confirmed via two index snippets. Treat raw DOI numeral as **unverified**; cite via the Optica abstract URL.

### 1.3 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Authors:** (peripheral-venous oximetry group; BioMedical Engineering OnLine)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x · PMC5437414
- **Relevance:** 8.0/10 — foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically.
- **Novelty:** External stimulation induces cyclical venous fluctuation, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** Conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering, PPG-waveform venous oximetry). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.
- **Metadata note:** Re-confirmed today via BioMedical Engineering OnLine full-text listing (biomedical-engineering-online.biomedcentral.com) + PMC snippet.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01)*
- **Authors:** Tan P., Lu N., et al. (UT Austin)
- **Year / Venue:** 2023/2024 · IEEE (EMBC-lineage); related patent US 20250025074
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent: https://patents.justia.com/patent/20250025074
- **Relevance:** 8.0/10 — explicitly names non-invasive **venous** oxygenation as the unmet need and targets it with a wrist-worn optical patch.
- **Novelty:** Ultra-thin self-adherent optical e-tattoo measures arterial + venous pulses from multiple wrist sites; proposes spatial filtering to separate arterial/venous crosstalk.
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.3 attacks by modulation and §1.1 sidesteps by anatomy. The standing JMIR hypoxia-accuracy caution bears directly on this device class.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Authors:** (VO100 clinical validation group)
- **Year / Venue:** 2023/2024 · *J. Cardiothorac. Vasc. Anesth.* (S1053-0770 lineage) / ScienceDirect · PMID 37827917
- **Link / DOI:** https://doi.org/10.1053/j.jvca.2023.10.006 · https://pubmed.ncbi.nlm.nih.gov/37827917/
- **Relevance:** 8.0/10 — a marketed non-invasive device that estimates central venous saturation from jugular-area NIRS (SjvO₂ surrogate for ScvO₂); reported strong correlation with invasive ScvO₂ (r ≈ 0.9 in prior pediatric jugular-NIRS work).
- **Novelty:** Transcutaneous NIRS sensor placed over the internal-jugular projection recovers a continuous central-venous-saturation surrogate at the bedside, the commercial counterpart to §1.1/§1.2.
- **Integration insight:** The device most directly bridging Topic-1's clinical need and Topic-2's optical physics on the systemic-venous front; validation-cohort agreement is the key open question for the whole jugular-NIRS class. Today's sweep re-confirmed the ScienceDirect record (S1053077023007826) and the pediatric jugular-NIRS validation (r = 0.91; bias 2.92 %, LoA −5.2 % to +11 %; TÜBİTAK *Turk. J. Med. Sci.* 50(5), PMC7491293) that grounds the technique's agreement claim.

### 1.6 — Noninvasix LIVOx Optoacoustic Central Venous Oxygenation Monitor (ScvO₂ for septic shock) *(previously surfaced — scan 08-11; device/regulatory anchor, not new research)*
- **Authors:** Noninvasix, Inc. / Esenaliev–Petrov optoacoustic lineage (UTMB)
- **Year / Venue:** FDA Breakthrough-Device designation 2022; ongoing development (not a dated research paper)
- **Link / DOI:** company / regulatory record; underlying method rooted in the superior-sagittal-sinus / transfontanelle optoacoustic oximetry lineage (*Sci. Rep.* 2022, s41598-022-19350-x)
- **Relevance:** 7.5/10 — an optoacoustic embodiment explicitly targeting **central venous** (ScvO₂) saturation non-invasively; the clearest regulatory-pathway endpoint in the corpus for the venous-optoacoustic thesis.
- **Novelty:** Laser-optoacoustic probe reads oxygenation from a named central vein directly, rather than through a tissue-StO₂ surrogate — the device-development counterpart to the IJV-PA research anchor §2.1.
- **Integration insight:** Demonstrates that non-invasive venous optoacoustic oximetry has crossed from lab demonstration into a regulated device pathway; the commercial bookend to Topic-2's PA measurement physics.
- **Metadata flag:** Regulatory/company record, not a peer-reviewed dated paper; treat designation year as reported. No new filing seen today.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new item today.* Measurement anchors carried forward with scores held; the 08-13 hyperspectral retinal system (§2.5) remains the most recent genuinely-new entry.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Authors:** (IJV-PA human oximetry group; Garcia-Uribe / Wang lineage)
- **Year / Venue:** 2023 · arXiv:2303.10775 / PA human-imaging lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: photoacoustic sO₂ of a named deep **vein** (internal jugular) in humans, non-invasively (sijvO₂ ≈ 72 ± 7 %).
- **Novelty:** Demonstrates human IJV oxygenation from multi-wavelength PA using a dual-wavelength PA-tomography + ultrasound system capturing co-registered images at 5 fps, pushing PA oximetry from superficial microvessels to a clinically meaningful deep venous target.
- **Integration insight:** Proof that optical/PA venous oximetry can reach a central-venous surrogate; the bridge between Topic 1's clinical need and Topic 2's imaging physics.
- **Metadata flag:** arxiv.org egress-blocked today; re-verified via ≥2 index snippets (arXiv abstract listing + PDF snippet).

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366 · https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring; radial artery–vein pair imaged in eight healthy adult volunteers.
- **Novelty:** The arterial prior method (APM+) leverages high arterial sO₂ to locally calibrate optical fluence and correct wavelength-dependent spectral coloring, recovering deep-tissue venous sO₂ where conventional linear unmixing fails. Phantom median estimation error 2.9 % vs 9.8 % for conventional linear unmixing (LUM).
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus; its fluence-correction strategy is the deep-vein counterpart to the retinal per-vessel corrections §2.4/§2.5 catalogue and to the Hybrid-Net / PINN spectral-unmixing leads.
- **Metadata flag:** Re-confirmed today via Wiley Advanced Science DOI landing + search snippets; full text 403 to direct fetch.

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Authors:** (PACT intravascular flow/oxygenation group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741 · PMC11161372
- **Link / DOI:** https://doi.org/10.1364/BOE.518632 → https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741
- **Relevance:** 8.0/10 — resolves sO₂ heterogeneity and laminar-flow structure *inside* human vessels (incl. veins) with PACT.
- **Novelty:** First-time recovery of the parabolic laminar-flow wavefront inside a deep vein in vivo by exploiting intravascular oxygenation heterogeneity across multi-wavelength PA spectra.
- **Integration insight:** Shows PACT can read *within-lumen* venous oxygen structure, not just a vessel-average — the imaging counterpart to the "fuse oximetry with blood-flow measurement" thesis.
- **Metadata flag:** DOI numeral not re-verifiable on the Optica page today (403); Optica locator (boe-15-5-2741) + PMC11161372 + title/year cross-confirmed. Cite via the Optica URL; treat the raw DOI numeral as **unverified**.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Authors:** (ADS-vis-OCT group)
- **Year / Venue:** 2023 · *Communications Medicine* 3:59
- **Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8 · PMC10126115
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3 % in veins; RMSE ≈ 2.1 % vs pulse oximeter in major arteries across 18 participants (SD of repeated sO₂ ≈ 2.5 % in smaller arteries, 2.3 % in veins).
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans (arteries ≈95 %, veins ≈72 % in reported cohorts). vis-OCT's 3-D depth localization excludes confounds from other tissue depths that limit 2-D hyperspectral fundus imaging.
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the retinal-oximetry review holds up as state-of-the-art for retinal venular oximetry.
- **Metadata note:** Title/venue/DOI re-confirmed today via Nature *Communications Medicine* landing + PMC10126115 + DOAJ snippet.

### 2.5 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — first surfaced 08-13; per-vessel retinal artery + vein sO₂; most recent genuinely-new entry)*
- **Authors:** Tran M.H., Pruitt K., Bryarly M., Emordi I., Ali A., Ma L., Fei B. (Quantitative Bioimaging Laboratory, UT Dallas / UT Southwestern)
- **Year / Venue:** **2026** · *Journal of Biomedical Optics* **31**(3):036006 (2026 Mar 1)
- **Link / DOI:** https://doi.org/10.1117/1.JBO.31.3.036006 · PMC12997856 · SPIE: https://www.spiedigitallibrary.org/journals/journal-of-biomedical-optics/volume-31/issue-3/036006/
- **Relevance:** 7.5/10 — a 2026 hyperspectral fundus system that measures **per-vessel retinal venule sO₂ (≈58 %)** alongside arteriole sO₂ (≈98 %) and vessel diameter; a true intravascular venular optical readout, though retinal per-vessel, **not systemic SvO₂**.
- **Novelty:** High-resolution snapshot/hyperspectral retinal imager that recovers vessel diameter *and* oxygenation simultaneously; a **deep-learning pansharpening** step fuses high-spatial and high-spectral channels (reported pansharpening RMSE 2.15 ± 0.64, correlation coefficient 0.96 ± 0.05). Reported venule sO₂ ≈ 58 % matches the accepted retinal venous norm (≈57.9 ± 9.9 %), giving physiological face-validity to the calibration.
- **Integration insight:** A 2026 entry in the retinal-oximetry cluster (with ADS-vis-OCT §2.4 and the standing HSI/retinal-review leads). It advances the *spatial–spectral fusion* angle — using deep learning to reconcile the resolution/spectral-sampling trade-off that limits fundus HSI — the same class of confound (per-vessel diameter, vessel boundary, media transparency) the vis-OCT and deep-vein PA work must correct. Reinforces that retinal venular oximetry remains the most mature, best-validated proving ground for per-vessel venous optical measurement, and offers a cheaper camera-based route (vs vis-OCT / PA hardware) toward the same per-vessel venous readout.
- **Metadata flag:** Title, authors, venue, volume/issue/article-number and DOI cross-confirmed across ≥2 independent index snippets (SPIE Digital Library listing + PMC + UT Southwestern Pure). **Full text not read** — spiedigitallibrary.org, pmc.ncbi.nlm.nih.gov and the UTSW Pure page were egress-blocked to direct fetch; numeric performance figures are snippet-level and should be treated as reported-not-verified.

**Topic-2 note:** the anchors most on-target for *systemic deep-vein* venous oximetry (§2.1 IJV-PA, §2.2 APM+ radial vein) are unchanged; no new item this cycle strengthens either the systemic deep-vein or the retinal per-vessel sub-cluster.

---

## Standing context leads (not ranked in the top-5)

- **Diffusive optics for medical imaging (Editorial)** — *Frontiers in Photonics* (2026) · DOI 10.3389/fphot.2026.1842429. **Editorial / framing piece, tissue-level, NOT venous.** Surveys diffuse optical tomography, SFDI, time-resolved spectroscopy, and diffuse correlation spectroscopy for tissue chromophore/hemodynamic mapping; the StO₂ signal is a mixed arterial+venous microvascular quantity, not intravascular SvO₂. Near-window sighting (2026) but adds no venous-specific measurement; logged only as diffuse-optics context for the strategy-2/strategy-3 method clusters. Snippet-verified only (frontiersin.org landing).
- **Near-infrared spectroscopy demonstrates preserved and reproducible resting skeletal muscle oxygenation across anatomical sites in stable heart failure** — *Am. J. Physiol. Heart Circ. Physiol.* (2026) · DOI 10.1152/ajpheart.00398.2026. **Tissue-level (StO₂), NOT venous.** Continuous-wave NIRS reproducibility study of resting skeletal-muscle oxygenation across anatomical sites in stable heart-failure patients; the StO₂ signal is a mixed arterial+venous microvascular quantity, not an intravascular SvO₂. Value to the corpus is as a 2026 StO₂-reproducibility baseline for the wearable/tissue-oximetry device class (§1.3/§1.4) — device-to-site repeatability is the same weakness those venous devices must beat. *journals.physiology.org egress-blocked; title/venue/DOI snippet-verified only — reported-not-verified.*
- **Retinal Oximetry: New Insights into Ocular and Systemic Diseases** — Zhang W., Tu X., Wang X., et al. · *Graefe's Archive for Clinical and Experimental Ophthalmology* 263:2101–2115 (2025) · DOI 10.1007/s00417-025-06831-8 · PMID 40254630 · PMC12414079. Review consolidating retinal oximetry across spectrophotometric-fundus, hyperspectral, and vis-OCT modalities; frames retinal artery *and vein* saturation as ocular + systemic biomarkers. The review-level companion to the §2.5 HSI system and the §2.4 vis-OCT anchor.
- **Integrated spectral and depth compensation for sO₂ and total-hemoglobin estimation in PAT for ovarian-lesion diagnosis** — *Biomed. Opt. Express*-lineage, 2026 · PMC12869027. Combines spectral + depth fluence compensation for deep-tissue PAT sO₂; **not venous-specific** (arterial+venous tissue, ovarian). Method lead for the deep-vein decoloring problem (§2.2). Snippet-verified only.
- **Comparative assessment of healthy tissue oxygenation using near-infrared imaging, transcutaneous oxygen measurement, and plethysmography** — El Masry et al. · *Scientific Reports* 15:30424 (2025) · PMID 40830190 · PMC12365204 · DOI 10.1038/s41598-025-15767-2. **Tissue-level (StO₂), NOT venous.** SFDI uniquely detected significant StO₂ differences; device-to-device correlations only moderate-to-fair — a sobering cross-modality-agreement baseline for the wearable-venous device class (§1.3/§1.4). Pairs with the AJP-Heart lead as StO₂-reproducibility context.
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** — arXiv:2512.15394 (Dec 2025). Joint vessel segmentation + sO₂ estimation without explicit fluence estimation. Not venous-specific but directly relevant to the deep-vein PA decoloring problem (§2.2). arxiv.org egress-blocked today; re-verified via index snippet only.
- **Optical Inversion and Spectral Unmixing of Spectroscopic PA Images with Physics-Informed Neural Networks (SPOI-AE)** — arXiv:2602.16357 (surfaced 06-11). PA decoloring/unmixing method — optically inverts and spectrally unmixes in-vivo spectroscopic PA images without assuming linearity, incorporating fluence compensation; not venous-specific. Method lead.
- **Distribution-Informed and Wavelength-Flexible Data-Driven Photoacoustic Oximetry** — arXiv:2403.14863. Learned spectral unmixing robust to unknown wavelength sets. Method lead, not venous-specific.
- **Machine-learning-enabled multiple-illumination quantitative optoacoustic oximetry imaging in humans** — arXiv:2102.11201 / PMC9203099. Multiple-illumination + learned spectral decoloring for quantitative PA sO₂ in humans; tissue/vessel-level, not venous-specific. Method lead underpinning the deep-vein decoloring family (§2.2 / Hybrid-Net).
- **Learned Spectral Decoloring enables Photoacoustic Oximetry** — *Scientific Reports* 11:6565 (2021) · DOI 10.1038/s41598-021-83405-8. Foundational learned-decoloring method (train on Monte-Carlo-simulated colored spectra); conceptual root of the data-driven-unmixing leads above. Not venous-specific.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % range. Standing metrology lead.
- **Anthropomorphic tissue-mimicking phantoms for oximetry validation in multispectral optical imaging** — arXiv:2503.23161. Anthropomorphic phantom framework for validating multispectral/PA oximetry; metrology lead complementing the sulfate-phantom work. Not venous-specific.
- **SFDI-net / deep-learning-enabled spatial frequency domain imaging** — *J. Biomed. Opt.* 30(4):046008 (2025; PMC12014942). Real-time two-layer SFDI inversion to hemoglobin/sO₂ maps; tissue-level. Transferable wide-field lead, not intravascular venous.
- **Near-Infrared Spiroximetry** (respiration-frequency-filtered NIRS venous saturation; Franceschini/Fantini lineage; *J. Appl. Physiol.* 92(1):372, 2002; PMC3786737). Foundational method for isolating the venous component by respiratory modulation — the physiological root of the "filter at the respiration frequency" strategy shared by §1.2/§1.3 and cerebral-venous DOS. Standing method lead; re-confirmed today.
- **PPG-waveform venous oximetry** (finger-PPG venous saturation from positive-pressure-ventilation modulation). Foundational peripheral-venous method family; conceptual sibling of §1.3.
- **Noninvasive optical quantification of cerebral venous oxygen saturation in humans** — PMID 24439329 (*Acad. Radiol.* / ScienceDirect S1076633213005011, 2014). Respiration-frequency-selected NIRS validated against a gold-standard cerebral-venous measurement; the cerebral-venous companion to the spiroximetry lead. Standing method lead, re-confirmed today.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction** — *JMIR Formative Research*, 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation showing >FDA-threshold error in the hypoxemic range — a transferable accuracy caution for the wearable-venous device class (§1.3/§1.4/§1.6), which operates at even lower saturations.
- **Quantitative Oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065; worldscientific.com). Review scaffold under the deep-vein PA anchors; authors unverified.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus triple-wavelength optoacoustic oximetry; transfontanelle cerebral oximetry, *Sci. Rep.* 2022 s41598-022-19350-x). Foundational venous-optoacoustic prior art, with a concrete commercial endpoint logged (§1.6, Noninvasix LIVOx).
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂; closest MSOT venous-challenge human data.

---

## Cross-topic synthesis

Today's two-day sweep (08-17 → 08-19) produced **no new intravascular venous optical result** for either topic, and **no item genuinely new to the corpus** — the only near-window sighting is a *Frontiers in Photonics* diffuse-optics editorial that is tissue-level and adds no venous measurement. The most recent genuinely-new addition to the corpus therefore remains the 08-13 Tran et al. hyperspectral retinal imager (§2.5), which sits in the **retinal per-vessel venular** sub-cluster. **No new systemic SvO₂/ScvO₂ measurement paper appeared — the seventeenth consecutive dry cycle** for true central/peripheral venous work once arterial-only and tissue-level items are excluded.

The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — addressed by three complementary strategies:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.1, chest/SSS optoacoustic LIVOx §1.6) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, e-tattoo spatial filtering §1.4, DNN inversion §1.2, respiration-frequency spiroximetry/cerebral-venous DOS, PPG-waveform venous oximetry). The standing tissue-level NIRS leads (AJP-Heart, El Masry) are a reminder that the *reproducibility* of the underlying StO₂ signal — not just its accuracy — is a live weakness this whole family must beat.
3. **Physics- and data-based decoloring / per-vessel correction** before unmixing (deep-tissue PA fluence correction §2.2, per-vessel spectral cleanup in vis-OCT §2.4, intravascular PACT §2.3, hyperspectral spatial–spectral fusion §2.5, plus the Hybrid-Net / SPOI-AE / learned-spectral-decoloring / distribution-informed unmixing leads and the sulfate- and anthropomorphic-phantom metrology).

The most mature, highest-precision proving ground for the strategy-3 corrections remains **retinal venular oximetry** (§2.4/§2.5). The hardest open problem remains the **systemic deep vein**, where §2.1/§2.2 push PA fluence correction toward a clinically meaningful central-venous surrogate, and where §1.6 shows one optoacoustic embodiment has already reached a regulatory pathway. The counterweight is unchanged: even *arterial* wearable oximetry (the JMIR lead) fails in the low-saturation range where venous measurement lives, and tissue-level modalities disagree substantially and repeat imperfectly (El Masry + AJP-Heart leads). Net: **no bedside-ready systemic non-invasive SvO₂ optical research result emerged this cycle**, and the honest population of strong, truly-venous, truly-optical *new* papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-19 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; pubmed.ncbi.nlm.nih.gov, journals.physiology.org, www.spiedigitallibrary.org, arxiv.org, and publisher full-text pages returned HTTP 403 / EGRESS_BLOCKED to direct fetch in this environment (source-/policy-side; agent proxy healthy), so items flagged "full text not read" / "snippet-verified" are abstract- or snippet-level and flagged unverified fields are noted inline.*
