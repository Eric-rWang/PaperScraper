# Venous Oxygen Research Scan — 2026-07-27

**Search window:** Twenty-eighth scan in the series, run **two days** after 2026-07-25 (no scan on 07-26). Emphasis on work published or first-surfacing after 07-25, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph / eess.IV new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, Wiley (*Advanced Science*, *J. Biophotonics*), Springer, De Gruyter, MDPI (*Biosensors*), *CHEST* / ScienceDirect, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — arxiv.org, pmc.ncbi.nlm.nih.gov, opg.optica.org, advanced.onlinelibrary.wiley.com, the Nature domains, sciencedirect.com and biorxiv.org — returned **HTTP 403** to direct `WebFetch` in this environment today (confirmed again on arXiv:2512.15394 and PMC12858309). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar-style result blocks + PMC/ResearchGate/Optica/ScienceDirect/De Gruyter listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the seventh consecutive scan cycle with none.** Today's two-day sweep produced no new SvO₂/ScvO₂/optical-venous demonstration and, unlike the 07-25 cycle, no new-to-corpus secondary literature either. Every item returned by today's searches maps to something already catalogued. The venous top-5 sets for both topics are **unchanged from 07-25 and 07-21** and carried forward with scores held.

Specifically re-verified today as **previously surfaced** (with the query that returned each):
- The **Alqahtani** external-jugular optical SvO₂ sensor (De Gruyter CDBME-2024-2072) — re-returned by the ScvO₂-optical-sensor query; catalogued since 06-10 (§1.1).
- The **2017 "Proof of concept non-invasive estimation of peripheral venous oxygen saturation"** (BioMed. Eng. OnLine, s12938-017-0351-x) — re-returned by the wearable-venous-oximetry query; already surfaced in eight prior scans (06-17 → 07-01). *Not re-added.*
- **APM+** radial-vein PA oximetry (Sastry et al., *Adv. Sci.* 2026, advs.76366) — §2.2, surfaced/​upgraded 07-15.
- **Hybrid-Net** (arXiv:2512.15394, Dec 2025) — standing PA-oximetry technique lead since 06-11; the joint segmentation+sO₂ result re-returned by two of today's PA queries.
- The **SFDI vs TCOM vs plethysmography** healthy-tissue-oxygenation comparison (*Sci. Rep.* s41598-025-15767-2, Aug 2025) — StO₂/venous-occlusion, tissue-level; catalogued 06-11.
- Retinal **vis-OCT** oximetry (§2.3), **PACT** venous-flow (§2.4), the **sulfate blood phantom** metrology paper (§2.5), the **IJV-PA anchor** (arXiv:2303.10775, §2.1), the **IJV DNN + Monte-Carlo** work (*Opt. Lett.* 49(10):2669, §1.2), **Mespere VO100** jugular NIRS (§1.5), and the **McDiarmid MRI iSvO₂** / **SSL intra-cardiac MR** oximetry pair (§1.4, §1.3).

One item checked and **excluded as arterial-only**: *JMIR Formative Research* 2026 (e85253) — wearable **pulse-oximeter** performance under controlled hypoxia induction. Instrument-validation of SpO₂ (arterial); no venous-transferable technique, so not carried.

One item checked and **excluded as out-of-scope venue/topic**: a Jan-2026 systematic review/meta-analysis of **hyperspectral imaging for surgical-flap monitoring** (PMC12858309) — flap perfusion/StO₂ at tissue level, not a venous SvO₂ measurement or a directly venous-transferable optical method; PMC full text 403, metadata unverified. Noted, not carried.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (~70–72 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.4) aim to close. *Metadata cross-confirmed via De Gruyter listing + ResearchGate; full text 403 (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (multi-author; NIRS + DNN group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling / fluence-correction leg of the program; the physics-simulation twin of the self-supervised-learning approach in §1.3. Its accuracy is bounded by the pathlength/fluence assumptions the DPF-model preprint (standing lead) reformulates. *Cross-confirmed via Optica listing + Semantic Scholar; full text 403 (flagged).*

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

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** (critical-care cohort study)
- **Year / Venue:** 2023 · *J. Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PMID 37827917
- **Relevance:** **7/10** — non-invasive NIRS surrogate for ScvO₂, clinical cohort.
- **Novelty:** Validates transcutaneous jugular NIRS (Mespere VO100) against invasive ScvO₂ in critically ill patients, reporting strong linear correlation with low bias/percentage error.
- **Integration insights:** The most clinically-mature non-invasive venous-NIRS device line — the practical baseline on bias and limits-of-agreement any optical/PA method must beat. Its accuracy floor is set by exactly the CW-NIRS pathlength assumptions the DPF-model preprint (standing lead) targets. *Cross-confirmed via ScienceDirect + PubMed 37827917; full text 403 (flagged).*

**Standing context (not scored in the top-5):** jugular transcutaneous NIRS in pediatric cardiac surgery (r = 0.91 vs ScvO₂, bias 2.92 %; PMC7491293), respiration-frequency-selected NIRS for cerebral SvO₂ (PMC4126245 / PMID 24439329), NIRS cerebral-oximetry tracking of mixed-venous SvO₂ (retrospective, *Sci. Rep.* s41598-023-49078-1), capnodynamic mixed-venous SvO₂ (NCT06632197; PMID 34609659), near-infrared spiroximetry venous saturation in piglets/humans (PMC3786737), the preterm-neonate NIRS venous-occlusion series (PMC8831784), and the 2017 proof-of-concept peripheral-venous pulse-oximetry calibration model (BioMed. Eng. OnLine s12938-017-0351-x) — all previously catalogued, none updated this cycle.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new venous-specific primary today.* The standing set carried forward with scores held. No new-to-corpus reviews or preprints this cycle.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** Gao / Zhu et al. (WashU / Garcia-Uribe lineage)
- **Year / Venue:** 2023 · arXiv preprint (dual-wavelength PAT + US); SPIE lineage (cf. 2014 SPIE 8943E..1MG)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** **10/10** — the single most on-target paper in the corpus: non-invasive, in-vivo, human, **internal-jugular venous** sO₂ (sijvO₂ ≈ 72 ± 7 %, n=7) by photoacoustics co-registered with ultrasound.
- **Novelty:** Reference demonstration that optical/PA deep-vein venous oximetry is physically achievable in a named deep vein in humans, in real time, with arterial-admixture-free specificity.
- **Integration insights:** The deep-vein anchor that everything else is measured against; APM+ (§2.2), APRECOT and the DPF model (standing leads) are all, in different ways, attempts to make this class of measurement quantitative and fluence-robust without an ultrasound co-registration crutch. Also the centerpiece of the *CHEST* clinical review (standing lead). *Metadata cross-confirmed via arXiv + ADS; full text 403 (flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry / Olick-Gibson et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366 · https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** **8/10** — a bona-fide non-invasive optical/PA venous-oximetry demonstration in humans (radial-vein median sO₂ 72.3 %, IQR 8.9 %, n=8 healthy adults; phantom median error 2.9 % vs 9.8 % linear unmixing).
- **Novelty:** Uses the neighbouring radial **artery** as an in-situ fluence calibrator to circumvent spectral coloring, requiring only two wavelengths and no hardware change to a standard dual-wavelength PAT system, then reports the adjacent **vein's** sO₂ in the physiological 60–80 % band.
- **Integration insights:** The clearest worked example of internal-reference calibration on the optical side and the corpus's second in-vivo human non-invasive optical venous result after the IJV-PA anchor (§2.1). The fluence-calibration problem it solves locally is the same one APRECOT attacks globally with anatomical priors. *Metadata cross-confirmed via Wiley + arXiv oximetry snippets; full text 403 (flagged).*

### 2.3 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (Yi / vis-OCT group; OHSU/Northwestern lineage)
- **Year / Venue:** 2023 · *Communications Medicine* (Nature) — s43856-023-00288-8
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8 · PMC10126115 · PMID 37095177
- **Relevance:** **7/10** — resolves **retinal-vein** sO₂ at single-vessel scale (venous ~48–72 % vs arterial ~92–95 % in normals); ~1 % bias vs blood-gas in phantoms, ~2.1 % RMSE vs pulse oximeter in human arteries (n=18).
- **Novelty:** ADS-vis-OCT adaptively removes per-vessel spectral contaminants, giving highly repeatable (≤2.5 %) per-vessel sO₂ across vessel types — the highest-accuracy per-vessel optical oximetry demonstrated.
- **Integration insights:** The retina is the one site where per-vessel optical venous saturation is routinely achievable; its adaptive spectral-contaminant-removal is exactly the class of correction a deep-vein PA/optical system needs to reach absolute SvO₂. *Cross-confirmed via Nature + PMC10126115; full text 403 (flagged).*

### 2.4 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-11 §2.2 / 06-10)*
- **Authors:** (PACT group)
- **Year / Venue:** 2024 · PMC11161372
- **Link / DOI:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** **7/10** — non-invasive PACT resolving intravascular oxygenation heterogeneity and the parabolic laminar-flow wavefront inside a deep human vein in vivo, from multi-wavelength PA spectra.
- **Novelty:** Shows oxygenation gradients inside a vessel can serve as endogenous contrast to visualize flow patterns, implicitly demonstrating spatially-resolved venous sO₂ within a single vessel lumen and coupling oxygenation to flow dynamics.
- **Integration insights:** Argues venous sO₂ is a spatial field, not a single number, and adds the **flow** leg that — combined with saturation (§2.1/§2.2) — yields true venous oxygen-flux. The pulsatile/flow-dynamics framing is exactly the subject of the dynamic-PA pulsation review (standing lead). *Cross-confirmed via PMC listing; full text 403 (flagged).*

### 2.5 — Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations *(previously surfaced — scan 07-07 §2.2; metrology)*
- **Authors:** Davenet et al. (Sorbonne Université)
- **Year / Venue:** 2026 · *Applied Optics* 65(6):1974 (also arXiv 2512.01458, submitted 2025-12-01)
- **Link / DOI:** https://arxiv.org/abs/2512.01458 · https://opg.optica.org/ao/abstract.cfm?uri=ao-65-6-1974
- **Relevance:** **7/10** — metrology enabling venous-range PA oximetry (not itself a venous measurement).
- **Novelty:** Inorganic sulfate solutions reproduce both the optical absorption *and* the Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm, injectable into tissue-mimicking phantoms.
- **Integration insights:** You cannot claim SvO₂ accuracy at depth under unknown fluence without a ground-truth phantom matching blood's *photoacoustic* response across the venous ≈40–75 % range that arterially-tuned phantoms handle poorly — a practical prerequisite for validating the §2.1/§2.2 systems. *Cross-confirmed via arXiv abstract + Optica listing; full text 403 (flagged).*

---

## Standing context leads (not ranked in the top-5) — no changes this cycle

- **Gokhale S., "Emerging Technology for Noninvasively Measuring Oxygen Saturations," *CHEST* 169(2):401–410, February 2026** (DOI 10.1016/j.chest.2025.09.025; S0012-3692(25)05393-0). Clinical-audience review covering the **photoacoustic** route — dual-wavelength **IJV PAT+US** (§2.1) and **PA-TEE mixed-venous** monitoring — as the emerging answer to the unmet non-invasive-SvO₂ need. First *CHEST*-level clinical framing of the deep-vein PA program. *Surfaced 07-25; metadata cross-confirmed via Ovid + ScienceDirect + journal.chestnet.org listings; full text 403 (flagged).*
- **Zheng W., Huang C., Xia J., "Review of Pulsation Signal Detection and Applications in Dynamic Photoacoustic Imaging," *Biosensors (MDPI)* 15(9):591, 2025** (DOI 10.3390/bios15090591; PMC12467494). Technique review of pulsatile-signal extraction in dynamic PA — the arterial-vs-venous separation machinery underneath continuous sO₂ tracking. *Surfaced 07-25; cross-confirmed via PMC + ResearchGate.*
- **Non-invasive photoacoustic imaging of cerebral oxygenation and hemoglobin content in awake mice** — bioRxiv 2025.10.02.679935 (Oct 2025). Murine, cerebral/tissue-level; not systemic-venous or human. Technique lead only. *bioRxiv full text 403; details unverified (flagged).*
- **Two SPIE 2026 hyperspectral whole-blood items** (Quantitative Bioimaging Laboratory / fei-lab.org) — an algorithm-comparison study for sO₂ in whole blood by diffuse-reflectance hyperspectral imaging (≈Mar 2026) and a high-speed reflectance-based hyperspectral sO₂ approach (≈Apr 2026). In-vitro / tissue-level blood-optics metrology; not venous. Catalogued 07-21; SPIE-403, **unverified** (flagged).
- **Machine-learning multiple-illumination quantitative optoacoustic oximetry in humans** (PMC9203099) — learned spectral decoloring for real-time quantitative sO₂; general, not venous-specific. Standing technique lead.
- **APRECOT — Conditioning Deep Anatomical Prior Knowledge for Reconstruction of MSOT Images** (arXiv:2606.16835, June 2026) — joint tissue segmentation + bulk-chromophore recovery attacking the MSOT fluence problem; in-silico only, not venous. Standing lead.
- **Novel Differential Pathlength Factor (DPF) model for NIR diffuse optical imaging** (arXiv:2602.00283, submitted 2026-01-30) — Monte-Carlo-derived distance/property-dependent DPF models reducing modified-Beer-Lambert error at small source–detector separations; underpins every transcutaneous-NIRS venous method (§1.2, §1.5). Standing lead.
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** (arXiv:2512.15394, Dec 2025) — joint vessel segmentation + sO₂ without explicit fluence estimation; general PA-oximetry method, not venous-specific. Re-returned by today's PA queries. Standing technique lead.
- **ISDC — Integrated Spectral and Depth Compensation for PA sO₂/THb** (*J. Biomed. Opt.* 31(2):026002, Feb 2026; DOI 10.1117/1.JBO.31.2.026002; PMC12869027) — depth+spectral fluence correction, transferable to deep-vein PA oximetry. Standing lead.
- **In-vivo continuous monitoring of mixed venous SvO₂ by PA-TEE** (SPIE 9689E..2U, 2016 lineage; swine) — minimally-invasive esophageal PA oximetry; the mixed-venous PA thread cited in the *CHEST* review. Standing lead.
- **SFDI vs TCOM vs plethysmography healthy-tissue oxygenation** (*Sci. Rep.* s41598-025-15767-2, Aug 2025) — StO₂/venous-occlusion, tissue-level, not vessel-specific SvO₂. Catalogued 06-11; re-returned by today's SFDI query. Standing lead.
- **ClinicalTrials.gov NCT06632197** — capnodynamic non-invasive mixed-venous SvO₂ in adults — non-optical clinical-reference lead.

---

## Cross-topic synthesis

1. **Sparseness confirmed, not padded — seventh consecutive cycle with no new venous primary.** A two-day sweep across PubMed, arXiv (incl. new-listing pages), bioRxiv/medRxiv, Optica, SPIE, Wiley, Nature, MDPI and *CHEST* produced **no new non-invasive venous-O₂ measurement paper** post-dating 07-25, and — unlike 07-25 — no new secondary literature either. The Topic-1 (true SvO₂) and Topic-2 (optical venous) top-5 sets are unchanged and carried forward with scores held. The §2.1 IJV-PA anchor, the §2.2 APM+ radial-vein result, and the §2.3 retinal vis-OCT result remain the anchors; nothing newer displaces them.

2. **Today's searches re-surfaced only known work — a maturity signal, not a coverage gap.** Broad queries on optical SvO₂/ScvO₂, PA venous oximetry, jugular NIRS, vis-OCT retinal oximetry, SFDI/hyperspectral StO₂, and diffuse-optical peripheral-venous occlusion all returned papers already in the corpus. The two candidates that were *not* already carried both failed the venous test: a *JMIR* 2026 wearable **pulse-oximeter** hypoxia-validation study (arterial SpO₂, no venous-transferable method) and a Jan-2026 **hyperspectral flap-monitoring** meta-analysis (tissue-level perfusion, not vessel SvO₂). Both excluded with reasons stated rather than padded in.

3. **The central obstacle is unchanged: absolute quantification under unknown, wavelength- and depth-dependent fluence.** Every live thread converges on it from a different side — internal-reference calibration (APM+ §2.2; non-optically the MRI RV/LV T₂ ratio §1.4), global anatomical priors (APRECOT), better forward physics (DPF model), fluence-free deep learning (Hybrid-Net; §1.2 DNN+Monte-Carlo), depth+spectral compensation (ISDC), blood-mimicking phantoms across the venous range (§2.5), and temporal/pulsatile discrimination (the dynamic-PA pulsation review). A clinically accurate deep-vein SvO₂ system will likely **stack** several of these; no single paper yet does.

4. **Clinical framing continues to lead the definitive measurement.** The *CHEST* review (07-25 lead) remains the strongest signal that the non-invasive venous-PA idea is being surveyed for practitioners even though the primary evidence base is still thin (Alqahtani n=3; APM+ n=8 healthy; IJV-PAT n=7). MRI remains the referee for the label problem — T₂/intra-cardiac CMR oximetry (§1.3 SSL, §1.4 iSvO₂) measures true mixed-venous SvO₂ non-invasively and reference-grade, the natural validation target the optical/PA methods chronically lack.

---

*Scan generated 2026-07-27 (UTC). Twenty-eighth in series. No new primary venous-optical measurement; standing top-5 sets carried forward with scores held. All publisher full-text pages returned HTTP 403 to direct fetch in this environment; metadata cross-verified across independent search-index snippets as noted per item.*
