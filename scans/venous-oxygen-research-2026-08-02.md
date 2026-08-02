# Venous Oxygen Research Scan — 2026-08-02

**Search window:** Thirtieth scan in the series, run **two days** after 2026-07-31 (no scan on 08-01). Emphasis on work published or first-surfacing after 07-31, with the standard fallback to the best-available venous-specific work already catalogued. Sources swept today: PubMed/PMC, arXiv (incl. physics.med-ph new-listing sweep), bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics, JOSA A), SPIE / *J. Biomed. Opt.*, *Photoacoustics* (ScienceDirect), IEEE Xplore, Nature / *Sci. Rep.* / *Commun. Med.*, Wiley (*Advanced Science*, *J. Biophotonics*), Springer, De Gruyter, MDPI (*Sensors*/*Biosensors*), *CHEST* / ScienceDirect, ClinicalTrials.gov, ResearchGate, Semantic Scholar, ADS.

**Verification caveat:** As in every prior scan, publisher **full-text** pages — including spiedigitallibrary.org, pmc.ncbi.nlm.nih.gov, arxiv.org (list + abstract), opg.optica.org, advanced.onlinelibrary.wiley.com, sciencedirect.com, the Nature domains and biorxiv/medrxiv — returned **HTTP 403** to direct `WebFetch` in this environment today (the physics.med-ph new-listing sweep was likewise 403). Every reference below was therefore cross-checked across **at least two independent search-index snippets** (Google Scholar–style result blocks + SPIE Digital Library / PMC / ADS / ResearchGate / Optica / De Gruyter listings); per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — day summary

**No new venous-specific work of any kind today — no new primary measurement and no new-to-corpus technique lead.** This is the **ninth consecutive scan cycle with no new systemic-SvO₂/ScvO₂ demonstration**, and the first cycle since 07-31 with **no** new-to-corpus item on the imaging side either. Today's two-day sweep re-surfaced only the standing corpus across every modality (PA/PACT, NIRS/DOT, hyperspectral, vis-OCT, SFDI, MRI reference). Both topic top-5 lists are **carried forward unchanged, with scores held.**

The one change worth logging is a small **verification consolidation** rather than a new paper: today's SFDI-specific sweep surfaced the **Nature *Sci. Rep.* (Aug 2025) comparative-oxygenation study** (near-infrared imaging vs transcutaneous O₂ vs plethysmography, s41598-025-15767-2), which reports SFDI uniquely resolving StO₂ differences by tissue heterogeneity. It is **tissue-level StO₂, not venous**, and is logged only as a standing SFDI context lead (§ standing leads) — it does **not** enter either top-5.

Everything else returned today is **previously surfaced** or out-of-scope: the IJV-PA anchor (arXiv:2303.10775), APM+ radial-vein PA oximetry (Sastry/Olick-Gibson et al., *Adv. Sci.* 2026, 10.1002/advs.76366), the Tran/Fei hyperspectral retinal HSI system (*J. Biomed. Opt.* 31(3):036006), ADS-vis-OCT retinal oximetry (*Commun. Med.* 2023), the PACT intravascular oxygenation/flow paper (BOE 15(5):2741 / PMC11161372), the Alqahtani jugular optical sensor (De Gruyter CDBME 2024), the IJV DNN + Monte-Carlo work (*Optics Letters* 49(10):2669), the SSL intra-cardiac MR oximetry preprint, the McDiarmid MRI iSvO₂ model, the pulse-modulation peripheral-venous method, the sulfate blood-phantom metrology paper (arXiv:2512.01458 / *Appl. Opt.* 65(6):1974), Mespere VO100 jugular NIRS, the score-based-diffusion DOT preprint (arXiv:2602.03449), Hybrid-Net (arXiv:2512.15394), the distribution-informed data-driven oximetry preprint (arXiv:2403.14863), APRECOT, ISDC, the Gokhale *CHEST* review, and the Zheng dynamic-PA pulsation review. **No new primary venous demonstration.**

Honest sparseness statement, per the standing brief: **fewer than 5 genuinely strong, genuinely venous, genuinely non-invasive-optical papers exist for either topic** once arterial-only and tissue-level (StO₂) work is excluded. The lists below present the best available with honest relevance scores; several entries are explicitly flagged as tissue-/retinal-level, MRI-based, or metrology rather than true systemic SvO₂ optical measurement, and are retained only because the true-venous population is that thin.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new items today.* The standing best-available set (all previously surfaced) with scores carried forward. This remains the sparse topic: **no primary non-invasive venous-O₂ measurement paper has first-surfaced since before 2026-07-15.**

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* 10(2) (De Gruyter; CDBME-2024-2072)
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072
- **Relevance:** **8/10** — true, non-invasive, optical, venous (but n=3, no invasive co-oximetry reference).
- **Novelty:** A pulse-oximeter-style optical sensor over the external jugular vein isolates the EJV waveform and returns SvO₂ estimates (71.1 %, 72.2 %, 70.4 %) within the healthy 60–90 % band — still the closest thing to a wearable-form-factor optical SvO₂ device in the literature.
- **Integration insights:** The superficial/low-cost optical analogue of the deep IJV-PA anchor (§2.1); together they bracket the venous-optical problem from the shallow and deep ends. Its open problem — calibration against a blood-gas gold standard — is exactly what the APM+ artery-as-reference approach (§2.2) and MRI reference oximetry (§1.4) aim to close. *Metadata cross-confirmed via De Gruyter + ResearchGate again today; full text 403 (flagged).*

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (multi-author; NIRS + DNN group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** **7/10** — IJV-specific, non-invasive, inverse-modeling for venous saturation *change*.
- **Novelty:** Multi-channel NIRS + DNNs trained on subject-specific 3-D Monte-Carlo forward models recover ΔSijvO₂ non-invasively, tying measured reflectance to a physically-modelled forward problem — sidestepping the labelled-data bottleneck via simulation.
- **Integration insights:** The inverse-modeling / fluence-correction leg of the program; the physics-simulation twin of the self-supervised-learning approach in §1.3. Its accuracy is bounded by the pathlength/fluence assumptions the DPF-model preprint (standing lead) reformulates, and the score-based-diffusion DOT preprint (standing lead) is a direct methodological competitor for the same inverse problem *with* uncertainty. *Cross-confirmed via Optica listing + Semantic Scholar again today; full text 403 (flagged).*

### 1.3 — Leveraging Self-Supervised Learning for Non-Invasive Intra-Cardiac Magnetic Resonance Oximetry Assessment *(previously surfaced — scan 07-13 §1.1; MRI, not optical)*
- **Authors:** Jiayuan Chen, Thai-Hoang Pham, Ping Zhang, Juliet Varghese
- **Year / Venue:** 2026 (preprint posted 2026-07-01) · medRxiv
- **Link / DOI:** https://www.medrxiv.org/content/10.64898/2026.06.29.26356860v1.full — DOI `10.64898/2026.06.29.26356860`
- **Relevance:** **7/10** for non-invasive venous O₂; **3/10** for the optical thrust of Topic 2 (MRI, not optical).
- **Novelty:** Self-supervised pre-training (contrastive + masked image modeling) on >48,000 cardiac images, then fine-tuning for O₂-saturation regression **with uncertainty quantification** (MAE ≈ 3.70; claimed >15 % improvement over baselines). Recovers chamber-level (intra-cardiac) blood O₂ — true mixed-venous SvO₂ — non-invasively and reference-grade.
- **Integration insights:** The label-scarce SSL + uncertainty recipe is **directly portable** to the optical side, where labelled in-vivo SvO₂ ground truth is the binding constraint (cf. §1.2). Value as a cross-modality **validation target** and transferable ML methodology; its UQ framing rhymes with the DOT diffusion-model preprint (standing lead) on the optical side. *Metadata confirmed across two search snippets; abstract not readable (medRxiv 403).*

### 1.4 — Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure (imaging-derived iSvO₂) *(previously surfaced — scan 07-07 §1.1)*
- **Authors:** McDiarmid et al.
- **Year / Venue:** 2025/2026 · *JACC: Advances*
- **Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484 · https://www.jacc.org/doi/10.1016/j.jacadv.2025.102484 · PMC12869880 · PMID 41609283
- **Relevance:** **7/10** — true mixed-venous, non-invasive, clinically validated (MRI, not optical).
- **Novelty:** 628-patient validation of an imaging-derived mixed-venous SvO₂ from the RV/LV blood-pool T₂ ratio on cardiac MRI (R = 0.82 vs invasive SvO₂), anchored to right-heart catheterization and an independent predictor of mortality/HF-hospitalization.
- **Integration insights:** Sets the **absolute-accuracy and outcome-relevance benchmark** any optical SvO₂ method must match, in exactly the population (heart failure) where a cheap continuous optical surrogate would be most valuable. Its internal-reference (RV vs LV) logic recurs on the optical side as artery-vs-vein calibration (§2.2). *Cross-confirmed via JACC/ScienceDirect + PMC + PubMed; full text 403 (flagged).*

### 1.5 — Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11; peripheral-venous proof-of-concept)*
- **Authors:** (peripheral venous oximetry group; proof-of-concept + bypass-surgery evaluation lineage)
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:79 (s12938-017-0351-x); earlier bypass-surgery evaluation lineage (Loughborough, *Physiol. Meas.* 28(8):012, 2007, IOP)
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x · proof-of-concept: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5437414/
- **Relevance:** **7/10** — true peripheral-venous, non-invasive, optical (pulse-oximetry-derived), with a co-oximetry correlation.
- **Novelty:** Exploits the arterial-vs-venous compliance difference to induce a respiration-like modulation of the peripheral vasculature, making venous blood pulsatile so a pulse-oximeter sensor can read it; reports a strong linear correlation (r² ≈ 0.95) between the estimated venous modulation ratio and measured SvO₂.
- **Integration insights:** The methodological ancestor of the Alqahtani EJV device (§1.1) and the clearest demonstration that **induced venous pulsatility** is a viable route to isolating the venous signal without imaging — a low-cost complement to the deep-vein PA/imaging approaches of Topic 2, and the peripheral analogue of respiration-frequency NIRS venous separation. *Metadata cross-confirmed via BMC/Springer + IOPscience + ResearchGate again today; full text reachable in abstract only (403 on some mirrors).*

*(Note: the Mespere VO100 jugular-NIRS ScvO₂ study — *J. Cardiothoracic Vasc. Anesth.*, S1053-0770(23)00782-6, PMID 37827917 — and the respiration-frequency-selected cerebral-SvO₂ NIRS work (PMC4126245 / PMID 24439329) remain in the standing pool as clinical/technique context; they trade in and out of the visible top-5 with §1.5 depending on cycle and are unchanged today.)*

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new items today.* The standing set is carried forward with scores held.

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

### 2.3 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — scan 07-31 §2.3; per-vessel retinal artery/vein sO₂)*
- **Authors:** Ling (Martin) H. Tran, Kaleb Pruitt, Miles Bryarly, Ikenna Emordi, Ali Ali, Ling Ma, Baowei Fei (Quantitative Bioimaging Laboratory, UT Southwestern)
- **Year / Venue:** 2026 (published online 18 March 2026) · *Journal of Biomedical Optics* 31(3):036006
- **Link / DOI:** https://doi.org/10.1117/1.JBO.31.3.036006 · https://www.spiedigitallibrary.org/journals/journal-of-biomedical-optics/volume-31/issue-3/036006/ · PMC12997856
- **Relevance:** **7/10** — resolves **per-vessel retinal vein vs artery sO₂** non-invasively and optically; retinal/per-vessel, not systemic SvO₂ (hence not higher).
- **Novelty:** A compact dual-camera design — a **snapshot hyperspectral camera** (fast, low native spatial resolution ~0.2 mm/pixel) fused with a **high-resolution RGB camera** via **deep-learning pansharpening** — produces high-resolution hyperspectral retinal images (~0.1 mm/pixel, a 2× spatial-resolution gain) from which **retinal vessel diameter and oxygen saturation are extracted simultaneously**. The journal-grade, *validated* successor to the group's earlier SPIE-conference hyperspectral retinal items.
- **Integration insights:** The retina remains the one anatomical site where per-vessel optical **venous** saturation is routinely achievable, and this is the newest, highest-spatial-resolution snapshot-HSI route to it — a hyperspectral sibling to the ADS-vis-OCT retinal method (§2.4). Two lessons port to the deep-vein program: (i) **pansharpening/sensor-fusion** to buy spatial resolution without sacrificing spectral bands is a general fix for the resolution–spectrum trade-off that also limits multispectral PA/DOT; (ii) snapshot acquisition mitigates motion, echoing the motion-rejection concern in deep-tissue MSOT oximetry. Its per-vessel A/V separation is the retinal analogue of the artery-vs-vein internal-reference idea (§2.2). *Title, authors, venue, volume/issue/article-ID and DOI cross-confirmed via SPIE Digital Library listing + PMC12997856 + search-index snippets; full text 403 (flagged).*

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (Yi / vis-OCT group; OHSU/Northwestern lineage)
- **Year / Venue:** 2023 · *Communications Medicine* (Nature) — s43856-023-00288-8
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8 · PMC10126115 · PMID 37095177
- **Relevance:** **7/10** — resolves **retinal-vein** sO₂ at single-vessel scale (venous ~48–72 % vs arterial ~92–95 % in normals); ~1 % bias vs blood-gas in phantoms, ~2.1 % RMSE vs pulse oximeter in human arteries (n=18).
- **Novelty:** ADS-vis-OCT adaptively removes per-vessel spectral contaminants, giving highly repeatable (≤2.5 %) per-vessel sO₂ across vessel types — the highest-accuracy per-vessel optical oximetry demonstrated.
- **Integration insights:** The depth-resolved, interferometric counterpart to the snapshot-HSI system (§2.3): both deliver retinal per-vessel A/V sO₂ but trade off differently (vis-OCT = depth-resolved, single-vessel accuracy; HSI = snapshot, wide-field, pansharpened). Its adaptive spectral-contaminant-removal is exactly the class of correction a deep-vein PA/optical system needs to reach absolute SvO₂. *Cross-confirmed via Nature + PMC10126115 again today; full text 403 (flagged).*

### 2.5 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-11 §2.2 / 06-10)*
- **Authors:** (PACT group)
- **Year / Venue:** 2024 · *Biomedical Optics Express* 15(5):2741 (PMC11161372)
- **Link / DOI:** https://opg.optica.org/boe/fulltext.cfm?uri=boe-15-5-2741 · https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** **7/10** — non-invasive PACT resolving intravascular oxygenation heterogeneity and the parabolic laminar-flow wavefront inside a deep human vein in vivo, from multi-wavelength PA spectra.
- **Novelty:** Shows oxygenation gradients inside a vessel can serve as endogenous contrast to visualize flow patterns, implicitly demonstrating spatially-resolved venous sO₂ within a single vessel lumen and coupling oxygenation to flow dynamics.
- **Integration insights:** Argues venous sO₂ is a spatial field, not a single number, and adds the **flow** leg that — combined with saturation (§2.1/§2.2) — yields true venous oxygen-flux. The pulsatile/flow-dynamics framing is exactly the subject of the Zheng dynamic-PA pulsation review (standing lead). *Cross-confirmed via Optica BOE + PMC listing again today; full text 403 (flagged).*

---

## Standing context leads (not ranked in the top-5)

- **★ NEW context lead this cycle — "Comparative assessment of healthy tissue oxygenation using near-infrared imaging, transcutaneous oxygen measurement, and plethysmography," *Scientific Reports* (Aug 2025; s41598-025-15767-2).** Head-to-head comparison in which **SFDI uniquely detected significant StO₂ differences** attributable to tissue heterogeneity, versus tcpO₂ and plethysmography. **Tissue-level StO₂, not venous** — logged here only because SFDI can discriminate venous-vs-arterial occlusion by StO₂/HbO₂/HHb dynamics and is therefore a technique-context anchor for the wide-field-diffuse-optical leg. *Metadata confirmed via Nature listing + search snippet; full text 403 (flagged).*
- **Score-based diffusion models for diffuse optical tomography with uncertainty quantification** — Schneider F., Mozumder M., Tamarov K., Taghizadeh L., Tarvainen T., Helin T., Duong D.-L., arXiv:2602.03449 (submitted 2026-02-03). Diffusion-model posterior sampling (UCoS framework) for linearized difference-imaging DOT, delivering state-of-the-art reconstructions on this severely ill-posed inverse problem **with calibrated uncertainty**. Not a venous measurement, but the DOT inverse problem it solves is the one underneath every transcutaneous-NIRS/DOT venous method (§1.2, §1.5); its UQ is the optical-side echo of the SSL/UQ MRI work (§1.3). *Cross-confirmed via arXiv listing + search snippet; full text 403 (flagged).*
- **Deep Learning From Diffuse Optical Oximetry Time-Series: An fNIRS-Focused Review** — *IEEE* (2025/2026; document 11230578). Review of deep-learning methods applied to diffuse-optical oximetry *time-series*; fNIRS/tissue-level, not venous, but scaffolds the temporal-ML machinery (continuous tracking, artifact rejection) that any continuous optical SvO₂ monitor will need. *Title/venue from IEEE Xplore listing; full text not read (flagged).*
- **Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** — Davenet et al. (Sorbonne Université), 2026 · *Applied Optics* 65(6):1974 (also arXiv:2512.01458). Inorganic sulfate solutions reproduce both the optical absorption *and* the Grüneisen coefficient of whole blood at chosen sO₂ over 700–850 nm — a ground-truth phantom for validating deep-vein PA oximetry across the venous ≈40–75 % range that arterially-tuned phantoms handle poorly. Complements the Fei-lab anthropomorphic oximetry phantoms (arXiv:2503.23161). Standing metrology lead. *Cross-confirmed via arXiv + Optica listing; full text 403 (flagged).*
- **Gokhale S., "Emerging Technology for Noninvasively Measuring Oxygen Saturations," *CHEST* 169(2):401–410, February 2026** (DOI 10.1016/j.chest.2025.09.025; article ID S0012-3692(25)05393-0). Clinical-audience review that explicitly covers the **photoacoustic** route — the dual-wavelength **IJV PAT+US** demonstration (§2.1) and **PA-TEE mixed-venous** monitoring — as the emerging answer to the unmet need for a non-invasive SvO₂ monitor. First *CHEST*-level clinical framing of the deep-vein PA program. *Confirmed via journal.chestnet.org + ScienceDirect listings; full text 403 (flagged).*
- **Zheng W., Huang C., Xia J., "Review of Pulsation Signal Detection and Applications in Dynamic Photoacoustic Imaging," *Biosensors (MDPI)* 15(9):591, 2025** (DOI 10.3390/bios15090591; PMC12467494). Technique review of **pulsatile-signal extraction** in dynamic PA — isolating the pulsatile arterial component is the first step toward attributing the residual/respiration-modulated signal to the vein. *Confirmed via PMC + ResearchGate; full text 403 (flagged).*
- **Distribution-informed and wavelength-flexible data-driven photoacoustic oximetry** (arXiv:2403.14863) — learned spectral unmixing robust to unknown wavelength sets; general PA-oximetry method, not venous-specific. Standing technique lead.
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging** (arXiv:2512.15394, Dec 2025) — joint vessel segmentation + sO₂ without explicit fluence estimation (segmentation ≥0.978 sim / 0.998 exp; sO₂ MSE ≤0.048 sim / 0.003 exp); general PA-oximetry method, not venous-specific. Standing lead.
- **Machine-learning-enabled multiple-illumination quantitative optoacoustic oximetry in humans** (PMC9203099) — learned spectral decoloring for real-time quantitative sO₂; general optoacoustic oximetry, not venous-specific. Standing lead.
- **APRECOT — Conditioning Deep Anatomical Prior Knowledge for Reconstruction of MSOT Images** (arXiv:2606.16835, June 2026) — joint tissue segmentation + bulk-chromophore (oxygenation) recovery attacking the ill-posed MSOT fluence problem; **in-silico only**, not venous. Standing lead.
- **Novel Differential Pathlength Factor (DPF) model for NIR diffuse optical imaging** (arXiv:2602.00283, submitted 2026-01-30) — Monte-Carlo-derived distance/property-dependent DPF models reducing modified-Beer-Lambert error at small source–detector separations; underpins every transcutaneous-NIRS venous method (§1.2, §1.5). Standing lead.
- **ISDC — Integrated Spectral and Depth Compensation for PA sO₂/THb** (*J. Biomed. Opt.* 31(2):026002, Feb 2026; DOI 10.1117/1.JBO.31.2.026002; PMC12869027) — depth+spectral fluence correction, transferable to deep-vein PA oximetry. Standing lead.
- **Validation of photoacoustic/ultrasound dual imaging in evaluating blood oxygen saturation** (PMC9664893) — PA/US dual-modality sO₂ validation (phantoms, animal + human arteries); arterial-focused but the PA+US co-registration is the same scaffold as the IJV-PA anchor (§2.1). Standing technique lead.
- **Transfontanelle photoacoustic imaging for in-vivo cerebral oxygenation measurement** (*Sci. Rep.* 2022, s41598-022-19350-x; PMC9470703) — through-fontanelle PA oxygenation in large-animal in vivo; cerebral/tissue-level, not systemic-venous. Standing lead.
- **In-vivo continuous monitoring of mixed venous SvO₂ by PA-TEE** (SPIE 9689E..2U, 2016 lineage; swine) — minimally-invasive esophageal PA oximetry; the mixed-venous PA thread now cited in the Gokhale *CHEST* review. Standing lead.
- **ClinicalTrials.gov** — **NCT06632197** capnodynamic non-invasive mixed-venous SvO₂ in adults (non-optical clinical-reference lead); **NCT05161884** MRI-based non-invasive ScvO₂ validation; **NCT02476630** thenar StO₂ as a ScvO₂ surrogate; **NCT04778150 / NCT04624009** NIRS SjvO₂ in liver-transplant / critically-ill patients; **NCT01891188** NIRS hepatic-venous saturation. Clinical NIRS/reference venous leads.

---

## Cross-topic synthesis

**1. Ninth consecutive cycle with no new venous *primary* measurement, and the first quiet cycle on the imaging side since 07-31.** Today's two-day sweep produced **no new systemic-SvO₂/ScvO₂ demonstration** (Topic 1 unchanged) and — unlike 07-31, which promoted the Tran/Fei retinal-HSI system — **no new-to-corpus imaging item** either. Both top-5 lists are carried forward with scores held. This reconfirms the standing read that truly novel non-invasive venous-optical *measurement* publishes at quarterly-at-best cadence; the intervening scans document tooling around it, not the measurement itself.

**2. The retina remains the only site with two complementary optical venous modalities, and it did not move today.** The snapshot-HSI system (§2.3) alongside ADS-vis-OCT (§2.4) still bracket per-vessel retinal A/V sO₂ from the wide-field-snapshot and depth-resolved-single-vessel directions. The transferable lesson for the deep-vein program is unchanged and worth restating: exploit the artery/vein pairing as an internal reference (as APM+ §2.2 does), and buy resolution through sensor fusion rather than more wavelengths (as §2.3 does).

**3. The *systemic* optical-venous field still rests on exactly two human papers, both photoacoustic.** The IJV-PA anchor (§2.1, deep central vein, US-co-registered) and APM+ (§2.2, peripheral radial vein, artery-calibrated) remain the only two in-vivo human non-invasive *optical* venous-sO₂ results in the corpus, converging on ~72 % by opposite routes. Everything else true-venous is non-optical (MRI iSvO₂ §1.4, SSL intra-cardiac MR §1.3) or shallow/peripheral device work (Alqahtani EJV §1.1, pulse-modulation §1.5). No new entrant challenged this today.

**4. Fluence + ill-posedness + uncertainty remains the universal bottleneck; today added no new lever but re-surfaced the SFDI leg.** The standing tooling stack is unchanged — score-based-diffusion DOT with UQ (Schneider/Tarvainen), APM+ (artery-as-calibrator), ISDC (depth+spectral compensation), APRECOT (anatomical priors), the DPF model (pathlength), Hybrid-Net (fluence-free DL), and the sulfate/anthropomorphic phantoms (ground-truth validation). Today's only addition is a **wide-field-diffuse-optical (SFDI) context lead** showing SFDI's sensitivity to StO₂ heterogeneity (standing lead) — tissue-level, not venous, but a reminder that the wide-field diffuse-optical route can discriminate venous-vs-arterial occlusion and is under-represented among the true-venous entries. The recurring 2026 theme across modalities is still **uncertainty quantification**, which MRI (§1.3) and DOT (standing) now ship and the PA anchors (§2.1/§2.2) still largely lack.

**5. Open gaps carried forward, all still open.** (a) No continuous, calibrated, wearable optical SvO₂ device validated against blood-gas with published limits-of-agreement; (b) no quantitative deep-venous PA sO₂ with an in-situ fluence reference across multiple deep sites and the full venous 40–75 % range; (c) no non-invasive optical/PA SvO₂ method benchmarked head-to-head against reference CMR oximetry. Today closed none of these and added no new tooling toward them — a genuinely quiet cycle, honestly reported rather than padded.

---

*Scan generated 2026-08-02 (UTC). **No new venous-specific primary systemic SvO₂/ScvO₂ measurement (ninth consecutive cycle) and no new-to-corpus imaging item** — both topic top-5 lists carried forward unchanged with scores held. One new **standing context lead** logged: an SFDI comparative-oxygenation study (*Sci. Rep.* Aug 2025, s41598-025-15767-2) — tissue-level StO₂, not venous, not entering either top-5. Publisher full-text access was 403-blocked throughout this environment; every reference was cross-checked across ≥2 independent search-index snippets, with per-item verification notes and flags above.*
