# Venous Oxygen Research Scan — 2026-08-12

**Search window:** Thirty-fourth scan in the series, run **one day** after 2026-08-11. Emphasis on work published or first-surfacing after 08-11, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (physics.med-ph / eess.IV new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer (Graefe's Archive), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Sensors/Biosensors/Biomedicines*), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, ClinicalTrials.gov, plus Semantic Scholar / Google-Scholar-style index snippets and ResearchGate.

**Verification caveat:** Publisher **full-text** pages and several databases were again unreachable for direct `WebFetch` today: **nature.com and pubmed.ncbi.nlm.nih.gov returned `EGRESS_BLOCKED`** from the network egress proxy, and the usual publisher hosts (link.springer.com, pmc.ncbi.nlm.nih.gov, opg.optica.org, sciencedirect.com, wiley.com) return **HTTP 403** to direct fetch; **arxiv.org is egress-blocked** in this environment. The agent proxy itself reported healthy — the blocks are source-/policy-side, not relay failures. Every reference below was therefore cross-checked across **≥2 independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the thirteenth consecutive scan cycle with none.** Today's one-day sweep produced **no new SvO₂/ScvO₂ demonstration**. The Topic-1 (true SvO₂) and Topic-2 (imaging-technique) top-5 measurement anchors are unchanged and carried forward with scores held.

Today's searches re-surfaced only corpus items, plus **one item new to the corpus that is *not* venous-specific**:

- **Comparative assessment of healthy tissue oxygenation using near-infrared imaging, transcutaneous oxygen measurement, and plethysmography** (El Masry, Li, Balasubramani, Roy, Sen, Gnyawali — *Scientific Reports* **15**:30424, 2025; PMID 40830190; PMC12365204; DOI 10.1038/s41598-025-15767-2) — **NEW to the corpus, but tissue-level (StO₂), not venous.** A head-to-head device-comparison study (SFDI vs transcutaneous oximetry vs wearable plethysmography vs pulse oximetry) in healthy tissue. It reports that **SFDI uniquely detected significant StO₂ differences** while device-to-device correlations were only moderate-to-fair (PO↔WD r = 0.44–0.59; SFDI↔TCOM r = 0.23–0.36). Added below as a *context lead* with an honest tissue-level flag — it is a methodological cross-check on the wide-field-imaging vs contact-PPG device classes, not a venous-oxygen measurement.
- All standing measurement anchors (Alqahtani jugular optical sensor, IJV DNN/Monte-Carlo, peripheral-venous modulation, e-tattoo, Mespere VO100, Noninvasix LIVOx optoacoustic ScvO₂, IJV-PA human, APM+ radial-vein PA, retinal-oximetry review, intravascular PACT, ADS-vis-OCT) — **carried forward, no change.**

**Per the standing brief: fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical *new* papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new primary measurement items today.* Standing best-available set (all previously surfaced), scores carried forward. **No primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90 % band (≈70–75 % across a three-subject set: 71.1 / 72.2 / 70.4 %).
- **Integration insight:** Anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck.

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
- **Integration insight:** The wearable-form embodiment of the venous-oximetry goal; its arterial/venous separation problem is the same one §1.3 attacks by modulation and §1.1 sidesteps by anatomy. The standing JMIR hypoxia-accuracy caution bears directly on this device class.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Authors:** (VO100 clinical validation group)
- **Year / Venue:** 2023/2024 · *J. Cardiothorac. Vasc. Anesth.* (S1053-0770 lineage) / ScienceDirect
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826
- **Relevance:** 7.5/10 — the one commercially available non-invasive jugular-NIRS ScvO₂ estimator clinically evaluated in critically ill patients.
- **Novelty:** Continuous non-invasive ScvO₂ estimate from an external jugular NIRS sensor, positioned as an alternative when catheter-based sampling is difficult.
- **Integration insight:** The clinical-translation benchmark for Topic 1 — the accuracy/bias any research-grade optical venous device (§1.1–1.4) must beat to matter at the bedside.

### 1.6 — Noninvasix LIVOx Optoacoustic Central Venous Oxygenation Monitor (ScvO₂ for septic shock) *(previously surfaced — newly catalogued scan 08-11; device/regulatory anchor, not new research)*
- **Authors / Sponsor:** Noninvasix Inc. (optoacoustic platform; Esenaliev / Petrov technology lineage, UTMB Galveston)
- **Year / Venue:** **2022** FDA **Breakthrough Device Designation** (device/regulatory milestone, not a peer-reviewed measurement paper)
- **Link:** https://noninvasix.com/ · trade coverage via BioWorld / NS Medical Devices / 24x7 (snippet-verified)
- **Relevance:** 8.0/10 to Topic 1 as a **device/translation anchor** — a chest-worn *optoacoustic* probe for non-invasive, real-time ScvO₂ in adults at risk of septic shock; arguably the most clinically advanced non-invasive *venous*-oxygen device on a regulatory pathway.
- **Novelty:** Optoacoustic (laser-induced ultrasound) readout of central venous oxygenation without a catheter; same platform demonstrated superior-sagittal-sinus venous sO₂ through the open fontanelle in preterm infants.
- **Integration insight:** The commercial/regulatory endpoint of the Esenaliev/Petrov large-vein optoacoustic lineage — the bedside destination the research-grade PA venous work (§2.2) is climbing toward; methodologically continuous with Topic-2 photoacoustics, making it the natural bridge between the two topics.
- **Honest flags:** **Not new research** — the designation dates to 2022 and is snippet-verified only; primary source pages were egress-blocked/403 today.

**Topic 1 honest note:** every measurement entry above is previously surfaced; nos. 1.3 and 1.5 predate 2023, and §1.6 is a 2022 regulatory milestone. The absence of *new* primary venous measurement work today is itself the finding, not a gap in searching.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new items today.* Carried-forward measurement anchors with scores held.

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
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring.
- **Novelty:** The arterial prior method (APM+) leverages high arterial sO₂ to locally calibrate optical fluence and correct wavelength-dependent spectral coloring, recovering deep-tissue venous sO₂ where conventional linear unmixing fails. Phantom median estimation error 2.9 % vs 9.8 % for conventional linear unmixing.
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus; its fluence-correction strategy is the deep-vein counterpart to the retinal per-vessel corrections §2.4/§2.5 catalogue and to the Hybrid-Net / PINN spectral-unmixing leads.

### 2.3 — Retinal Oximetry: New Insights into Ocular and Systemic Diseases *(previously surfaced — scan 08-05; review of per-vessel retinal artery+vein sO₂)*
- **Authors:** Zhang W., Tu X., Wang X., et al.
- **Year / Venue:** 2025 · *Graefe's Archive for Clinical and Experimental Ophthalmology* 263:2101–2115
- **Link / DOI:** https://doi.org/10.1007/s00417-025-06831-8 · PMID 40254630 · PMC12414079
- **Relevance:** 7.5/10 — retinal veins are among the very few human sites where a true **intravascular venous sO₂** is read optically and non-invasively. (Retinal venular, per-vessel — not systemic SvO₂.)
- **Novelty:** Consolidates retinal oximetry across spectrophotometric-fundus, hyperspectral, and vis-OCT modalities; frames retinal artery *and vein* saturation as ocular + systemic biomarkers; enumerates vessel-diameter, pigmentation, and media-transparency error sources.
- **Integration insight:** Ties the Topic-2 retinal cluster (HSI; ADS-vis-OCT §2.5) into one framework and names, at review level, the exact per-vessel confounds a venular oximeter must correct — the retinal analogue of the fluence/spectral-coloring problem the deep-vein PA anchors face.
- **Metadata flag:** Bibliographic fields cross-confirmed (Springer + PubMed + PMC); **full text not read** (403) — summary is abstract/snippet-level.

### 2.4 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Authors:** (PACT intravascular flow/oxygenation group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741 · PMC11161372
- **Link / DOI:** https://doi.org/10.1364/BOE.518632 → https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741
- **Relevance:** 8.0/10 — resolves sO₂ heterogeneity and laminar-flow structure *inside* human vessels (incl. veins) with PACT.
- **Novelty:** First-time recovery of the parabolic laminar-flow wavefront inside a deep vein in vivo by exploiting intravascular oxygenation heterogeneity across multi-wavelength PA spectra.
- **Integration insight:** Shows PACT can read *within-lumen* venous oxygen structure, not just a vessel-average — the imaging counterpart to §2.3's "fuse oximetry with blood-flow measurement" thesis.
- **Metadata flag:** DOI numeral not re-verifiable on the Optica page today (403); Optica locator (boe-15-5-2741) + PMC11161372 + title/year cross-confirmed. Cite via the Optica URL; treat the raw DOI numeral as **unverified**.

### 2.5 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Authors:** (ADS-vis-OCT group)
- **Year / Venue:** 2023 · *Communications Medicine* 3:59
- **Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8 · PMC10126115
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3 % in veins; ≈1 % bias vs blood-gas across 0–100 % (ex-vivo phantom validation).
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans (arteries ≈95 %, veins ≈72 % in reported cohorts).
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the §2.3 review holds up as state-of-the-art for retinal venular oximetry.

---

## Standing context leads (not ranked in the top-5)

- **Comparative assessment of healthy tissue oxygenation using near-infrared imaging, transcutaneous oxygen measurement, and plethysmography** — El Masry, Li, Balasubramani, Roy, Sen, Gnyawali · *Scientific Reports* **15**:30424 (2025) · PMID 40830190 · PMC12365204 · DOI 10.1038/s41598-025-15767-2. **NEW to the corpus; tissue-level (StO₂), NOT venous.** Head-to-head comparison of SFDI, transcutaneous oximetry (TCOM), wearable plethysmography (WD), and pulse oximetry (PO) in healthy tissue: **SFDI uniquely detected significant StO₂ differences**; device-to-device correlations were only moderate-to-fair (PO↔WD r = 0.44–0.59; SFDI↔TCOM r = 0.23–0.36). Retained as a **methodological cross-check on the wide-field-imaging vs contact-PPG device classes** relevant to the wearable-venous devices (§1.3/§1.4) and the SFDI lead — it quantifies how poorly these device classes agree even at tissue level, a sobering baseline for any venous device claiming cross-modality agreement. **Metadata cross-confirmed via ≥2 index snippets** (Nature + PubMed + PMC listings); nature.com/pubmed egress-blocked today so full text not read.
- **Quantitative analysis of tissue oxygenation variability across anatomical landmarks in healthy individuals via NIRS** — *Scientific Reports* 2025 (s41598-025-23102-y). Tissue-level NIRS variability mapping; not venous. Newly seen today; noted only as a normative-baseline lead.
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** — arXiv:2512.15394 (Dec 2025). Joint vessel segmentation + sO₂ estimation without explicit fluence estimation (seg accuracy ≥0.978 sim / 0.998 exp; sO₂ MSE ≤0.048 sim / 0.003 exp). Not venous-specific but directly relevant to the deep-vein PA decoloring problem (§2.2). **arxiv.org egress-blocked today**; re-verified via index snippet only.
- **Optical Inversion and Spectral Unmixing of Spectroscopic PA Images with Physics-Informed Neural Networks (SPOI-AE)** — arXiv:2602.16357 (surfaced 06-11). PA decoloring/unmixing method giving biologically coherent optical-parameter, chromophore, and sO₂ estimates; not venous-specific. Method lead.
- **Distribution-Informed and Wavelength-Flexible Data-Driven Photoacoustic Oximetry** — arXiv:2403.14863. Learned spectral unmixing robust to unknown wavelength sets. Method lead, not venous-specific.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Inorganic sulfate solutions reproduce both optical absorption and Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm — a ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % range. Standing metrology lead.
- **SFDI-net / deep-learning-enabled spatial frequency domain imaging** — *J. Biomed. Opt.* 30(4):046008 (2025; PMC12014942). Real-time two-layer SFDI inversion to hemoglobin/sO₂ maps; tissue-level, includes venous-area respiratory-wave dynamics. Transferable wide-field lead, not intravascular venous.
- **PPG-waveform venous oximetry** (finger-PPG venous saturation from positive-pressure-ventilation modulation; measuring venous oxygenation from the PPG waveform). Foundational peripheral-venous method family; conceptual sibling of §1.3.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction** — *JMIR Formative Research*, 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation showing >FDA-threshold error in the hypoxemic range — a transferable accuracy caution for the wearable-venous device class (§1.3/§1.4/§1.6), which operates at even lower saturations.
- **Quantitative Oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065; worldscientific.com). Review scaffold under the deep-vein PA anchors; authors unverified.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus, triple-wavelength optoacoustic large-vein oximetry; transfontanelle cerebral oximetry, *Sci. Rep.* 2022 s41598-022-19350-x). Foundational venous-optoacoustic prior art, with a concrete commercial endpoint logged (§1.6, Noninvasix LIVOx).
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂; retained as the closest MSOT venous-challenge human data.

---

## Cross-topic synthesis

Today reinforces the series' central, honest finding: **non-invasive optical measurement of true venous blood oxygen is a low-volume field, and no new primary venous *measurement* appeared today** (thirteenth consecutive dry cycle). The only item genuinely new to the corpus — the **El Masry et al. *Scientific Reports* device-comparison study** — is **tissue-level StO₂, not venous**, and its most useful contribution is a cautionary one: even for *tissue* oxygenation in healthy subjects, four established modalities (SFDI, TCOM, wearable plethysmography, pulse oximetry) agree with one another only moderately-to-poorly (r as low as 0.23). That is a sobering baseline for the venous field, where the signal is smaller and the saturation range lower — it quantifies just how much cross-modality-agreement work any candidate venous device still owes.

The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — addressed by three complementary strategies:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.1, chest/SSS optoacoustic LIVOx §1.6) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, e-tattoo spatial filtering §1.4, DNN inversion §1.2, PPG-waveform venous oximetry).
3. **Physics-based decoloring** to correct wavelength-dependent fluence / spectral contaminants before unmixing (deep-tissue PA fluence correction §2.2, per-vessel spectral cleanup in vis-OCT §2.5, intravascular PACT §2.4, Hybrid-Net / SPOI-AE / distribution-informed unmixing leads, sulfate-phantom metrology).

No entry moved between these strategies today and no new instance of any of them was published. The most mature, highest-precision proving ground for the strategy-3 corrections remains **retinal venular oximetry** (§2.3/§2.5); the hardest open problem remains the **systemic deep vein**, where §2.1/§2.2 push PA fluence correction toward a clinically meaningful central-venous surrogate — and where §1.6 shows one optoacoustic embodiment has already reached a regulatory pathway. The counterweight is unchanged and now doubly underlined: even *arterial* wearable oximetry (the JMIR lead) fails in the low-saturation range where venous measurement lives, and today's device-comparison study shows even *tissue-level* modalities disagree substantially with each other. Net: **no bedside-ready systemic non-invasive SvO₂ optical *research* result emerged today**, and the honest population of strong, truly-venous, truly-optical *new* papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-12 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; nature.com and pubmed.ncbi.nlm.nih.gov were egress-blocked, arxiv.org was egress-blocked, and publisher full-text pages returned HTTP 403 to direct fetch in this environment (source-/policy-side; agent proxy healthy), so items flagged "full text not read" / "snippet-verified" are abstract- or snippet-level and flagged unverified fields are noted inline.*
