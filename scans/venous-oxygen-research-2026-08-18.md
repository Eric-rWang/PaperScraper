# Venous Oxygen Research Scan — 2026-08-18

**Search window:** Thirty-eighth scan in the series, run **one day** after 2026-08-17. Emphasis on work published or first-surfacing after 08-17, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (physics.med-ph / eess.IV new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer, Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter/Brill, MDPI (*Sensors/Biosensors/Bioengineering*), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, *JACC: Advances* and American Physiological Society journals, ClinicalTrials.gov, plus Semantic Scholar / Google-Scholar-style index snippets and ResearchGate.

**Verification caveat:** Publisher **full-text** pages and several databases were again unreachable for direct `WebFetch` today. **pubmed.ncbi.nlm.nih.gov, www.ncbi.nlm.nih.gov (PMC), www.degruyterbrill.com, and www.researchgate.net all returned `EGRESS_BLOCKED`** on direct fetch, and the usual publisher hosts (link.springer.com, opg.optica.org, sciencedirect.com, wiley.com, spiedigitallibrary.org, jacc.org, journals.physiology.org) return **HTTP 403 / EGRESS_BLOCKED** to direct fetch; arxiv.org remains egress-blocked in this environment. The blocks are source-/policy-side, not relay failures. Every reference below was therefore cross-checked across **≥2 independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**One genuinely new venous-specific paper first-surfaced in the 08-17 → 08-18 window — but it is NON-OPTICAL.** McDiarmid et al., *JACC: Advances* (2026 Jan), develop and validate a **cardiac-MRI (T2-mapping) model of true mixed venous oxygen saturation (SvO₂)** in heart failure, validated in a 628-patient cohort. It is a legitimate, large-cohort, non-invasive **true mixed-venous SvO₂** result — directly on-topic for **Topic 1** ("non-invasive monitoring of venous blood oxygen") — but it uses **CMR, not any optical modality**, so it does **not** advance Topic 2. It is added below as Topic-1 §1.1 (new) with an honest split score: high for the non-invasive-venous goal, low for the optical-imaging thesis.

**No new venous-specific *optical* measurement paper first-surfaced today.** Repeated targeted sweeps (SvO₂/ScvO₂ optical, jugular PA/NIRS, deep-vein PA, vis-OCT venular oximetry, hyperspectral, DOS/DOI, SFDI) returned only the **standing corpus**. The most recent genuinely-new *optical* intravascular-venular result remains the 08-13 hyperspectral retinal system (Tran et al., *J. Biomed. Opt.* 31(3):036006, Topic-2 §2.5), carried forward unchanged.

**Metadata correction logged today (see §1.2):** the flagship jugular optical-sensing paper (previously catalogued with authors "Alqahtani et al.", vol 10(2)) is in fact **Hill, Campbell, Chase & Pretty**, *Curr. Dir. Biomed. Eng.* **10(4):295–298** (2024). Title, DOI (10.1515/cdbme-2024-2072) and the reported SvO₂ values (71.1/72.2/70.4 %) are unchanged and re-confirmed. The corpus author/volume fields were wrong; corrected here.

**No new venous-specific *optical* systemic (SvO₂/ScvO₂) measurement paper today — the seventeenth consecutive scan cycle with none.** All standing optical Topic-1 anchors and the deep-vein PA anchors are unchanged and carried forward with scores held.

**Per the standing brief: fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-*optical* *new* papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*One new primary item today (§1.1, non-optical CMR). Standing best-available optical set follows, scores carried forward. No primary non-invasive systemic venous-O₂ **optical** measurement paper has first-surfaced since before 2026-07-15.*

### 1.1 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure *(NEW today — non-optical CMR method)*
- **Authors:** Adam K. McDiarmid, Bradley S. Chambers, David A. Broadbent, Roshan Patel, Gareth Matthews, Oscar Gonzalez-Fernandez, Sven Plein, Pankaj Garg, Peter P. Swoboda
- **Year / Venue:** **2026 Jan** · *JACC: Advances* **5**(1):102484
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · https://www.jacc.org/doi/10.1016/j.jacadv.2025.102484 · PMID 41609283 · PMC12869880 · ScienceDirect S2772963X25009135
- **Relevance:** **7.0/10 for the non-invasive-venous goal; ~2/10 for the optical-imaging thesis** — a genuinely non-invasive estimate of **true mixed venous SvO₂** validated at scale, but by cardiac MRI, not optics.
- **Novelty:** Derives an imaging-derived SvO₂ (**iSvO₂**) from **CMR T2 mapping** (blood T2 depends on deoxyhaemoglobin fraction, the magnetic analogue of the optical hemoglobin-absorption contrast the rest of this corpus exploits). Model built by linear regression in a **discovery cohort of N=30** with paired CMR T2 mapping and invasive right-heart catheterisation, then applied to a **validation cohort of 628** recently-diagnosed heart-failure patients; iSvO₂ was prognostic for all-cause mortality / HF hospitalisation over a median 3-year follow-up.
- **Integration insight:** The first genuinely-new *true mixed-venous* SvO₂ result the series has logged in weeks, and it reframes the corpus's central question. Every optical Topic-1 anchor (§1.2–§1.6) chases a **local/regional** venous target (jugular, radial, peripheral); this paper reaches **systemic mixed venous** SvO₂ — the actual RHC gold-standard quantity — but only inside an MRI scanner, i.e. not continuous, not bedside, not wearable. It sets the clinical bar (systemic SvO₂, large-cohort prognostic validation) that the optical/PA program (§1.6 LIVOx, §2.1 IJV-PA, §2.2 APM+) is trying to reach in a portable form, and its T2-vs-deoxyHb contrast mechanism is a useful cross-modality mirror of the spectral-decoloring problem on the optical side.
- **Metadata note:** Title, full author list, venue, volume/issue/article-number, DOI, PMID and PMC id cross-confirmed across ≥2 independent index snippets (JACC landing + PubMed + PMC + ScienceDirect). **Full text not read** (jacc.org, pubmed, PMC all egress-blocked/403 today); cohort sizes (30 / 628) and method (CMR T2 mapping, linear regression) are snippet-level and should be treated as reported-not-verified.

### 1.2 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10; flagship optical-venous device paper; **author/volume metadata corrected today**)*
- **Authors:** **Jordan F. Hill, Jake Campbell, J. Geoffrey Chase, Christopher G. Pretty** *(University of Canterbury, NZ)* — **corrects the prior corpus attribution "Alqahtani et al."**
- **Year / Venue:** 2024 (Dec) · *Current Directions in Biomedical Engineering* **10(4):295–298** (De Gruyter/Brill; CDBME-2024-2072) — **corrects the prior corpus "10(2)"**
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072 · open-access PDF: https://www.degruyterbrill.com/document/doi/10.1515/cdbme-2024-2072/pdf?licenseType=open-access
- **Relevance:** 9.0/10 — direct non-invasive **optical** SvO₂ at the external jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the external-jugular venous waveform and estimates SvO₂ within the healthy 60–90 % band. Across three subjects: **SvO₂ from the EJV pulse = 71.1 / 72.2 / 70.4 %**, and from the breathing (respiration) pulse = 74.7 / 75.3 / 74.1 % — both bands physiologically plausible, and the two-pulse cross-check (cardiac EJV pulse vs respiration pulse) is itself a useful internal consistency test.
- **Integration insight:** Anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck. The respiration-pulse readout ties it directly to the spiroximetry / cerebral-venous-DOS method leads. It is the portable-optical counterpoint to the new §1.1 CMR result — same quantity family (venous sO₂), opposite ends of the cost/portability/validation spectrum (3 subjects, no gold-standard calibration yet, vs 628-patient CMR validation).
- **Metadata note:** Title, DOI, and SvO₂ values re-confirmed today via De Gruyter/Brill open-access listing + d-nb.info catalogue snippet + ResearchGate record; the **author list and volume/issue are today's correction** (both cross-confirmed across the De Gruyter listing and two search-index snippets). Full text (open access) not directly fetchable today (degruyterbrill.com egress-blocked).

### 1.3 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see flag)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume / overlying-tissue confound.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.2's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work.
- **Metadata flag:** DOI string not re-verifiable on the Optica page today (403); Optica locator (ol-49-10-2669) + title/authors/year cross-confirmed via two index snippets. Treat raw DOI numeral as **unverified**; cite via the Optica abstract URL.

### 1.4 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Authors:** (peripheral-venous oximetry group; BioMedical Engineering OnLine)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x · PMC5437414
- **Relevance:** 8.0/10 — foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically.
- **Novelty:** External stimulation induces cyclical venous fluctuation, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** Conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering, PPG-waveform venous oximetry). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.
- **Metadata note:** Re-confirmed today via BioMedical Engineering OnLine full-text listing + PMC snippet.

### 1.5 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01)*
- **Authors:** Tan P., Lu N., et al. (UT Austin)
- **Year / Venue:** 2023/2024 · IEEE (EMBC-lineage); related patent US 20250025074
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent: https://patents.justia.com/patent/20250025074 · author PDF: https://sites.utexas.edu/nanshulu/files/2024/10/Towards_Simultaneous_Noninvasive_Arterial_and_Venous_Oxygenation_Monitoring_with_Wearable_E-Tattoo.pdf
- **Relevance:** 8.0/10 — explicitly names non-invasive **venous** oxygenation as the unmet need and targets it with a wrist-worn optical patch.
- **Novelty:** Ultra-thin self-adherent optical e-tattoo measures arterial + venous pulses from multiple wrist sites; proposes spatial filtering to separate arterial/venous crosstalk. Phantom studies show well-separated per-vessel sensor responses.
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.4 attacks by modulation and §1.2 sidesteps by anatomy. The standing JMIR hypoxia-accuracy caution bears directly on this device class.

### 1.6 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Authors:** (VO100 clinical validation group)
- **Year / Venue:** 2023/2024 · *J. Cardiothorac. Vasc. Anesth.* (S1053-0770 lineage) / ScienceDirect · PMID 37827917
- **Link / DOI:** https://doi.org/10.1053/j.jvca.2023.10.006 · https://www.sciencedirect.com/science/article/pii/S1053077023007826
- **Relevance:** 8.0/10 — a marketed non-invasive device that estimates central venous saturation from external-jugular NIRS (SjvO₂ surrogate for ScvO₂); prospective ICU cohort (79 patients: 36 COVID-19, 43 post-liver-transplant) reported strong linear correlation with invasive ScvO₂.
- **Novelty:** Transcutaneous NIRS sensor placed over the external-jugular projection recovers a continuous central-venous-saturation surrogate at the bedside, the commercial counterpart to §1.2/§1.3.
- **Integration insight:** The optical device most directly bridging Topic-1's clinical need and Topic-2's optical physics on the systemic-venous front; validation-cohort agreement is the key open question for the whole jugular-NIRS class. Complements the new §1.1 CMR result: same clinical target (a central/systemic venous surrogate), but continuous and bedside rather than scanner-bound.
- **Metadata note:** ScienceDirect record (S1053077023007826) and PMID 37827917 re-confirmed today; the pediatric jugular-NIRS validation grounding the agreement claim (r = 0.91; bias 2.92 %, LoA −5.2 % to +11 %; PMC7491293) is unchanged.

### 1.7 — Noninvasix LIVOx Optoacoustic Central Venous Oxygenation Monitor (ScvO₂ for septic shock) *(previously surfaced — scan 08-11; device/regulatory anchor, not new research)*
- **Authors:** Noninvasix, Inc. / Esenaliev–Petrov optoacoustic lineage (UTMB)
- **Year / Venue:** FDA Breakthrough-Device designation 2022; ongoing development (not a dated research paper)
- **Link / DOI:** company / regulatory record; underlying method rooted in the superior-sagittal-sinus / transfontanelle optoacoustic oximetry lineage (*Sci. Rep.* 2022, s41598-022-19350-x)
- **Relevance:** 7.5/10 — an optoacoustic embodiment explicitly targeting **central venous** (ScvO₂) saturation non-invasively; the clearest regulatory-pathway endpoint in the corpus for the venous-optoacoustic thesis.
- **Novelty:** Laser-optoacoustic probe reads oxygenation from a named central vein directly, rather than through a tissue-StO₂ surrogate — the device-development counterpart to the IJV-PA research anchor §2.1.
- **Integration insight:** Demonstrates that non-invasive venous optoacoustic oximetry has crossed from lab demonstration into a regulated device pathway; the commercial bookend to Topic-2's PA measurement physics.
- **Metadata flag:** Regulatory/company record, not a peer-reviewed dated paper; treat designation year as reported. No new filing seen today.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new item today.* Measurement anchors carried forward with scores held; the 08-13 hyperspectral retinal system (§2.5) remains the most recent genuinely-new entry. (The new §1.1 CMR paper is deliberately **not** listed here — it is non-optical.)

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Authors:** (IJV-PA human oximetry group; Garcia-Uribe / Wang lineage)
- **Year / Venue:** 2023 · arXiv:2303.10775 / PA human-imaging lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: photoacoustic sO₂ of a named deep **vein** (internal jugular) in humans, non-invasively (sijvO₂ ≈ 72 ± 7 %).
- **Novelty:** Demonstrates human IJV oxygenation from multi-wavelength PA, pushing PA oximetry from superficial microvessels to a clinically meaningful deep venous target.
- **Integration insight:** Proof that optical/PA venous oximetry can reach a central-venous surrogate; the bridge between Topic 1's clinical need and Topic 2's imaging physics. It is the portable-optical analogue of the new §1.1 CMR systemic-SvO₂ result.
- **Metadata flag:** arxiv.org egress-blocked today; re-verified via ≥2 index snippets (arXiv abstract listing + PDF snippet).

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366 · https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring; radial artery–vein pair imaged in eight healthy adult volunteers.
- **Novelty:** The arterial prior method (APM+) leverages high arterial sO₂ to locally calibrate optical fluence and correct wavelength-dependent spectral coloring, recovering deep-tissue venous sO₂ where conventional linear unmixing fails. Phantom median estimation error 2.9 % vs 9.8 % for conventional linear unmixing.
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
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3 % in veins; ≈1 % bias vs blood-gas across 0–100 % (ex-vivo phantom validation); RMSE ≈ 2.1 % vs pulse oximeter in major arteries.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans (arteries ≈95 %, veins ≈72 % in reported cohorts).
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the retinal-oximetry review holds up as state-of-the-art for retinal venular oximetry.
- **Metadata note:** Title/venue/DOI re-confirmed today via Nature *Communications Medicine* landing + PMC10126115 + DOAJ snippet.

### 2.5 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — first surfaced 08-13; per-vessel retinal artery + vein sO₂; most recent genuinely-new optical entry)*
- **Authors:** Tran M.H., Pruitt K., Bryarly M., Emordi I., Ali A., Ma L., Fei B. (Quantitative Bioimaging Laboratory, UT Dallas / UT Southwestern)
- **Year / Venue:** **2026** · *Journal of Biomedical Optics* **31**(3):036006 (2026 Mar 1)
- **Link / DOI:** https://doi.org/10.1117/1.JBO.31.3.036006 · PMC12997856 · SPIE: https://www.spiedigitallibrary.org/journals/journal-of-biomedical-optics/volume-31/issue-3/036006/
- **Relevance:** 7.5/10 — a 2026 hyperspectral fundus system that measures **per-vessel retinal venule sO₂ (≈58 %)** alongside arteriole sO₂ (≈98 %) and vessel diameter; a true intravascular venular optical readout, though retinal per-vessel, **not systemic SvO₂**.
- **Novelty:** High-resolution snapshot/hyperspectral retinal imager that recovers vessel diameter *and* oxygenation simultaneously; a **deep-learning pansharpening** step fuses high-spatial and high-spectral channels (reported pansharpening RMSE 2.15 ± 0.64, correlation coefficient 0.96 ± 0.05, spectral-angle 0.06 ± 0.03 rad, ERGAS 2.37 ± 1.71). Reported venule sO₂ ≈ 58 % matches the accepted retinal venous norm (≈57.9 ± 9.9 %), giving physiological face-validity to the calibration.
- **Integration insight:** A 2026 entry in the retinal-oximetry cluster (with ADS-vis-OCT §2.4 and the standing HSI/retinal-review leads). It advances the *spatial–spectral fusion* angle — using deep learning to reconcile the resolution/spectral-sampling trade-off that limits fundus HSI — the same class of confound (per-vessel diameter, vessel boundary, media transparency) the vis-OCT and deep-vein PA work must correct. Reinforces that retinal venular oximetry remains the most mature, best-validated proving ground for per-vessel venous optical measurement, and offers a cheaper camera-based route (vs vis-OCT / PA hardware) toward the same per-vessel venous readout.
- **Metadata flag:** Title, authors, venue, volume/issue/article-number and DOI cross-confirmed today across ≥2 independent index snippets (SPIE Digital Library listing + PMC12997856 + UT Southwestern Pure). **Full text not read** — spiedigitallibrary.org, pmc.ncbi.nlm.nih.gov and the UTSW Pure page were egress-blocked to direct fetch; numeric performance figures are snippet-level and should be treated as reported-not-verified.

**Topic-2 note:** the anchors most on-target for *systemic deep-vein* venous oximetry (§2.1 IJV-PA, §2.2 APM+ radial vein) are unchanged; no new item this cycle strengthens either the systemic deep-vein or the retinal per-vessel sub-cluster.

---

## Standing context leads (not ranked in the top-5)

- **Low-Rate Wrist SpO₂ Estimation under Micro-Perturbations Using Motion-Aware Beat Selection and Perfusion-Guided Calibration** — arXiv:2607.08001 (2026). **Arterial-only** wrist PPG SpO₂ method; surfaced today. Not venous, but its motion-aware beat-selection and perfusion-guided calibration attack the same low-perfusion/low-SNR signal-extraction problem the wearable venous devices (§1.4/§1.5) face at even lower saturations. Method/robustness lead only. arxiv.org egress-blocked; snippet-verified.
- **Near-infrared spectroscopy demonstrates preserved and reproducible resting skeletal muscle oxygenation across anatomical sites in stable heart failure** — *Am. J. Physiol. Heart Circ. Physiol.* (2026) · DOI 10.1152/ajpheart.00398.2026. **Tissue-level (StO₂), NOT venous.** CW-NIRS reproducibility study; the StO₂ signal is a mixed arterial+venous microvascular quantity. Value is as a 2026 StO₂-reproducibility baseline for the wearable/tissue-oximetry device class (§1.4/§1.5). *journals.physiology.org egress-blocked; snippet-verified only.*
- **Retinal Oximetry: New Insights into Ocular and Systemic Diseases** — Zhang W., Tu X., Wang X., et al. · *Graefe's Archive* 263:2101–2115 (2025) · DOI 10.1007/s00417-025-06831-8 · PMID 40254630 · PMC12414079. Review consolidating retinal oximetry across spectrophotometric-fundus, hyperspectral, and vis-OCT modalities; frames retinal artery *and vein* saturation as ocular + systemic biomarkers. Review-level companion to §2.5 and §2.4.
- **Integrated spectral and depth compensation for sO₂ and total-hemoglobin estimation in PAT for ovarian-lesion diagnosis** — *Biomed. Opt. Express*-lineage, 2026 · PMC12869027. Combines spectral + depth fluence compensation for deep-tissue PAT sO₂; **not venous-specific** (arterial+venous tissue, ovarian). Method lead for the deep-vein decoloring problem (§2.2). Snippet-verified only.
- **Comparative assessment of healthy tissue oxygenation using near-infrared imaging, transcutaneous oxygen measurement, and plethysmography** — El Masry et al. · *Scientific Reports* 15:30424 (2025) · PMID 40830190 · PMC12365204 · DOI 10.1038/s41598-025-15767-2. **Tissue-level (StO₂), NOT venous.** SFDI uniquely detected significant StO₂ differences; device-to-device correlations only moderate-to-fair — a cross-modality-agreement baseline for the wearable-venous device class (§1.4/§1.5).
- **OxyGAN / adversarial snapshot SFDI oxygenation mapping** — (PMC7701163; arXiv:2007.00760). Rapid tissue-oxygenation mapping from single structured-light snapshots via adversarial deep learning; ~10× faster inversion enabling ~25-Hz video-rate StO₂ mapping. Tissue-level, not intravascular venous; wide-field real-time SFDI lead.
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** — arXiv:2512.15394 (Dec 2025). Joint vessel segmentation + sO₂ estimation without explicit fluence estimation. Not venous-specific but directly relevant to the deep-vein PA decoloring problem (§2.2). arxiv.org egress-blocked; snippet-verified.
- **Optical Inversion and Spectral Unmixing of Spectroscopic PA Images with Physics-Informed Neural Networks (SPOI-AE)** — arXiv:2602.16357 (surfaced 06-11). PA decoloring/unmixing method; not venous-specific. Method lead.
- **Distribution-Informed and Wavelength-Flexible Data-Driven Photoacoustic Oximetry** — arXiv:2403.14863 · PMC11151660. LSTM/RNN learned spectral unmixing robust to arbitrary/unknown wavelength sets; outperforms linear unmixing. Method lead, not venous-specific.
- **Machine-learning-enabled multiple-illumination quantitative optoacoustic oximetry imaging in humans** — PMC9203099. Multiple-illumination + learned spectral decoloring for quantitative PA sO₂ in humans; tissue/vessel-level, not venous-specific. Method lead underpinning the deep-vein decoloring family (§2.2 / Hybrid-Net).
- **Learned Spectral Decoloring enables Photoacoustic Oximetry** — *Scientific Reports* 11:6565 (2021) · DOI 10.1038/s41598-021-83405-8. Foundational learned-decoloring method (train on Monte-Carlo-simulated colored spectra); conceptual root of the data-driven-unmixing leads above. Not venous-specific.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % range. Standing metrology lead.
- **Anthropomorphic tissue-mimicking phantoms for oximetry validation in multispectral optical imaging** — arXiv:2503.23161. Anthropomorphic phantom framework for validating multispectral/PA oximetry; metrology lead complementing the sulfate-phantom work. Not venous-specific.
- **SFDI-net / deep-learning-enabled spatial frequency domain imaging** — *J. Biomed. Opt.* 30(4):046008 (2025; PMC12014942). Real-time two-layer SFDI inversion to hemoglobin/sO₂ maps; tissue-level. Transferable wide-field lead, not intravascular venous.
- **Near-Infrared Spiroximetry** (respiration-frequency-filtered NIRS venous saturation; Franceschini/Fantini lineage; *J. Appl. Physiol.* 92(1):372, 2002; PMC3786737). Foundational method for isolating the venous component by respiratory modulation — the physiological root of the "filter at the respiration frequency" strategy shared by §1.2/§1.3/§1.4 and cerebral-venous DOS, and the exact mechanism behind §1.2's "breathing-pulse" SvO₂ readout. Standing method lead; re-confirmed today.
- **PPG-waveform venous oximetry** (finger-PPG venous saturation from positive-pressure-ventilation modulation). Foundational peripheral-venous method family; conceptual sibling of §1.4.
- **Noninvasive optical quantification of cerebral venous oxygen saturation in humans** — PMID 24439329 (*Acad. Radiol.* / ScienceDirect S1076633213005011, 2014). Respiration-frequency-selected NIRS validated against a gold-standard cerebral-venous measurement; the cerebral-venous companion to the spiroximetry lead. Standing method lead, re-confirmed today.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction** — *JMIR Formative Research*, 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation showing >FDA-threshold error in the hypoxemic range — a transferable accuracy caution for the wearable-venous device class (§1.4/§1.5/§1.7), which operates at even lower saturations.
- **Quantitative Oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065). Review scaffold under the deep-vein PA anchors; authors unverified.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus triple-wavelength optoacoustic oximetry; transfontanelle cerebral oximetry, *Sci. Rep.* 2022 s41598-022-19350-x). Foundational venous-optoacoustic prior art, with a concrete commercial endpoint logged (§1.7, Noninvasix LIVOx).
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂; closest MSOT venous-challenge human data.
- **Novel Noninvasive Estimation of Mixed Venous Oxygen Saturation by Echocardiography and Expired Gas Analysis** — *Am. J. Physiol. Heart Circ. Physiol.* (2020; DOI 10.1152/ajpheart.00429.2020). **Non-optical** (echo + expired-gas) mixed-venous SvO₂ estimate; the methodological predecessor to the new CMR model §1.1 and a reminder that non-optical non-invasive SvO₂ estimation predates it.

---

## Cross-topic synthesis

Today's one-day sweep (08-17 → 08-18) produced **one genuinely-new venous-specific paper — McDiarmid et al.'s CMR-derived mixed-venous SvO₂ model (§1.1, *JACC: Advances* 2026)** — and **no new intravascular venous *optical* result** for either topic. That single new entry is significant precisely because it reaches the quantity the optical program keeps circling: **true systemic mixed-venous SvO₂**, the right-heart-catheter gold-standard, validated in **628** heart-failure patients. But it does so inside an **MRI scanner** via **T2 mapping**, so it is neither continuous, bedside, nor wearable — and it advances Topic 1 without touching Topic 2. It sets the clinical/validation bar (systemic SvO₂, large-cohort prognosis) that the portable-optical work — jugular NIRS (§1.6), IJV-PA (§2.1), APM+ radial-vein PA (§2.2), the LIVOx optoacoustic device (§1.7) — is trying to reach in a form a patient can wear. Notably, CMR's contrast mechanism (blood T2 ∝ deoxyhaemoglobin fraction) is the magnetic mirror of the optical hemoglobin-absorption contrast, and it faces its own version of the "separate the confound from the signal" problem the optical side calls spectral coloring.

A second, smaller housekeeping outcome today: a **metadata correction** to the corpus's flagship optical-venous paper (§1.2) — correct authors **Hill, Campbell, Chase & Pretty**, vol **10(4):295–298** (not "Alqahtani et al.", 10(2)). Title, DOI and reported SvO₂ values are unchanged and re-confirmed.

On the optical front the picture is unchanged. The two optical topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — addressed by three complementary strategies:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.2, jugular NIRS §1.6, IJV-PA §2.1, chest/SSS optoacoustic LIVOx §1.7) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.4, e-tattoo spatial filtering §1.5, DNN inversion §1.3, respiration-frequency spiroximetry/cerebral-venous DOS, PPG-waveform venous oximetry — and note §1.2 uses exactly this via its "breathing-pulse" readout). The standing tissue-level NIRS leads (AJP-Heart, El Masry) are a reminder that the *reproducibility* of the underlying StO₂ signal — not just its accuracy — is a live weakness this whole family must beat; today's arterial wrist-SpO₂ arXiv lead reinforces the low-perfusion signal-extraction difficulty.
3. **Physics- and data-based decoloring / per-vessel correction** before unmixing (deep-tissue PA fluence correction §2.2, per-vessel spectral cleanup in vis-OCT §2.4, intravascular PACT §2.3, hyperspectral spatial–spectral fusion §2.5, plus the Hybrid-Net / SPOI-AE / learned-spectral-decoloring / distribution-informed unmixing leads and the sulfate- and anthropomorphic-phantom metrology).

The most mature, highest-precision proving ground for the strategy-3 corrections remains **retinal venular oximetry** (§2.4/§2.5). The hardest open problem remains the **systemic deep vein**, where §2.1/§2.2 push PA fluence correction toward a clinically meaningful central-venous surrogate and §1.7 shows one optoacoustic embodiment has already reached a regulatory pathway — and where, as of today, the *only* validated large-cohort systemic-SvO₂ result (§1.1) is still tethered to an MRI scanner. The counterweight is unchanged: even *arterial* wearable oximetry (the JMIR and wrist-SpO₂ leads) struggles in the low-saturation range where venous measurement lives, and tissue-level modalities disagree substantially and repeat imperfectly (El Masry + AJP-Heart leads). Net: **no bedside-ready systemic non-invasive SvO₂ *optical* research result emerged this cycle** — the seventeenth consecutive dry cycle for optical systemic venous work — and the honest population of strong, truly-venous, truly-*optical* *new* papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-18 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; pubmed.ncbi.nlm.nih.gov, www.ncbi.nlm.nih.gov (PMC), www.degruyterbrill.com, www.researchgate.net, journals.physiology.org, jacc.org, www.spiedigitallibrary.org, and arxiv.org were egress-blocked, and publisher full-text pages returned HTTP 403 to direct fetch in this environment (source-/policy-side; agent proxy healthy), so items flagged "full text not read" / "snippet-verified" are abstract- or snippet-level and flagged unverified fields are noted inline.*
