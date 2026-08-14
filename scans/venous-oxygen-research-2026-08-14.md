# Venous Oxygen Research Scan — 2026-08-14

**Search window:** Thirty-sixth scan in the series, run **one day** after 2026-08-13. Emphasis on work published or first-surfacing after 08-13, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (physics.med-ph / eess.IV new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer, Wiley (*Advanced Science*, *Advanced Materials Technologies*, *J. Biophotonics*), De Gruyter, MDPI (*Sensors/Biosensors*), IEEE Xplore, Nature / *Sci. Rep.* / *npj Acoustics*, ClinicalTrials.gov, plus Semantic Scholar / Google-Scholar-style index snippets and ResearchGate.

**Verification caveat:** Publisher **full-text** pages and several databases were again unreachable for direct `WebFetch` today: **www.nature.com returned `EGRESS_BLOCKED`** from the network egress proxy, and the usual publisher hosts (link.springer.com, opg.optica.org, sciencedirect.com, wiley.com, spiedigitallibrary.org, pmc.ncbi.nlm.nih.gov) return **HTTP 403 / egress-block** to direct fetch; arxiv.org remains egress-blocked in this environment. The agent proxy itself reported healthy — the blocks are source-/policy-side, not relay failures. Every reference below was therefore cross-checked across **≥2 independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No item genuinely new to the corpus today. The fifteenth consecutive scan cycle with no new systemic SvO₂/ScvO₂ measurement paper**, and no new primary venous-specific optical measurement paper of any kind (including retinal per-vessel).

- Today's one-day sweep surfaced **no new primary 2026 venous-oxygen measurement paper**. The item that was new yesterday — **Tran et al., hyperspectral retinal imaging system** (*J. Biomed. Opt.* 31(3):036006, 2026, §2.5) — is now **previously surfaced** and carried forward as the most recent primary per-vessel venular result.
- Two **new-to-the-corpus context leads** appeared, both **review-level and wearable-adjacent, not venous-specific measurements**: a 2026 *Advanced Materials Technologies* review of on-skin tattoo-embedded sensors, and a 2025/2026 IOPscience review of electronic tattoos for wearable healthcare. They reinforce the wearable-optical-venous device thesis (§1.4) but contribute no new venous saturation data; logged under standing context leads with honest flags.

**Per the standing brief: fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical *new* papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. In fact **zero** genuinely new venous-specific measurement papers surfaced today. The lists below present the best available with honest relevance scores; all measurement entries are previously surfaced.

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
- **Metadata flag:** De Gruyter abstract snippet-confirmed; DOI resolves. Full text not read today (publisher 403).

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

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01)*
- **Authors:** Tan P., Lu N., et al. (UT Austin)
- **Year / Venue:** 2023/2024 · IEEE (EMBC-lineage); related patent US 20250025074
- **Link / DOI:** https://pubmed.ncbi.nlm.nih.gov/38083768/ · patent: https://patents.justia.com/patent/20250025074
- **Relevance:** 8.0/10 — explicitly names non-invasive **venous** oxygenation as the unmet need and targets it with a wrist-worn optical patch.
- **Novelty:** Ultra-thin self-adherent optical e-tattoo measures arterial + venous pulses from multiple wrist sites; proposes spatial filtering to separate arterial/venous crosstalk.
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.3 attacks by modulation and §1.1 sidesteps by anatomy. The standing JMIR hypoxia-accuracy caution bears directly on this device class. The two new 2026 tattoo-sensor **reviews** surfaced today (see standing leads) cite this thread as the exemplar of the venous-oxygenation use case, confirming it remains the field's reference point for optical-wearable SvO₂.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Authors:** (VO100 clinical validation group)
- **Year / Venue:** 2023/2024 · *J. Cardiothorac. Vasc. Anesth.* (S1053-0770 lineage) / ScienceDirect · PMID 37827917
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826
- **Relevance:** 7.5/10 — the one commercially available non-invasive jugular-NIRS ScvO₂ estimator clinically evaluated in critically ill patients.
- **Novelty:** Continuous non-invasive ScvO₂ estimate from an external jugular NIRS sensor, positioned as an alternative when catheter-based sampling is difficult.
- **Integration insight:** The clinical-translation benchmark for Topic 1 — the accuracy/bias any research-grade optical venous device (§1.1–1.4) must beat to matter at the bedside.

### 1.6 — Noninvasix LIVOx Optoacoustic Central Venous Oxygenation Monitor (ScvO₂ for septic shock) *(previously surfaced — scan 08-11; device/regulatory anchor, not new research)*
- **Authors / Sponsor:** Noninvasix Inc. (optoacoustic platform; Esenaliev / Petrov technology lineage, UTMB Galveston)
- **Year / Venue:** **2022** FDA **Breakthrough Device Designation** (device/regulatory milestone, not a peer-reviewed measurement paper)
- **Link:** https://noninvasix.com/ · trade coverage via BioWorld / NS Medical Devices / 24x7 (snippet-verified)
- **Relevance:** 8.0/10 to Topic 1 as a **device/translation anchor** — a chest-worn *optoacoustic* probe for non-invasive, real-time ScvO₂ in adults at risk of septic shock; arguably the most clinically advanced non-invasive *venous*-oxygen device on a regulatory pathway.
- **Novelty:** Optoacoustic (laser-induced ultrasound) readout of central venous oxygenation without a catheter; same platform demonstrated superior-sagittal-sinus venous sO₂ through the open fontanelle in preterm infants.
- **Integration insight:** The commercial/regulatory endpoint of the Esenaliev/Petrov large-vein optoacoustic lineage — the bedside destination the research-grade PA venous work (§2.2) is climbing toward; methodologically continuous with Topic-2 photoacoustics, making it the natural bridge between the two topics.
- **Honest flags:** **Not new research** — the designation dates to 2022 and is snippet-verified only; primary source pages were egress-blocked/403 today.

**Topic 1 honest note:** every measurement entry above is previously surfaced; nos. 1.3 and 1.5 predate 2023, and §1.6 is a 2022 regulatory milestone. The absence of *new* primary systemic venous measurement work today is itself the finding, not a gap in searching.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new items today.* Measurement anchors carried forward with scores held; the §2.5 hyperspectral retinal system, new yesterday, is now previously surfaced.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Authors:** (IJV-PA human oximetry group; Garcia-Uribe / Wang lineage)
- **Year / Venue:** 2023 · arXiv:2303.10775 / PA human-imaging lineage
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: photoacoustic sO₂ of a named deep **vein** (internal jugular) in humans, non-invasively (sijvO₂ ≈ 72 ± 7 %).
- **Novelty:** Demonstrates human IJV oxygenation from multi-wavelength PA, pushing PA oximetry from superficial microvessels to a clinically meaningful deep venous target.
- **Integration insight:** Proof that optical/PA venous oximetry can reach a central-venous surrogate; the bridge between Topic 1's clinical need and Topic 2's imaging physics.
- **Metadata flag:** arxiv.org egress-blocked today; re-verified via ≥2 index snippets.

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366 · https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring; radial artery–vein pair imaged in eight healthy adult volunteers.
- **Novelty:** The arterial prior method (APM+) leverages high arterial sO₂ to locally calibrate optical fluence and correct wavelength-dependent spectral coloring, recovering deep-tissue venous sO₂ where conventional linear unmixing fails. Phantom median estimation error 2.9 % vs 9.8 % for conventional linear unmixing.
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus; its fluence-correction strategy is the deep-vein counterpart to the retinal per-vessel corrections §2.4/§2.5 catalogue and to the Hybrid-Net / PINN spectral-unmixing leads.
- **Metadata flag:** Wiley abstract snippet cross-confirmed; full text 403 today.

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
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3 % in veins; ≈1 % bias vs blood-gas across 0–100 % (ex-vivo phantom validation).
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans (arteries ≈95 %, veins ≈72 % in reported cohorts).
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the retinal-oximetry review holds up as state-of-the-art for retinal venular oximetry.

### 2.5 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — first surfaced 08-13; per-vessel retinal artery + vein sO₂; most recent primary venular result)*
- **Authors:** Tran M.H., Pruitt K., Bryarly M., Emordi I., Ali A., Ma L., Fei B. (Quantitative Bioimaging Laboratory, UT Dallas / UT Southwestern)
- **Year / Venue:** **2026** · *Journal of Biomedical Optics* **31**(3):036006 (2026 Mar 1)
- **Link / DOI:** https://doi.org/10.1117/1.JBO.31.3.036006 · PMC12997856 · SPIE: https://www.spiedigitallibrary.org/journals/journal-of-biomedical-optics/volume-31/issue-3/036006/
- **Relevance:** 7.5/10 — a primary 2026 hyperspectral fundus system that measures **per-vessel retinal venule sO₂ (≈58 %)** alongside arteriole sO₂ (≈98 %) and vessel diameter; a true intravascular venular optical readout, though retinal per-vessel, **not systemic SvO₂**.
- **Novelty:** High-resolution snapshot/hyperspectral retinal imager that recovers vessel diameter *and* oxygenation simultaneously; a **deep-learning pansharpening** step fuses high-spatial and high-spectral channels (reported pansharpening RMSE 2.15 ± 0.64, correlation coefficient 0.96 ± 0.05). Reported venule sO₂ ≈ 58 % matches the accepted retinal venous norm (≈57.9 ± 9.9 %), giving physiological face-validity to the calibration.
- **Integration insight:** The most recent primary entry in the retinal-oximetry cluster (with ADS-vis-OCT §2.4 and the standing HSI/retinal-review leads). It advances the *spatial–spectral fusion* angle — using deep learning to reconcile the resolution/spectral-sampling trade-off that limits fundus HSI — the same class of confound (per-vessel diameter, vessel boundary, media transparency) the vis-OCT and deep-vein PA work must correct. Reinforces that retinal venular oximetry remains the most mature, best-validated proving ground for per-vessel venous optical measurement, and offers a cheaper camera-based route (vs vis-OCT / PA hardware) toward the same per-vessel venous readout.
- **Metadata flag:** Title, authors, venue, volume/issue/article-number and DOI cross-confirmed across ≥2 independent index snippets (SPIE Digital Library listing + PMC + UT Southwestern Pure). **Full text not read** — spiedigitallibrary.org, pmc.ncbi.nlm.nih.gov and the UTSW Pure page were egress-blocked to direct fetch; numeric performance figures are snippet-level and should be treated as reported-not-verified.

**Topic-2 note:** the anchors most on-target for *systemic deep-vein* venous oximetry (§2.1 IJV-PA, §2.2 APM+ radial vein) are unchanged; no new item strengthened either the systemic deep-vein or the retinal per-vessel sub-cluster today.

---

## Standing context leads (not ranked in the top-5)

- **On-Skin Tattoo-Embedded Sensors (TES) for Next-Generation Sensing and Future Directions for Healthcare Monitoring** — Mazumdar et al. · *Advanced Materials Technologies* (Wiley), 2026 · DOI 10.1002/admt.202501304. **NEW to the corpus today.** Broad review of tattoo-embedded wearable sensors; frames continuous non-invasive **SvO₂** as an unmet need and cites the optical e-tattoo thread (§1.4) as an exemplar. **Review, not a venous measurement paper** — no new saturation data; logged as a wearable-context scaffold for §1.4. Snippet-verified only (Wiley 403).
- **Electronic Tattoos for Next-Generation Wearable Electronics and Healthcare Applications** — *IOP ECS Sensors Plus* / IOPscience, 2025/2026 · DOI 10.1149/2754-2726/ae23e2. **NEW to the corpus today.** Review of electronic-tattoo platforms for wearable healthcare; venous/optical oximetry is one use case among many. **Review, not venous-specific measurement.** Snippet-verified only.
- **Retinal Oximetry: New Insights into Ocular and Systemic Diseases** — Zhang W., Tu X., Wang X., et al. · *Graefe's Archive for Clinical and Experimental Ophthalmology* 263:2101–2115 (2025) · DOI 10.1007/s00417-025-06831-8 · PMID 40254630 · PMC12414079. Review consolidating retinal oximetry across spectrophotometric-fundus, hyperspectral, and vis-OCT modalities; frames retinal artery *and vein* saturation as ocular + systemic biomarkers. The review-level companion to the §2.5 HSI system and the §2.4 vis-OCT anchor.
- **Integrated spectral and depth compensation for sO₂ and total-hemoglobin estimation in PAT for ovarian-lesion diagnosis** — *J. Biomed. Opt.*-lineage, 2026 · PMC12869027. Combines spectral + depth fluence compensation for deep-tissue PAT sO₂; **not venous-specific** (arterial+venous tissue, ovarian). Method lead for the deep-vein decoloring problem (§2.2).
- **Heterogeneous tumor blood oxygenation dynamics during phototherapy deciphered with real-time label-free photoacoustic imaging** — *npj Acoustics* (2025) · DOI 10.1038/s44384-025-00012-x. Real-time label-free PA imaging of **tumor tissue-level StO₂** dynamics during phototherapy; **not venous, not intravascular sO₂.** Method/context lead for real-time PA oximetry only. nature.com egress-blocked today; snippet-verified.
- **Comparative assessment of healthy tissue oxygenation using near-infrared imaging, transcutaneous oxygen measurement, and plethysmography** — El Masry et al. · *Scientific Reports* 15:30424 (2025) · PMID 40830190 · PMC12365204 · DOI 10.1038/s41598-025-15767-2. **Tissue-level (StO₂), NOT venous.** SFDI uniquely detected significant StO₂ differences; device-to-device correlations only moderate-to-fair — a sobering cross-modality-agreement baseline for the wearable-venous device class (§1.3/§1.4).
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** — arXiv:2512.15394 (Dec 2025). Joint vessel segmentation + sO₂ estimation without explicit fluence estimation. Not venous-specific but directly relevant to the deep-vein PA decoloring problem (§2.2). arxiv.org egress-blocked today; re-verified via index snippet only.
- **Optical Inversion and Spectral Unmixing of Spectroscopic PA Images with Physics-Informed Neural Networks (SPOI-AE)** — arXiv:2602.16357 (surfaced 06-11). PA decoloring/unmixing method; not venous-specific. Method lead.
- **Distribution-Informed and Wavelength-Flexible Data-Driven Photoacoustic Oximetry** — arXiv:2403.14863. Learned spectral unmixing robust to unknown wavelength sets. Method lead, not venous-specific.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % range. Standing metrology lead.
- **Anthropomorphic tissue-mimicking phantoms for oximetry validation in multispectral optical imaging** — arXiv:2503.23161. Phantom-standardization lead for multispectral/PA oximetry validation; not venous-specific.
- **SFDI-net / deep-learning-enabled spatial frequency domain imaging** — *J. Biomed. Opt.* 30(4):046008 (2025; PMC12014942). Real-time two-layer SFDI inversion to hemoglobin/sO₂ maps; tissue-level. Transferable wide-field lead, not intravascular venous.
- **PPG-waveform venous oximetry** (finger-PPG venous saturation from positive-pressure-ventilation modulation). Foundational peripheral-venous method family; conceptual sibling of §1.3.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction** — *JMIR Formative Research*, 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation showing >FDA-threshold error in the hypoxemic range — a transferable accuracy caution for the wearable-venous device class (§1.3/§1.4/§1.6), which operates at even lower saturations.
- **Quantitative Oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065; worldscientific.com). Review scaffold under the deep-vein PA anchors; authors unverified.
- **Non-Invasive Monitoring of Mixed Venous Oxygen Saturation Using the Capnodynamic Method in Adults** — ClinicalTrials.gov NCT06632197. **Non-optical** (capnodynamic/CO₂-rebreathing) SvO₂ estimation; logged as a non-optical comparator/benchmark for the optical venous target, not an optical-imaging method.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus triple-wavelength optoacoustic oximetry; transfontanelle cerebral oximetry, *Sci. Rep.* 2022 s41598-022-19350-x). Foundational venous-optoacoustic prior art, with a concrete commercial endpoint logged (§1.6, Noninvasix LIVOx).
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂; closest MSOT venous-challenge human data.

---

## Cross-topic synthesis

Today produced **no item genuinely new to the corpus** on the measurement front. The most recent primary venous-specific optical result remains the Tran et al. hyperspectral retinal system (*J. Biomed. Opt.* 31(3):036006, 2026, §2.5), now one day old and previously surfaced — a **retinal per-vessel venular** measurement, not systemic SvO₂. The two genuinely new documents surfaced today are both **wearable-sensor reviews** (*Advanced Materials Technologies* TES review; IOPscience electronic-tattoo review) that name non-invasive SvO₂ as an unmet need and cite the optical e-tattoo thread (§1.4) — useful confirmation that the wearable-optical-venous framing is the field's reference point, but contributing no new saturation data. **No new systemic SvO₂/ScvO₂ measurement paper appeared today — the fifteenth consecutive dry cycle** for true central/peripheral venous work once arterial-only and tissue-level (StO₂) items are excluded.

The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — addressed by three complementary strategies:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.1, chest/SSS optoacoustic LIVOx §1.6) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, e-tattoo spatial filtering §1.4, DNN inversion §1.2, PPG-waveform venous oximetry) — the strategy the two new wearable reviews implicitly survey.
3. **Physics- and data-based decoloring / per-vessel correction** before unmixing (deep-tissue PA fluence correction §2.2, per-vessel spectral cleanup in vis-OCT §2.4, intravascular PACT §2.3, hyperspectral spatial–spectral fusion §2.5, plus the Hybrid-Net / SPOI-AE / distribution-informed unmixing leads and sulfate-phantom / anthropomorphic-phantom metrology).

The most mature, highest-precision proving ground for the strategy-3 corrections remains **retinal venular oximetry** (§2.4/§2.5). The hardest open problem remains the **systemic deep vein**, where §2.1/§2.2 push PA fluence correction toward a clinically meaningful central-venous surrogate, and where §1.6 shows one optoacoustic embodiment has already reached a regulatory pathway. The counterweight is unchanged: even *arterial* wearable oximetry (the JMIR lead) fails in the low-saturation range where venous measurement lives, and tissue-level modalities disagree substantially with one another (El Masry lead). Net: **no new venous-specific optical measurement result emerged today**, the field's wearable-venous framing was re-affirmed by two new reviews, and the honest population of strong, truly-venous, truly-optical *new* papers remains **fewer than five per topic** — indeed zero new ones today — once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-14 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; www.nature.com, pmc.ncbi.nlm.nih.gov, www.spiedigitallibrary.org, and arxiv.org were egress-blocked, and publisher full-text pages (Wiley, Springer, Optica, ScienceDirect) returned HTTP 403 to direct fetch in this environment (source-/policy-side; agent proxy healthy), so items flagged "full text not read" / "snippet-verified" are abstract- or snippet-level and flagged unverified fields are noted inline.*
