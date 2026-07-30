# Venous Oxygen Research Scan — 2026-07-30

**Search window:** Twenty-ninth scan in the series, run **two days** after 2026-07-28 (no scan on 07-29). Emphasis on work published or first-surfacing after 07-28, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, Wiley (*Advanced Science*, *J. Biophotonics*), Springer, De Gruyter, MDPI (*Biosensors*), IOP (*J. Phys. Photonics*), *CHEST* / ScienceDirect, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including iopscience.iop.org, arxiv.org, pmc.ncbi.nlm.nih.gov, opg.optica.org, advanced.onlinelibrary.wiley.com, sciencedirect.com, the Nature domains, degruyterbrill.com and biorxiv/medrxiv — returned **HTTP 403** to direct `WebFetch` in this environment today (the new IOP review below was 403 on full text and confirmed via ≥2 index snippets only). Every reference was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar-style result blocks + ADS/ResearchGate/PMC/Optica/ScienceDirect/IOP listings); per-item notes state what was confirmed and what could not be read directly on a publisher page. Two WebSearch queries also returned transient "unavailable" errors today (retried via alternate phrasings).

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the eighth consecutive scan cycle with none.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical work publishes at very low volume, and today's two-day sweep produced **no new SvO₂/ScvO₂ demonstration** and no new-to-corpus *measurement* of any kind. Every venous-specific result returned today was already catalogued.

The only genuinely **new-to-corpus** item this cycle is **secondary literature (a review), not a measurement**, and is out-of-core-scope (general wearable NIRS, not venous):

- **★ NEW (standing lead, not top-5) — "Advances in fully integrated wearable near-infrared spectroscopy: hardware innovations and biomedical applications," *Journal of Physics: Photonics* (IOP), 2026** (DOI 10.1088/2515-7647/ae6ae4; published 2026-05-28). A hardware-focused review of miniaturized/integrated **wearable NIRS** — light sources, detectors, embedded processing, wireless — for continuous tissue-oxygenation monitoring. **Not** a venous measurement and not venous-specific, but relevant as the clearest recent survey of the *form-factor* leg of the goal: any future continuous, wearable optical SvO₂ device (cf. the Alqahtani EJV sensor §1.1, the peripheral pulse-modulation method §1.5) will be built on exactly this hardware base. Logged under Standing context leads.

Everything else returned today is **previously surfaced** or out-of-scope: the IJV-PA anchor (arXiv:2303.10775); APM+ radial-vein PA oximetry (Sastry et al., *Adv. Sci.* 2026, 10.1002/advs.76366); the Alqahtani jugular optical sensor (De Gruyter CDBME 2024); the IJV DNN + Monte-Carlo work (*Optics Letters* 49(10):2669); the peripheral-venous pulse-modulation method (BioMed Eng OnLine, s12938-017-0351-x); ADS-vis-OCT retinal oximetry (*Commun. Med.* 2023); PACT intravascular oxygenation/flow (PMC11161372); the sulfate blood-phantom metrology paper (arXiv:2512.01458 / *Appl. Opt.* 65(6):1974); Hybrid-Net (arXiv:2512.15394); the distribution-informed data-driven oximetry preprint (arXiv:2403.14863); the SSL intra-cardiac MR oximetry preprint; the McDiarmid MRI iSvO₂ model; the Mespere VO100 jugular NIRS study; the Gokhale *CHEST* review; and the Zheng dynamic-PA pulsation review. **No new primary venous demonstration.**

Honest sparseness statement, per the standing brief: **fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical papers exist for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores; several entries are explicitly flagged as tissue-level, MRI-based, or metrology rather than true SvO₂ optical measurement, and are retained only because the true-venous population is that thin.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (~70–75 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.4) aim to close. The wearable-NIRS hardware review new this cycle (standing lead) is the natural build path for turning this proof-of-concept into a continuous device. *Metadata cross-confirmed via De Gruyter/DeGruyterBrill + ResearchGate (pub. 387159780) again today; full text 403 (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (multi-author; NIRS + DNN group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling / fluence-correction leg of the program; the physics-simulation twin of the self-supervised-learning approach in §1.3. Its accuracy is bounded by the pathlength/fluence assumptions the DPF-model preprint (standing lead) reformulates. *Cross-confirmed via Optica listing + Semantic Scholar again today; full text 403 (flagged).*

### 1.3 — Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment *(previously surfaced — scan 07-13 §1.1; MRI, not optical)*
- **Authors:** Jiayuan Chen, Thai-Hoang Pham, Ping Zhang, Juliet Varghese
- **Year / Venue:** 2026 (preprint posted 2026-07-01) · medRxiv
- **Link / DOI:** https://www.medrxiv.org/content/10.64898/2026.06.29.26356860v1.full — DOI `10.64898/2026.06.29.26356860`
- **Relevance:** **7/10** for non-invasive venous O₂; **3/10** for the optical thrust of Topic 2 (MRI, not optical).
- **Novelty:** Self-supervised pre-training (contrastive + masked image modeling) on >48,000 cardiac images, then fine-tuning for O₂-saturation regression **with uncertainty quantification** (MAE ≈ 3.70; claimed >15 % improvement over baselines). Recovers chamber-level (intra-cardiac) blood O₂ — true mixed-venous SvO₂ — non-invasively and reference-grade.
- **Integration insights:** The label-scarce SSL + uncertainty recipe is **directly portable** to the optical side, where labelled in-vivo SvO₂ ground truth is the binding constraint (cf. §1.2). Value as a cross-modality **validation target** and transferable ML methodology. *Metadata confirmed across two search snippets; abstract not readable (medRxiv 403).*

### 1.4 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂) *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · https://www.jacc.org/doi/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **7/10** — true mixed-venous, non-invasive, clinically validated (MRI, not optical).
- **Novelty:** 628-patient validation of an imaging-derived mixed-venous SvO₂ from the RV/LV blood-pool T₂ ratio on cardiac MRI (R = 0.82 vs invasive SvO₂), anchored to right-heart catheterization and an independent predictor of mortality/HF-hospitalization.
- **Integration insights:** Sets the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must match, in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. Its internal-reference (RV vs LV) logic recurs on the optical side as artery-vs-vein calibration (§2.2). *Cross-confirmed via JACC/ScienceDirect + PMC + PubMed; full text 403 (flagged).*

### 1.5 — Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11; peripheral-venous proof-of-concept)*
- **Authors:** (peripheral venous oximetry group; proof-of-concept + bypass-surgery evaluation lineage)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:79 (s12938-017-0351-x); earlier bypass-surgery evaluation lineage (Loughborough, *Physiol. Meas.* 28(8), 2007)
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x · https://biomedical-engineering-online.biomedcentral.com/articles/10.1186/s12938-017-0351-x
- **Relevance:** **7/10** — true peripheral-venous, non-invasive, optical (pulse-oximetry-derived), with a co-oximetry correlation.
- **Novelty:** Exploits the arterial-vs-venous compliance difference to induce a respiration-like modulation of the peripheral vasculature, making venous blood pulsatile so a pulse-oximeter sensor can read it; reports a strong linear correlation (r² ≈ 0.95) between the estimated venous modulation ratio and measured SvO₂.
- **Integration insights:** The methodological ancestor of the Alqahtani EJV device (§1.1) and the clearest demonstration that **induced venous pulsatility** is a viable route to isolating the venous signal without imaging — a low-cost complement to the deep-vein PA/imaging approaches of Topic 2, and the peripheral analogue of respiration-frequency NIRS venous separation. *Metadata cross-confirmed via BMC/Springer + ResearchGate (pub. 317067368) again today; full text reachable in abstract only (403 on some mirrors).*

*(Note: the Mespere VO100 jugular-NIRS ScvO₂ study — *J. Cardiothoracic Vasc. Anesth.*, S1053-0770(23)00782-6 — and the respiration-frequency-selected cerebral-SvO₂ NIRS work (PMC4126245 / PMID 24439329) remain in the standing pool as clinical/technique context; they trade in and out of the visible top-5 with §1.5 depending on cycle and are unchanged today.)*

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new venous-specific primary today.* The standing set carried forward with scores held; no new-to-corpus *measurement* this cycle (the one new item is the general wearable-NIRS hardware review, logged under Standing context leads).

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** Gao / Zhu et al. (WashU / Garcia-Uribe lineage)
- **Year / Venue:** 2023 · arXiv preprint (dual-wavelength PAT + US); SPIE lineage (cf. 2014 SPIE 8943E..1MG)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **10/10** — the single most on-target paper in the corpus: non-invasive, in-vivo, human, **internal-jugular venous** sO₂ (sijvO₂ ≈ 72 ± 7 %, n=7) by photoacoustics co-registered with ultrasound.
- **Novelty:** Reference demonstration that optical/PA deep-vein venous oximetry is physically achievable in a named deep vein in humans, in real time, with arterial-admixture-free specificity.
- **Integration insights:** The deep-vein anchor that everything else is measured against; APM+ (§2.2), APRECOT and the DPF model (standing leads) are all, in different ways, attempts to make this class of measurement quantitative and fluence-robust without an ultrasound co-registration crutch. Also the centerpiece of the Gokhale *CHEST* clinical review (standing lead). *Metadata cross-confirmed via arXiv + ADS + SPIE listing again today; full text 403 (flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry / Olick-Gibson et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366 · https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** **8/10** — a bona-fide non-invasive optical/PA venous-oximetry demonstration in humans (radial-vein median sO₂ 72.3 %, IQR 8.9 %, n=8 healthy adults; phantom median error 2.9 % vs 9.8 % linear unmixing).
- **Novelty:** Uses the neighbouring radial **artery** as an in-situ fluence calibrator to circumvent spectral coloring, requiring only two wavelengths and no hardware change to a standard dual-wavelength PAT system, then reports the adjacent **vein's** sO₂ in the physiological 60–80 % band.
- **Integration insights:** The clearest worked example of internal-reference calibration on the optical side and the corpus's second in-vivo human non-invasive optical venous result after the IJV-PA anchor (§2.1). The fluence-calibration problem it solves locally is the same one APRECOT attacks globally with anatomical priors. *Metadata cross-confirmed via Wiley + arXiv oximetry snippets again today; full text 403 (flagged).*

### 2.3 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (Yi / vis-OCT group; OHSU/Northwestern lineage)
- **Year / Venue:** 2023 · *Communications Medicine* (Nature) — s43856-023-00288-8
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8 · PMC10126115 · PMID 37095177
- **Relevance:** **7/10** — resolves **retinal-vein** sO₂ at single-vessel scale (venous ~48–72 % vs arterial ~92–95 % in normals; baseline parafoveal study reports venous 48.4 ± 5.0 %); ~1 % bias vs blood-gas in phantoms, ~2.1 % RMSE vs pulse oximeter in human arteries (n=18).
- **Novelty:** ADS-vis-OCT adaptively removes per-vessel spectral contaminants, giving highly repeatable (≤2.5 %) per-vessel sO₂ across vessel types — the highest-accuracy per-vessel optical oximetry demonstrated.
- **Integration insights:** The retina is the one site where per-vessel optical venous saturation is routinely achievable; its adaptive spectral-contaminant-removal is exactly the class of correction a deep-vein PA/optical system needs to reach absolute SvO₂. *Cross-confirmed via Nature + PMC10126115 + parafoveal baseline PMC9133487 again today; full text 403 (flagged).*

### 2.4 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-11 §2.2 / 06-10)*
- **Authors:** (PACT group)
- **Year / Venue:** 2024 · PMC11161372
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** **7/10** — non-invasive PACT resolving intravascular oxygenation heterogeneity and the parabolic laminar-flow wavefront inside a deep human vein in vivo, from multi-wavelength PA spectra.
- **Novelty:** Shows oxygenation gradients inside a vessel can serve as endogenous contrast to visualize flow patterns, implicitly demonstrating spatially-resolved venous sO₂ within a single vessel lumen and coupling oxygenation to flow dynamics.
- **Integration insights:** Argues venous sO₂ is a spatial field, not a single number, and adds the **flow** leg that — combined with saturation (§2.1/§2.2) — yields true venous oxygen-flux. The pulsatile/flow-dynamics framing is exactly the subject of the Zheng dynamic-PA pulsation review (standing lead). *Cross-confirmed via PMC listing again today; full text 403 (flagged).*

### 2.5 — Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations *(previously surfaced — scan 07-07 §2.2; metrology)*
- **Authors:** Davenet et al. (Sorbonne Université)
- **Year / Venue:** 2026 · *Applied Optics* 65(6):1974 (also arXiv 2512.01458, submitted 2025-12-01)
- **Link / DOI:** https://arxiv.org/abs/2512.01458 · https://opg.optica.org/ao/abstract.cfm?uri=ao-65-6-1974
- **Relevance:** **7/10** — metrology enabling venous-range PA oximetry (not itself a venous measurement).
- **Novelty:** Inorganic sulfate solutions reproduce both the optical absorption *and* the Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm, injectable into tissue-mimicking phantoms.
- **Integration insights:** You cannot claim SvO₂ accuracy at depth under unknown fluence without a ground-truth phantom matching blood's *photoacoustic* response across the venous ≈40–75 % range that arterially-tuned phantoms handle poorly — a practical prerequisite for validating the §2.1/§2.2 systems. Complemented by the anthropomorphic multispectral-oximetry phantom work (arXiv:2503.23161, standing lead). *Cross-confirmed via arXiv abstract + Optica listing again today; full text 403 (flagged).*

---

## Standing context leads (not ranked in the top-5; all previously surfaced except where marked ★ NEW)

- **★ NEW this cycle — "Advances in fully integrated wearable near-infrared spectroscopy: hardware innovations and biomedical applications," *Journal of Physics: Photonics* (IOP), 2026** (DOI 10.1088/2515-7647/ae6ae4; published 2026-05-28). A hardware-centric review of miniaturized/integrated **wearable NIRS** — dense integration of light sources and detectors, embedded processing, wireless telemetry — for continuous, real-time tissue-oxygenation monitoring. **Not** venous-specific and **not** a measurement; matters to this program as the clearest recent survey of the *form-factor / instrumentation* leg — the engineering base on which a continuous wearable optical SvO₂ device (cf. Alqahtani EJV §1.1, peripheral pulse-modulation §1.5) would be built. A companion IOP item, "Wearable NIRS device for low-resource settings" (DOI 10.1088/2515-7647/ae4cdf), and a "Wearable frequency-domain NIRS (FD-NIRS) system" (PMC12904531) surfaced alongside it — same wearable-NIRS/tissue-oxygenation thrust, none venous-specific. *Title, venue, DOI, and 2026-05-28 date cross-confirmed via two IOP index snippets; full text 403 (flagged); author list not readable on the publisher page today (unverified).*
- **Gokhale S., "Emerging Technology for Noninvasively Measuring Oxygen Saturations," *CHEST* 169(2):401–410, February 2026** (DOI 10.1016/j.chest.2025.09.025; article ID S0012-3692(25)05393-0). Clinical-audience review that explicitly covers the **photoacoustic** route — the dual-wavelength **IJV PAT+US** demonstration (§2.1) and **PA-TEE mixed-venous** monitoring — as the emerging answer to the unmet need for a non-invasive SvO₂ monitor. First *CHEST*-level clinical framing of the deep-vein PA program. *Confirmed via Ovid + ScienceDirect + journal.chestnet.org listings; full text 403 (flagged).*
- **Zheng W., Huang C., Xia J., "Review of Pulsation Signal Detection and Applications in Dynamic Photoacoustic Imaging," *Biosensors (MDPI)* 15(9):591, 2025** (DOI 10.3390/bios15090591; PMC12467494; U. at Buffalo). Technique review of **pulsatile-signal extraction** in dynamic PA — isolating the pulsatile arterial component is the first step toward attributing the residual/respiration-modulated signal to the vein. *Confirmed via PMC + ResearchGate; full text 403 (flagged).*
- **Anthropomorphic tissue-mimicking phantoms for oximetry validation in multispectral optical imaging** (arXiv:2503.23161, March 2025) — anatomically realistic phantoms for validating multispectral/optoacoustic sO₂ estimation; metrology, not venous. Complements the sulfate-phantom paper (§2.5) on the ground-truth-validation leg. Standing lead, re-confirmed present today.
- **Distribution-informed and wavelength-flexible data-driven photoacoustic oximetry** (arXiv:2403.14863) — learned spectral unmixing robust to unknown wavelength sets; general PA-oximetry method, not venous-specific. Standing technique lead, re-confirmed present today.
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** (arXiv:2512.15394, Dec 2025) — joint vessel segmentation + sO₂ without explicit fluence estimation; general PA-oximetry method, not venous-specific. Standing lead.
- **Transfontanelle photoacoustic imaging for in-vivo cerebral oxygenation measurement** (*Sci. Rep.* 2022, s41598-022-19350-x) — through-fontanelle PA oxygenation in large-animal in vivo; cerebral/tissue-level, not systemic-venous. Standing lead.
- **APRECOT — Conditioning Deep Anatomical Prior Knowledge for Reconstruction of MSOT Images** (arXiv:2606.16835, June 2026) — joint tissue segmentation + bulk-chromophore (oxygenation) recovery attacking the ill-posed MSOT fluence problem; **in-silico only**, not venous. Standing lead.
- **Novel Differential Pathlength Factor (DPF) model for NIR diffuse optical imaging** (arXiv:2602.00283, submitted 2026-01-30) — Monte-Carlo-derived distance/property-dependent DPF models reducing modified-Beer-Lambert error at small source–detector separations; underpins every transcutaneous-NIRS venous method (§1.2, §1.5). Standing lead.
- **ISDC — Integrated Spectral and Depth Compensation for PA sO₂/THb** (*J. Biomed. Opt.* 31(2):026002, Feb 2026; DOI 10.1117/1.JBO.31.2.026002; PMC12869027) — depth+spectral fluence correction, transferable to deep-vein PA oximetry. Standing lead.
- **Two SPIE 2026 hyperspectral whole-blood items** (Quantitative Bioimaging Laboratory) — in-vitro / tissue-level blood-optics metrology; **not** venous. Metadata SPIE-403 and **unverified** (flagged).
- **In-vivo continuous monitoring of mixed venous SvO₂ by PA-TEE** (SPIE 9689E..2U, 2016 lineage; swine) — minimally-invasive esophageal PA oximetry; the mixed-venous PA thread now cited in the Gokhale *CHEST* review. Standing lead.
- **ClinicalTrials.gov NCT06632197** — capnodynamic non-invasive mixed-venous SvO₂ in adults — non-optical clinical-reference lead. **NCT04778150** — NIRS SjvO₂ in liver-transplant surgery; **NCT04624009** — NIRS SjvO₂ vs ScvO₂ in critically ill patients (Geneva) — clinical NIRS-venous leads.

---

## Cross-topic synthesis

**1. Eighth consecutive null cycle — the publication rate, not a search gap.** Eight scans in a row with zero new primary non-invasive-venous-optical measurement papers is itself the finding: truly novel venous-specific optical work publishes at a quarterly-at-best cadence, not weekly. Today's two-day sweep across PubMed, arXiv (incl. the physics.med-ph new-listing page), bioRxiv/medRxiv, Optica, SPIE, Wiley, Nature, MDPI, IOP and *CHEST* re-confirmed every anchor is still current and surfaced no new venous *measurement* at any tier. The honest read for anyone tracking this space: watch the **~5 anchor programs**, not the weekly literature.

**2. This cycle's only new signal is instrumentation, not measurement — and that is a meaningful gap-shift.** The lone new-to-corpus item is a **wearable-NIRS hardware review** (*J. Phys. Photonics*, May 2026), joined by two more wearable-NIRS engineering items. None measures a vein. But their arrival points at the part of the problem that is *not* stuck: while the venous-sO₂ *algorithm/measurement* literature is frozen, the **wearable-optical hardware** it would run on is advancing steadily. The binding constraint on a deployable optical SvO₂ monitor was never the sensor package (the Alqahtani EJV device §1.1 and peripheral pulse-modulation §1.5 already show a wearable form factor works); it is calibrated venous specificity. Progress on the hardware leg without matching progress on the calibration leg widens, rather than closes, that gap.

**3. Two independent human demonstrations still bracket the problem, and both remain photoacoustic.** The IJV-PA anchor (§2.1, deep central vein, US-co-registered) and APM+ (§2.2, peripheral radial vein, artery-calibrated) are the only two in-vivo human non-invasive *optical* venous-sO₂ results in the corpus, converging on ~72 % by opposite routes. Everything else true-venous is either non-optical (MRI iSvO₂ §1.4, SSL intra-cardiac MR §1.3) or shallow/peripheral device work (Alqahtani EJV §1.1, pulse-modulation §1.5). The optical-venous field still rests on two papers.

**4. Fluence calibration remains the universal bottleneck; the corpus keeps converging on internal references.** APM+ (artery-as-calibrator), ISDC (depth+spectral compensation), APRECOT (anatomical priors), the DPF model (pathlength), and the phantom-metrology thread (§2.5 sulfate + arXiv:2503.23161 anthropomorphic phantoms) all attack the *same* ill-posed problem — recovering absolute sO₂ from a signal scaled by unknown local fluence — from complementary angles. The internal-reference idea (calibrate against something whose saturation you know: an adjacent artery, an RV/LV pool ratio) recurs across optical and MRI work alike and is the most promising unifying route to *absolute* venous SvO₂.

**5. Venous sO₂ is a spatiotemporal field, and the label-scarcity problem couples the modalities.** The PACT flow/oxygenation-heterogeneity work (§2.4) plus the dynamic-PA pulsation review reframe the target as saturation × flow = oxygen flux — the clinically meaningful variable. Meanwhile the binding constraint on optical venous oximetry is not hardware but **labelled in-vivo SvO₂ ground truth**: the MRI/ML entries (§1.3 SSL + uncertainty, §1.4 628-patient validation) matter to the optical program precisely as *transferable methodology and validation targets* — the SSL/uncertainty recipe ports to the data-starved optical side, and the MRI cohorts define the accuracy/outcome bar (R≈0.82 vs invasive; mortality prediction) any optical device must clear. **Open gaps carried forward, all still open:** (a) no continuous, calibrated, wearable optical SvO₂ device validated against blood-gas with published limits-of-agreement — the new wearable-NIRS hardware supplies the *platform* for exactly this; (b) no quantitative deep-venous PA sO₂ with an in-situ fluence reference across multiple deep sites and the full venous 40–75 % range beyond APM+'s single radial-vein demonstration; (c) no non-invasive optical/PA SvO₂ method benchmarked head-to-head against reference CMR oximetry. Today moved none of these.

---

*Scan complete. No new primary venous-specific optical measurement identified for 2026-07-30 (eighth consecutive null cycle). Top-5 sets carried forward unchanged with scores held. One new-to-corpus item logged as a standing context lead — a wearable-NIRS hardware review (*J. Phys. Photonics*, DOI 10.1088/2515-7647/ae6ae4, May 2026), general/tissue-oxygenation and not venous-specific. All metadata re-cross-confirmed against ≥2 independent index snippets today; publisher full-text 403 throughout this environment (flagged per item).*
