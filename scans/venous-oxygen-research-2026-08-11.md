# Venous Oxygen Research Scan — 2026-08-11

**Search window:** Thirty-third scan in the series, run **two days** after 2026-08-09. Emphasis on work published or first-surfacing after 08-09, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (physics.med-ph / eess.IV new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), Springer (Graefe's Archive), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Sensors/Biosensors/Biomedicines*), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, ClinicalTrials.gov, plus device/regulatory trade press (BioWorld, NS Medical Devices, 24x7) and Semantic Scholar / Google-Scholar-style index snippets.

**Verification caveat:** Publisher **full-text** pages (link.springer.com, pmc.ncbi.nlm.nih.gov, opg.optica.org, sciencedirect.com, nature.com, wiley.com) again returned **HTTP 403** to direct `WebFetch`, **arxiv.org is egress-blocked** in this environment today, and several **device-news domains** (hhmglobal.com, nsmedicaldevices.com) are **egress-blocked** by the proxy. The agent proxy itself reported healthy — the blocks are source-/policy-side, not relay failures. Every reference below was therefore cross-checked across **≥2 independent search-index snippets**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the twelfth consecutive scan cycle with none.** Today's two-day sweep produced **no new SvO₂/ScvO₂ demonstration**. The Topic-1 (true SvO₂) and Topic-2 (imaging-technique) top-5 measurement anchors are unchanged and carried forward with scores held.

Today's searches did surface two items that read as "recent" in the result blocks but are **already in the corpus**, plus one commercial/regulatory item **not previously named** in the corpus:

- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** (arXiv:2512.15394, Dec 2025) — **previously surfaced** (standing lead since the 08-03 cycle); joint vessel segmentation + sO₂ without explicit fluence estimation. Not venous-specific. No change.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood** (Davenet et al., *Applied Optics* 65(6):1974; also arXiv:2512.01458) — **previously surfaced** as a metrology lead. A ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % band. No change.
- **NEW to the corpus (but not new research): Noninvasix LIVOx optoacoustic ScvO₂ monitor** — a chest-worn *optoacoustic* device with **FDA Breakthrough Device Designation** for non-invasive, real-time central venous oxygen saturation in adults at risk of septic shock. Genuinely on-target for Topic 1 and **not previously named** in this corpus — but the designation dates to **2022**, and it is the commercial embodiment of the **Esenaliev/Petrov superior-sagittal-sinus optoacoustic lineage already logged** as a standing lead. Added below as a device anchor with an honest not-new flag; it does **not** represent new 2026 measurement work.

**Per the standing brief: fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical *new* papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new primary measurement items today.* Standing best-available set (all previously surfaced except §1.6, newly catalogued), scores carried forward. **No primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device.
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90 % band (≈70–75 % across a three-subject set).
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
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x
- **Relevance:** 8.0/10 — foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically.
- **Novelty:** External stimulation induces cyclical venous fluctuation, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** Conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.

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

### 1.6 — Noninvasix LIVOx Optoacoustic Central Venous Oxygenation Monitor (ScvO₂ for septic shock) *(NEWLY CATALOGUED this scan — but not new research; FDA designation 2022)*
- **Authors / Sponsor:** Noninvasix Inc. (optoacoustic platform; Esenaliev / Petrov technology lineage, UTMB Galveston)
- **Year / Venue:** **2022** FDA **Breakthrough Device Designation** (device/regulatory milestone, not a peer-reviewed measurement paper)
- **Link:** https://noninvasix.com/noninvasix-receives-fda-breakthrough-device-designation-for-non-invasive-monitoring-technology-for-sepsis/ · trade coverage: https://www.bioworld.com/articles/516374-noninvasix-breathes-easier-with-breakthrough-device-designation
- **Relevance:** 8.0/10 to Topic 1 as a **device/translation anchor** — a chest-worn *optoacoustic* probe for **non-invasive, real-time, continuous or spot ScvO₂** in adults at risk of septic shock; arguably the most clinically advanced non-invasive *venous*-oxygen device on a regulatory pathway.
- **Novelty:** Optoacoustic (laser-induced ultrasound) readout of central venous oxygenation without a catheter; disposable patient interface + reusable probe + display. Same platform demonstrated superior-sagittal-sinus venous sO₂ (SSSO₂) through the open fontanelle in preterm infants.
- **Integration insight:** The commercial/regulatory endpoint of the **Esenaliev/Petrov large-vein optoacoustic lineage** the corpus has carried as a standing lead — the bedside destination that the research-grade PA venous work (§2.2/§2.3) is climbing toward. Its optoacoustic approach is methodologically continuous with Topic-2 photoacoustics, making it the natural bridge between the two topics.
- **Honest flags:** **Not new research** — the Breakthrough designation is from **2022** and cross-confirmed via multiple trade-press snippets (BioWorld, NS Medical Devices, 24x7, company release); primary source pages were **egress-blocked** today, so the designation year and device description are **snippet-verified, not read on a publisher/regulatory page**. Added now only because the LIVOx device was never explicitly named in prior scans; it is a *newly catalogued* anchor, not a *newly published* finding.

**Topic 1 honest note:** every measurement entry above is previously surfaced; nos. 1.3 and 1.5 predate 2023, and the newly-catalogued §1.6 is a 2022 regulatory milestone. The absence of *new* primary venous measurement work today is itself the finding, not a gap in searching.

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

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366
- **Relevance:** 9.0/10 — in-vivo human **radial-vein** sO₂ via a deep-tissue PA method that explicitly tackles spectral coloring.
- **Novelty:** The arterial prior method (APM+) leverages high arterial sO₂ to locally calibrate optical fluence and correct wavelength-dependent spectral coloring, recovering deep-tissue venous sO₂ where conventional linear unmixing fails.
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus; its fluence-correction strategy is the deep-vein counterpart to the retinal per-vessel corrections §2.4 catalogues and to the Hybrid-Net / PINN spectral-unmixing leads.

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
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ with reported repeatability SD ≈ 2.3 % in veins; ≈1 % bias vs blood-gas across 0–100 %.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans (arterial RMSE vs pulse-oximeter ≈2.1 % across 18 participants).
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the §2.3 review holds up as state-of-the-art for retinal venular oximetry.

---

## Standing context leads (not ranked in the top-5)

- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** — arXiv:2512.15394 (Dec 2025). Joint vessel segmentation + sO₂ estimation without explicit fluence estimation; not venous-specific but directly relevant to the deep-vein PA decoloring problem (§2.2). **arxiv.org egress-blocked today**; re-verified via index snippet only.
- **Distribution-Informed and Wavelength-Flexible Data-Driven Photoacoustic Oximetry** — arXiv:2403.14863. Learned spectral unmixing robust to unknown wavelength sets. Method lead, not venous-specific.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Inorganic sulfate solutions reproduce both the optical absorption *and* Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm — a ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % range. Standing metrology lead.
- **SFDI-net / deep-learning-enabled spatial frequency domain imaging** — *J. Biomed. Opt.* 30(4):046008 (2025; PMC12014942). Real-time two-layer SFDI inversion to hemoglobin/sO₂ maps; tissue-level, includes venous-area respiratory-wave dynamics. Transferable wide-field lead, not intravascular venous.
- **Wearable NIRS for neck-vessel (carotid) hemodynamics — preliminary study** (PMC12384115). **Arterial (carotid)**, not venous; retained as a transferable wearable-NIRS neck-vessel form-factor lead.
- **Performance of Wearable Pulse Oximetry During Controlled Hypoxia Induction** — *JMIR Formative Research*, 2026 (formative.jmir.org/2026/1/e85253). **Arterial-only** wearable SpO₂ validation showing >FDA-threshold error in the hypoxemic range — a transferable accuracy caution for the wearable-venous device class (§1.3/§1.4/§1.6), which operates at even lower saturations.
- **Quantitative Oximetry with PACT: Principles, Progress, and Prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065). Review scaffold under the deep-vein PA anchors; authors unverified.
- **Classic ovine / large-vein optoacoustic SSS venous work** (Esenaliev/Petrov lineage; superior sagittal sinus, triple-wavelength optoacoustic large-vein oximetry). Foundational venous-optoacoustic prior art — now with a concrete commercial endpoint logged this scan (§1.6, Noninvasix LIVOx).
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂; retained as the closest MSOT venous-challenge human data.

---

## Cross-topic synthesis

Today reinforces the series' central, honest finding: **non-invasive optical measurement of true venous blood oxygen is a low-volume field, and no new primary venous *measurement* appeared today** (twelfth consecutive dry cycle). The one item new to the corpus — the **Noninvasix LIVOx optoacoustic ScvO₂ monitor (§1.6)** — is a *regulatory* milestone from **2022**, not a new measurement, but it is a meaningful addition: it is the first explicitly **FDA-Breakthrough-designated, non-invasive, central-venous** optical/optoacoustic device the corpus has named, and it sits exactly on the seam between the two topics — an optoacoustic (i.e. photoacoustic) readout deployed for the Topic-1 clinical endpoint (ScvO₂ in septic shock). It makes concrete the destination that the research-grade PA venous work (§2.1/§2.2) is climbing toward.

The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — addressed by three complementary strategies:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.1, and now the chest/SSS optoacoustic LIVOx §1.6) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, e-tattoo spatial filtering §1.4, DNN inversion §1.2).
3. **Physics-based decoloring** to correct wavelength-dependent fluence / spectral contaminants before unmixing (deep-tissue PA fluence correction §2.2, per-vessel spectral cleanup in vis-OCT §2.5, intravascular PACT §2.4, Hybrid-Net / distribution-informed unmixing leads, sulfate-phantom metrology).

No entry moved between these strategies today and no new instance of any of them was published. The most mature, highest-precision proving ground for the strategy-3 corrections remains **retinal venular oximetry** (§2.3/§2.5); the hardest open problem remains the **systemic deep vein**, where §2.1/§2.2 push PA fluence correction toward a clinically meaningful central-venous surrogate — and where §1.6 shows one optoacoustic embodiment has already reached a regulatory pathway. The counterweight is unchanged: even *arterial* wearable oximetry (the JMIR lead) fails in the low-saturation range where venous measurement lives, so the accuracy bar for any wearable venous device (§1.3/§1.4/§1.6) is, if anything, higher than the arterial state of the art. Net: **no bedside-ready systemic non-invasive SvO₂ optical *research* result emerged today**, and the honest population of strong, truly-venous, truly-optical *new* papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-11 (UTC). Metadata cross-checked across ≥2 search-index snippets per item; arxiv.org and several device-news domains were egress-blocked and publisher full-text pages returned HTTP 403 to direct fetch in this environment (source-/policy-side; agent proxy healthy), so items flagged "full text not read" / "snippet-verified" are abstract- or snippet-level and flagged unverified fields are noted inline.*
