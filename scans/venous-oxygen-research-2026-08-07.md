# Venous Oxygen Research Scan — 2026-08-07

**Search window:** Thirty-second scan in the series, run **two days** after 2026-08-05 (no scan on 08-06). Emphasis on work published or first-surfacing after 08-05, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph new-listing sweep — note egress caveat below), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), World Scientific (*J. Innov. Opt. Health Sci.*), Springer (Graefe's Archive), Wiley (*Advanced Science*, *J. Biophotonics*), De Gruyter, MDPI (*Biosensors/Sensors*), Frontiers (*Photonics*), Nature / *Sci. Rep.* / *Commun. Med.*, IEEE Xplore, JMIR, ClinicalTrials.gov, USPTO, ResearchGate, Semantic Scholar.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including link.springer.com, pmc.ncbi.nlm.nih.gov, pubmed.ncbi.nlm.nih.gov, opg.optica.org, worldscientific.com, sciencedirect.com and the Nature/Wiley domains — were not directly readable to `WebFetch` in this environment today, and **arxiv.org returned an explicit egress block** (proxy `EGRESS_BLOCKED`, not a source-side 403) so no arXiv `/abs/` page could be opened directly. Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + PubMed / PMC / Springer / Optica / World Scientific / De Gruyter / USPTO listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific *primary* measurement paper today — the eleventh consecutive scan cycle with none.** Consistent with the series' standing observation, truly novel non-invasive **venous**-optical measurement work publishes at very low volume, and today's two-day sweep produced **no new SvO₂/ScvO₂ demonstration**. The Topic-1 (true SvO₂) top-5 and the Topic-2 top-5 measurement anchors are unchanged and carried forward with scores held.

Today surfaced **one genuinely new-to-corpus item** (a technique/method preprint, logged as a standing lead — not a venous measurement):

- **★ NEW lead (Topic 2, technique) — "Optical Inversion and Spectral Unmixing of Spectroscopic Photoacoustic Images with Physics-Informed Neural Networks," arXiv:2602.16357 (Feb 2026).** Introduces the **Spectroscopic Photoacoustic Optical Inversion Autoencoder (SPOI-AE)**, a physics-informed neural network that performs sPA optical inversion and spectral unmixing **without assuming linearity**, jointly estimating optical parameters, chromophore concentrations, and percent sO₂ from multispectral initial-pressure images. This is a direct attack on the *same* fluence / spectral-coloring bottleneck that separates the two human venous-PA demonstrations (§2.1 IJV-PA, §2.2 APM+) from a quantitative clinical device, and it belongs to the "learning-based correction" family the JIOHS quantitative-PACT-oximetry review (standing lead) catalogues. Not venous-specific → standing lead, honest low venous score. *Title / arXiv ID / method name (SPOI-AE) cross-confirmed across two search-index snippets; **arXiv full text and author list could not be read (proxy egress block on arxiv.org)** — flagged as such.*

Everything else returned today is **previously surfaced** or out-of-scope: the IJV-PA anchor (arXiv:2303.10775), APM+ radial-vein PA oximetry (Sastry/Olick-Gibson et al., *Adv. Sci.* 2026, 10.1002/advs.76366), the Zhang et al. retinal-oximetry review (*Graefe's Archive* 2025, 10.1007/s00417-025-06831-8), the Tran/Fei hyperspectral retinal HSI system (*J. Biomed. Opt.* 31(3):036006), the Alqahtani jugular optical sensor (De Gruyter CDBME 2024), the IJV DNN + Monte-Carlo work (*Optics Letters* 49(10):2669), the ADS-vis-OCT retinal oximetry paper (*Commun. Med.* 2023), PACT intravascular oxygenation/flow (BOE 15(5):2741 / PMC11161372), the quantitative-PACT-oximetry review (*J. Innov. Opt. Health Sci.* 2026), the NI-PARS venous patent (USPTO US 10,327,646), the sulfate blood-phantom metrology paper (arXiv:2512.01458 / *Appl. Opt.* 65(6):1974), Mespere VO100 jugular NIRS, the McDiarmid MRI iSvO₂ model, the SSL intra-cardiac MR oximetry preprint, Hybrid-Net (arXiv:2512.15394), the distribution-informed data-driven oximetry preprint (arXiv:2403.14863), and the Karlas MSOT muscle-occlusion pilot. **No new primary venous demonstration.**

Honest sparseness statement, per the standing brief: **fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical papers first-surfaced today for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores; several entries are explicitly flagged as tissue-/retinal-level, MRI-based, or metrology rather than true systemic SvO₂ optical measurement, and are retained only because the true-venous population is that thin.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new primary items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** 9.0/10 — direct non-invasive optical SvO₂ at the external/internal jugular; the closest thing the corpus has to a pulse-oximeter-form venous device (but n=3, no invasive co-oximetry reference).
- **Novelty:** Proof-of-concept optical sensor that identifies the jugular venous waveform and estimates SvO₂ within the healthy 60–90% band across a small subject set.
- **Integration insight:** The anchor for the "wearable venous pulse oximeter" thesis; every Topic-1 wearable/peripheral entry is a variation on isolating the venous component this device targets at the neck. Its open problem — calibration against a blood-gas gold standard — is what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.4) aim to close. *Metadata re-confirmed via De Gruyter + ResearchGate today; full text not read (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN / Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 (Optica abstract locator; raw DOI numeral unverified — see metadata flag below)
- **Relevance:** 8.5/10 — model-based recovery of IJV sO₂ change from multi-channel NIRS reflectance.
- **Novelty:** Subject-specific 3-D Monte-Carlo forward models train a DNN to invert measured reflectance into IJV saturation change, addressing the partial-volume/overlying-tissue confound and sidestepping the labelled-data bottleneck via simulation.
- **Integration insight:** Supplies the computational-inversion half of the jugular-NIRS approach; complements §1.1's hardware. The Monte-Carlo-to-DNN pattern recurs in the Topic-2 PA fluence-correction work, and its physics-simulation training strategy is the same idea the new SPOI-AE PINN lead pushes further on the PA side.

> **Metadata flag:** §1.2 DOI string could not be re-verified on the Optica page today; the stable Optica abstract locator (ol-49-10-2669) and title/authors/year are cross-confirmed via two search-index snippets. Treat the raw DOI numeral as **unverified**; cite via the Optica abstract URL.

### 1.3 — Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11; peripheral-venous proof-of-concept)*
- **Authors:** (peripheral-venous oximetry group; BioMedical Engineering OnLine; earlier Loughborough bypass-surgery lineage)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:60 (s12938-017-0351-x); earlier *Physiol. Meas.* 28(8), 2007
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x
- **Relevance:** 8.0/10 — a foundational demonstration that an induced/modulated venous signal yields a peripheral SvO₂ estimate optically (reports r² ≈ 0.95 vs measured SvO₂).
- **Novelty:** Exploits the arterial-vs-venous compliance difference to induce cyclical venous fluctuation, lifting the venous component out of the low-SNR background so a PPG-style optical readout can estimate local venous saturation.
- **Integration insight:** The conceptual root of the "modulate the vein, then demodulate" family (muscle-stimulation PPG, e-tattoo spatial filtering) and the methodological ancestor of the Alqahtani EJV device (§1.1). Landmark; recurs because nothing newer has displaced it as the peripheral-venous proof-of-concept.

### 1.4 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂) *(previously surfaced — scan 07-07 §1.1; MRI, not optical)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** 7.0/10 for non-invasive venous O₂; low for the optical thrust (MRI, not optical) — retained as the accuracy/outcome benchmark.
- **Novelty:** 628-patient validation of an imaging-derived mixed-venous SvO₂ from the RV/LV blood-pool T₂ ratio on cardiac MRI (R = 0.82 vs invasive SvO₂), anchored to right-heart catheterization and an independent predictor of mortality/HF-hospitalization.
- **Integration insight:** Sets the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must match, in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. Its internal-reference (RV vs LV) logic recurs on the optical side as artery-vs-vein calibration (§2.2). *Cross-confirmed via JACC/ScienceDirect + PMC + PubMed; full text not read (flagged).*

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Authors:** (VO100 clinical validation group)
- **Year / Venue:** 2023/2024 · *J. Cardiothorac. Vasc. Anesth.* (S1053-0770(23)00782-6; PMID 37827917)
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · https://pubmed.ncbi.nlm.nih.gov/37827917/
- **Relevance:** 7.5/10 — the one commercially available non-invasive jugular-NIRS ScvO₂ estimator; clinically evaluated in critically ill patients (n=79, strong linear correlation vs reference in COVID-19 and post-liver-transplant groups).
- **Novelty:** Continuous non-invasive ScvO₂ estimate from an external jugular NIRS sensor (Mespere VO100), positioned as an alternative when catheter-based sampling is difficult.
- **Integration insight:** The clinical-translation benchmark for Topic 1 — the accuracy/bias any research-grade optical venous device (§1.1–1.3) must beat to matter at the bedside.

**Topic 1 honest note:** every entry above is previously surfaced; nos. 1.3 and 1.5 predate 2024. The absence of *new* primary venous measurement work today is itself the finding, not a gap in searching.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new top-5 items this cycle — the one new-to-corpus item (SPOI-AE PINN spectral unmixing) is a technique/method, not a venous measurement, and is logged as a standing lead.* The standing top-5 measurement anchors are carried forward with scores held.

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** Gao / Zhu et al. (WashU / Garcia-Uribe lineage)
- **Year / Venue:** 2023 · arXiv:2303.10775 (dual-wavelength PAT + US); SPIE lineage (cf. 2014 SPIE 8943E..1MG)
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9.5/10 — the single most on-target Topic-2 paper: non-invasive, in-vivo, human, **internal-jugular venous** sO₂ (sijvO₂ ≈ 72 ± 7%, n=7) by photoacoustics co-registered with ultrasound.
- **Novelty:** Reference demonstration that optical/PA deep-vein venous oximetry is physically achievable in a named deep vein in humans, in real time, with arterial-admixture-free specificity.
- **Integration insight:** The deep-vein anchor that everything else is measured against; APM+ (§2.2), the JIOHS review (standing lead), and the new SPOI-AE PINN lead are all, in different ways, attempts to make this class of measurement quantitative and fluence-robust. *Metadata cross-confirmed via arXiv listing + ADS + SPIE snippet; arXiv full text not read today (proxy egress block; flagged).*

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): in-vivo human radial-vein sO₂ *(previously surfaced — upgraded 07-15 §2.2)*
- **Authors:** Sastry, Olick-Gibson, et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://doi.org/10.1002/advs.76366 · https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9.0/10 — a bona-fide non-invasive optical/PA venous-oximetry demonstration in humans (radial-vein median sO₂ 72.3%, IQR 8.9%, n=8; phantom median error 2.9% vs 9.8% linear unmixing).
- **Novelty:** Uses the neighbouring radial **artery** as an in-situ fluence calibrator to circumvent spectral coloring, requiring only two wavelengths and no hardware change to a standard dual-wavelength PAT system, then reports the adjacent **vein's** sO₂ in the physiological 60–80% band.
- **Integration insight:** The most recent (2026) primary PA venous-oximetry advance in the corpus and the clearest worked example of internal-reference calibration on the optical side. The fluence-calibration problem it solves *locally* is exactly the "spectral coloring" bottleneck the JIOHS review frames as central and the new SPOI-AE PINN lead attacks *globally* with a learned nonlinear inversion. *Cross-confirmed via Wiley + arXiv oximetry snippets; full text not read (flagged).*

### 2.3 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (Yi / vis-OCT group; OHSU/Northwestern lineage)
- **Year / Venue:** 2023 · *Communications Medicine* (Nature) 3:59 — s43856-023-00288-8
- **Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8 · https://www.nature.com/articles/s43856-023-00288-8 · PMC10126115 · PMID 37095177
- **Relevance:** 8.5/10 — per-vessel retinal **vein** sO₂ (venous ~48–72% vs arterial ~92–95% in normals) with reported repeatability SD ≈ 2.3% in veins; ~1% phantom bias vs blood-gas.
- **Novelty:** Adaptively removes per-vessel spectral contaminants, yielding accurate, repeatable artery *and vein* sO₂ across varying vessel diameters in humans — the highest-accuracy per-vessel optical oximetry demonstrated.
- **Integration insight:** The highest-precision per-vessel venous optical readout in the corpus; the concrete modality the Zhang et al. retinal-oximetry review (standing lead) holds up as state-of-the-art for retinal venular oximetry, and the depth-resolved counterpart to the snapshot-HSI retinal system (§2.4).

### 2.4 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — scan 07-31 §2.3; per-vessel retinal artery/vein sO₂)*
- **Authors:** Ling (Martin) H. Tran, Kaleb Pruitt, Miles Bryarly, Ikenna Emordi, Ali Ali, Ling Ma, Baowei Fei (Quantitative Bioimaging Laboratory, UT Southwestern / fei-lab.org)
- **Year / Venue:** 2026 (published online 18 March 2026) · *Journal of Biomedical Optics* 31(3):036006
- **Link / DOI:** https://doi.org/10.1117/1.JBO.31.3.036006 · PMC12997856
- **Relevance:** 7.5/10 — resolves **per-vessel retinal vein vs artery sO₂** non-invasively and optically; retinal/per-vessel, not systemic SvO₂ (hence not higher).
- **Novelty:** A compact dual-camera design — a **snapshot hyperspectral camera** fused with a **high-resolution RGB camera** via **deep-learning pansharpening** — produces high-resolution hyperspectral retinal images (~0.1 mm/pixel, a 2× spatial-resolution gain) from which retinal vessel diameter and oxygen saturation are extracted simultaneously.
- **Integration insight:** The newest, highest-spatial-resolution snapshot-HSI route to per-vessel retinal venous saturation. Two lessons port to the deep-vein program: (i) pansharpening/sensor-fusion buys spatial resolution without sacrificing spectral bands — a general fix for the resolution–spectrum trade-off that also limits multispectral PA/DOT; (ii) snapshot acquisition mitigates motion. Its per-vessel A/V separation is the retinal analogue of the artery-vs-vein internal-reference idea (§2.2). *Title/authors/venue/DOI cross-confirmed via SPIE listing + PMC12997856; full text not read (flagged).*

### 2.5 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-11 / 06-10)*
- **Authors:** (PACT intravascular flow/oxygenation group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741 (PMC11161372)
- **Link / DOI:** https://doi.org/10.1364/BOE.518632 → https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741
- **Relevance:** 8.0/10 — resolves sO₂ heterogeneity and laminar-flow structure *inside* human vessels (incl. veins) with PACT.
- **Novelty:** First-time recovery of the parabolic laminar-flow wavefront inside a deep vein in vivo by exploiting intravascular oxygenation heterogeneity across multi-wavelength PA spectra.
- **Integration insight:** Shows PACT can read *within-lumen* venous oxygen structure, not just a vessel-average — argues venous sO₂ is a spatial field, not a single number, and adds the **flow** leg that, combined with saturation (§2.1/§2.2), yields true venous oxygen-flux. *Metadata flag: DOI numeral could not be re-verified on the Optica page today; the stable Optica locator (boe-15-5-2741) + title/year cross-confirmed. Cite via the Optica URL; treat the raw DOI numeral as unverified.*

---

## Standing context leads (not ranked in the top-5)

- **★ NEW this cycle — "Optical Inversion and Spectral Unmixing of Spectroscopic Photoacoustic Images with Physics-Informed Neural Networks," arXiv:2602.16357 (Feb 2026).** The **SPOI-AE** (Spectroscopic Photoacoustic Optical Inversion Autoencoder) — a physics-informed NN that performs sPA optical inversion + spectral unmixing **without a linearity assumption**, jointly estimating optical parameters, chromophore concentrations, and percent sO₂ and (per snippet) giving more biologically coherent estimates than conventional algorithms. General PA-oximetry method, not venous-specific; belongs to the "learning-based correction" family under the JIOHS quantitative-PACT-oximetry review, and is a direct methodological competitor/complement to Hybrid-Net and the distribution-informed data-driven oximetry preprint. *arXiv full text + author list not read (proxy egress block); title/ID/method-name cross-confirmed via two snippets. Standing lead, honest low venous score.*
- **Retinal oximetry: new insights into ocular and systemic diseases** — Zhang W., Tu X., Wang X., et al., *Graefe's Archive for Clinical and Experimental Ophthalmology* 263:2101–2115, 2025 (DOI 10.1007/s00417-025-06831-8; PMID 40254630; PMC12414079). Review treating retinal **venular** sO₂ as a first-class quantity across spectrophotometric-fundus, hyperspectral, and vis-OCT modalities; catalogues the per-vessel error sources (diameter, pigmentation, media). Review, not a device — standing lead. *(Surfaced 08-05; full text not read, flagged.)*
- **Quantitative oximetry with photoacoustic computed tomography: Principles, progress, and prospects** — *J. Innov. Opt. Health Sci.*, 2026 (DOI 10.1142/S1793545826300065; World Scientific). First journal-grade dedicated review of quantitative PACT sO₂ and the fluence/spectral-coloring bottleneck; the umbrella under which the deep-vein PA anchors, SPOI-AE, Hybrid-Net, ISDC and the DPF model all sit. **Author list unverified (publisher 403; flagged).** Standing lead.
- **NI-PARS (non-interferometric photoacoustic remote sensing), USPTO US 10,327,646** (illumiSonics / PARS lineage). Granted patent explicitly claiming **estimation of venous / cerebrovenous / central-venous O₂** via a non-contact, low-coherence probe-beam PA readout — one of the very few pieces of prior art naming venous sO₂ as an explicit design target for a non-contact optical/PA modality. IP/technique lead, not a measurement.
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Inorganic sulfate solutions reproduce both the optical absorption and the Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm — a ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75% range. Standing metrology lead.
- **Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac MR Oximetry** — Chen, Pham, Zhang, Varghese, 2026 · medRxiv (DOI 10.64898/2026.06.29.26356860). SSL + uncertainty-quantification recipe for chamber-level (true mixed-venous) O₂ regression; MRI not optical, but the label-scarce SSL+UQ methodology ports directly to the optical side. Standing lead.
- **Hybrid-Net** (arXiv:2512.15394, Dec 2025) — joint vessel segmentation + sO₂ without explicit fluence estimation; general PA-oximetry method. **Distribution-informed and wavelength-flexible data-driven photoacoustic oximetry** (arXiv:2403.14863 / PMC11151660) — learned spectral unmixing robust to unknown wavelength sets. Both standing leads, both in the same learning-based-correction family as the new SPOI-AE lead.
- **Karlas et al., MSOT of muscle perfusion/oxygenation under arterial and venous occlusion — human pilot** (*J. Biophotonics* 2020). Tissue-level (StO₂), not intravascular SvO₂, but the closest MSOT venous-challenge human data. Standing tissue-level lead.
- **ClinicalTrials.gov** — NCT04778150 / NCT04624009 (NIRS SjvO₂ in liver-transplant / critically-ill patients); NCT02476630 (thenar StO₂ as a ScvO₂ surrogate); NCT06632197 (capnodynamic non-invasive mixed-venous SvO₂). Clinical-reference / NIRS-venous leads.

---

## Cross-topic synthesis

Today reinforces the series' central, honest finding: **non-invasive optical measurement of true venous blood oxygen is a low-volume field, and no new primary venous *measurement* appeared today** (eleventh consecutive dry cycle). The two topics remain coupled by one problem — **isolating the venous signal and correcting the confound that corrupts its saturation estimate** — solved by three complementary strategies:

1. **Anatomical targeting** of a large, named vein (jugular optical sensing §1.1, jugular NIRS §1.5, IJV-PA §2.1) — pick a vessel big enough that the venous signal dominates.
2. **Signal modulation / separation** to lift a small venous component out of a noisy mixed background (peripheral-venous modulation §1.3, DNN inversion §1.2).
3. **Physics-based decoloring** to correct wavelength-dependent fluence / spectral contaminants before unmixing (deep-tissue PA fluence correction §2.2, per-vessel spectral cleanup in vis-OCT §2.3, intravascular PACT §2.5).

The one genuinely new item today — the **SPOI-AE physics-informed-NN preprint** — sits squarely in strategy 3. It is the latest move in a now-crowded methodological cluster (Hybrid-Net, distribution-informed data-driven oximetry, learned spectral decoloring, and the anatomical-prior APRECOT line) all attacking the fluence/spectral-coloring inversion that the JIOHS review named as *the* central obstacle. The telling pattern of 2026 is that **the correction tooling keeps converging while primary venous *measurements* do not**: the systemic optical-venous field still rests on exactly two in-vivo human photoacoustic demonstrations (IJV-PA §2.1, APM+ §2.2), both landing on ~72% by opposite routes, with everything else true-venous being non-optical (MRI iSvO₂ §1.4, SSL intra-cardiac MR) or shallow/peripheral device work (§1.1, §1.3). The three open gaps carried forward are all still open: (a) no continuous, calibrated, wearable optical SvO₂ device validated against blood-gas with published limits-of-agreement; (b) no quantitative deep-venous PA sO₂ with an in-situ fluence reference across multiple deep sites and the full venous 40–75% range; (c) no non-invasive optical/PA SvO₂ method benchmarked head-to-head against reference CMR oximetry. Today closed none of these — it added one more learned-inversion method (SPOI-AE) that, if it generalizes, is a candidate tool for gap (b). Net: the honest population of strong, truly-venous, truly-optical papers remains **fewer than five per topic** once arterial-only and tissue-level work is excluded.

---

*Scan generated 2026-08-07 (UTC). No new venous-specific **primary** SvO₂/ScvO₂ measurement (eleventh consecutive cycle); Topic-1 and Topic-2 top-5 lists carried forward with scores held. **One new-to-corpus item logged as a standing lead** (a technique, not a venous measurement): the SPOI-AE physics-informed-NN spectral-unmixing preprint (arXiv:2602.16357). Publisher full-text access was unavailable in this environment (source-side blocks), and arxiv.org returned an explicit proxy egress block, so every reference was cross-checked across ≥2 independent search-index snippets, with per-item verification notes and flags above.*
