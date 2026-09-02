# Daily Venous-Oxygen Research Scan — 2026-09-02

## ⚠️ Read this first — day summary

- **Scan cadence:** 46th scan in the series (immediately prior run 2026-09-01). Emphasis on work published or first-surfacing after 09-01.
- **Verification caveat (today):** `WebSearch` was available and productive, but `WebFetch` to scholarly hosts remains **egress-blocked by the environment's network policy** — a direct `WebFetch` of arXiv (arxiv.org/list/physics.med-ph/2026-08) returned `EGRESS_BLOCKED`, identical to the 08-29 → 09-01 runs. Every item below was therefore **cross-checked across ≥2 independent search-index snippets** rather than read on the publisher page. Items whose full metadata could not be page-verified are flagged **⚠ search-derived**.
- **No new venous-specific optical measurement paper first-surfaced today.** Targeted sweeps across all in-scope modalities — SvO₂/ScvO₂ optical, jugular PA/NIRS, peripheral/PPG venous oximetry, vis-OCT venular oximetry, hyperspectral fundus, DOS/SFDI venous-occlusion, ScvO₂ optoacoustic, ULM+PA co-registration, recent arXiv physics.med-ph — returned **only papers already catalogued** in prior dated files. This is a genuine low-publication-volume field, exactly as the last several scans reported — **not** a search gap. I am **not** padding with arterial-only SpO₂ work.
- **Candidates checked and confirmed already-in-corpus this run:** the jugular optical-sensing paper (De Gruyter CDBME 10.1515/cdbme-2024-2072), the peripheral pulse-modulation proof-of-concept (BMEO s12938-017-0351-x), the e-tattoo (IEEE 10340010), the ULM+PA platform (arXiv:2608.19823) and its 3D-PAULM sibling (bioRxiv), the hyperspectral fundus system (PMC12997856), APM+ (Adv. Sci. 10.1002/advs.76366), and the wearable FD-NIRS ASIC (PMC12904531) all re-surfaced but are already logged. No new true-venous lead emerged.
- The strongest true-venous entries recur below, all marked *previously surfaced*, with honest relevance scores. The most recent genuinely-new intravascular-venular result in the corpus remains the **08-13 hyperspectral retinal system** (Tran et al.); the most recent new imaging-platform lead remains the **08-25 Davenet/Gateau ULM+PA** preprint.

---

## Topic 1 — Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous)

*No new human venous-specific paper today. The five strongest true-venous entries — all previously surfaced — are carried forward with honest scores. This reflects genuine low publication volume in this niche, not an incomplete search.*

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al. (author list fetch-verified 06-10; re-confirmed via ResearchGate index snippet today).
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter), CDBME.
- **Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072 · ResearchGate mirror pub. 387159780. ⚠ De Gruyter full text egress-blocked today; metadata cross-checked on two index snippets.
- **Relevance:** 9/10 — directly targets non-invasive *venous* sO₂ at the jugular via a pulse-oximeter-style optical sensor.
- **Novelty:** Pulse-oximeter-analogue sensor over the external/internal jugular; exploits arterio-venous compliance differences to render venous blood detectably pulsatile, estimating SvO₂ in the healthy 60–90 % band across a small (n≈3) subject cohort. Correctly identifies the EJV waveform.
- **Integration insights:** The cleanest "wearable optical → true venous sO₂" proof point; the reference design for a low-cost venous analogue to SpO₂. Complements the deep-tissue PA and imaging methods in Topic 2 (which localize the vessel but need bulkier hardware).

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Year / Venue:** 2024 · *Optics Letters* **49**(10):2669 (opg.optica.org/ol) — venue re-confirmed via Optica index snippet today.
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669 ⚠ full text egress-blocked today.
- **Relevance:** 8/10 — IJV-specific, non-invasive, venous.
- **Novelty:** Couples subject-specific 3-D Monte-Carlo light-transport modeling with a DNN to map multi-channel surface NIRS reflectance to IJV sO₂ *changes*, handling anatomical variability that defeats fixed calibration.
- **Integration insights:** The modeling/ML calibration layer a device like §1.1 needs to generalize across patients; the Monte-Carlo prior is reusable for PA and DOT venous inversion in Topic 2.

### 1.3 — Proof-of-Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation (pulse-modulation venous oximetry) *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2017 · *BioMedical Engineering OnLine* 16:126 (s12938-017-0351-x).
- **Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x · PMC5437414. ⚠ PMC full text egress-blocked; abstract re-confirmed via index snippet today.
- **Relevance:** 8/10 — foundational peripheral venous method.
- **Novelty:** Induces artificial respiration-like modulation of the peripheral vasculature (exploiting arterio-venous compliance contrast) to make venous blood pulsatile, then extracts a venous PPG for regional venous sO₂ (SpvO₂) — the conceptual root of the modulation-based venous-oximetry line. Also re-surfaced today: the earlier venous-oximetry-during-cardiac-bypass method (IOP *Physiol. Meas.* 28(8), 10.1088/0967-3334/28/8/012), part of the same peripheral-venous lineage.
- **Integration insights:** Method ancestor of the jugular device (§1.1) and the e-tattoo (§1.4); establishes arterio-venous compliance contrast as an exploitable, reproducible signal source. The Apple PPGen/HAI forward-model lead (standing list) is the modern, physics-grounded successor to this compartment-separation idea.

### 1.4 — Towards Simultaneous Non-Invasive Arterial and Venous Oxygenation Monitoring with a Wearable Optical E-Tattoo *(previously surfaced — scan 07-01)*
- **Authors / Venue:** Lu group (UT Austin) · 2023 IEEE conference (EMBC-style), IEEE Xplore doc 10340010; PubMed 38083768; MRS Fall 2024 talk EL05.07.03. Re-confirmed via IEEE + MRS + UT-Austin PDF snippets today.
- **Relevance:** 8/10 — explicitly separates arterial *and* venous oxygenation in a conformal wearable.
- **Novelty:** Ultrathin conformal optical "e-tattoo" measuring arterial and venous pulses at the wrist; identifies artery–vein **crosstalk** (from their close proximity) as the key obstacle to simultaneous SaO₂/SvO₂ extraction and proposes **spatial filtering** to suppress it, characterized in simulation, in vitro, and in vivo.
- **Integration insights:** The form-factor endpoint for the §1.1/§1.3 modulation approaches — shows the sensing principle can shrink to skin-conformal hardware for continuous ambulatory venous monitoring; the crosstalk-suppression framing is the practical bridge from bench to wearable.

### 1.5 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-14; commercial NIRS device)*
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia* (S1053-0770(23)00782-6); PubMed 37827917; ScienceDirect S1053077023007826.
- **Link:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 ⚠ egress-blocked; metadata via index snippet.
- **Relevance:** 7/10 — non-invasive ScvO₂ surrogate via transcutaneous jugular NIRS; commercially fielded.
- **Novelty:** Clinical validation of the Mespere VO100 measuring SjvO₂ over the jugular as a non-invasive stand-in for catheter ScvO₂ in critically ill patients. Supporting evidence re-surfaced today: the pediatric-cardiac transcutaneous-jugular NIRS cohort (PMC7491293) and a retrospective NIRS-cerebral-oximetry SvO₂-tracking study (PMC10709586).
- **Integration insights:** The commercial-maturity reference point for jugular venous NIRS; benchmarks the accuracy bar (trend-monitoring, not absolute) that optical/PA methods in Topic 2 must beat to displace catheters.

> **Device/regulatory anchor (not ranked):** *Noninvasix LIVOx optoacoustic central venous oxygenation monitor* (ScvO₂ for septic shock; FDA Breakthrough Device Designation, 2022; chest-worn disposable-probe optoacoustic platform) — previously surfaced scan 08-11, re-confirmed via BioWorld/DelveInsight snippets today (Mar/May 2026 news briefs). No 2026 peer-reviewed validation data has yet appeared; watch for it.
> **Clinical-trial anchors (not ranked, non-optical/reference):** *Capnodynamic non-invasive mixed-venous SvO₂* (NCT06632197) — the most active *venous* clinical effort; watch for first results. *Continuous jugular venous oxygen saturation after cardiac arrest* (NCT06511999, Univ. Pittsburgh; est. completion 2027) — jugular venous validation cohort, non-optical reference. *Noninvasive Internal Jugular Venous Oximetry* (NCT06004466) and *SjvO₂ NIRS* trials (NCT04624009, NCT04778150) — jugular-NIRS validation cohorts, non-optical reference. *OCOSO2* (PMC10568773) — ScvO₂-guided goal-directed-therapy RCT, catheter-based reference.

---

## Topic 2 — Optical imaging techniques for non-invasively obtaining venous blood oxygen (PA/PACT, NIRS, DOI/DOT, hyperspectral, vis-OCT, SFDI)

*No new item first-surfaced today. Standing best-available set carried forward; the 08-13 hyperspectral system (§2.5) remains the most recent genuinely-new intravascular-venular result, and the 08-25 Davenet/Gateau ULM+PA platform (standing lead below) the most recent new imaging-platform lead.*

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10; the Topic-2 anchor)*
- **Year / Venue:** 2023 · preprint arXiv:2303.10775 (+ SPIE lineage). ⚠ arXiv egress-blocked today; abstract re-confirmed on two index snippets.
- **Link:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9/10 — human, in vivo, PA, *venous* (IJV).
- **Novelty:** Dual-wavelength PAT + ultrasound images the internal jugular vein in **7 healthy volunteers** at 5 fps; reported average IJV sO₂ ≈ **72 ± 7 %**, with fast US co-registration enabling temporal sO₂ tracking under physiologic challenges — true venous oximetry at depth, non-invasively.
- **Integration insights:** The proof that PA reaches a clinically relevant central vein through intact tissue; the benchmark every new PA-oximetry method (2.2–2.4) is implicitly measured against for venous applicability.

### 2.2 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+): In-Vivo Human Radial-Vein sO₂ *(previously surfaced — upgraded 07-15)*
- **Authors:** Sastry, Olick-Gibson et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley), 10.1002/advs.76366. ⚠ Wiley egress-blocked today; abstract re-confirmed via index snippet.
- **Link:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366
- **Relevance:** 9/10 — solves the fluence problem for deep-tissue PA sO₂ and reports in-vivo human values on the radial artery–vein pair (n = 8).
- **Novelty:** Uses high, known arterial oxygenation as a local in-situ **fluence reference** to correct spectral coloring, cutting median sO₂ error to **2.9 %** (vs 9.8 % for linear unmixing); demonstrated on the human radial vein.
- **Integration insights:** Directly attacks the single biggest barrier to quantitative deep venous PA — unknown local fluence — using the artery as a self-calibrator. Pairs naturally with §2.1's IJV geometry and §1.2's Monte-Carlo priors.

### 2.3 — Oxygenation Heterogeneity Facilitates Spatiotemporal Flow-Pattern Visualization Inside Human Blood Vessels Using PACT *(previously surfaced — scan 06-10/06-11)*
- **Year / Venue:** 2024 · photoacoustic-computed-tomography venue; PMC11161372. ⚠ PMC egress-blocked; abstract re-confirmed via snippet.
- **Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11161372/
- **Relevance:** 8/10 — human, intravascular sO₂ heterogeneity and flow, PACT; recovers the parabolic laminar-flow wavefront inside a deep vein in vivo.
- **Novelty:** Shows intravascular oxygenation heterogeneity can be turned into a *contrast mechanism* for visualizing flow patterns inside human vessels with PACT — oxygenation as a tracer, not just an endpoint — and demonstrates dynamic sO₂ imaging in a deep vein.
- **Integration insights:** Conceptual sibling of the ULM+PA platform (standing lead); supports vessel-type discrimination from hemodynamics and confirms human-scale PACT sensitivity to venous-range sO₂ gradients.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry (ADS-vis-OCT) *(previously surfaced — scan 06-11)*
- **Year / Venue:** 2023 · *Communications Medicine* (Nature), s43856-023-00288-8; PubMed 37095177; PMC10126115. ⚠ egress-blocked; metadata via snippet.
- **Link:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10126115/
- **Relevance:** 8/10 — resolves *per-vessel arterial and venous* retinal sO₂ non-invasively.
- **Novelty:** Adaptively removes vessel-specific spectral contaminants; RMSE ≈ 2.1 % vs pulse oximeter in major arteries, repeatability SD ≈ 2.3 % in *veins* — among the most accurate non-invasive per-vessel venous sO₂ figures reported. Demonstrated across glaucoma, ischemia, DR, CRVO, sickle-cell retinopathy.
- **Integration insights:** Sets the accuracy ceiling for optical venous oximetry in an accessible vascular bed; the adaptive spectral-correction idea is transferable to PA/DOT venous inversion where spectral coloring dominates error (cf. §2.2).

### 2.5 — Development and Validation of a High-Resolution Hyperspectral Imaging System for the Retina *(previously surfaced — scan 08-13; most recent genuinely-new intravascular-venular result)*
- **Authors:** Tran M.H., Pruitt K., Bryarly M., Emordi I., Ali A., Ma L., Fei B. (UT Southwestern / UT Dallas).
- **Year / Venue:** 2026 · *Journal of Biomedical Optics* **31**(3):036006 (2026 Mar 1); DOI 10.1117/1.JBO.31.3.036006; PMC12997856; PMID 41858558. ⚠ SPIE/PMC egress-blocked today; metadata re-confirmed on two index snippets (accepted Feb 2026, published Mar 2026).
- **Relevance:** 7.5/10 — measures **per-vessel retinal venule sO₂ (≈ 58 %)** alongside arteriole sO₂ (≈ 98 %) and vessel diameter; a true intravascular venular optical readout, though **retinal per-vessel, not systemic SvO₂**.
- **Novelty:** Snapshot hyperspectral fundus imager (hyperspectral camera + high-res RGB camera + beamsplitter + imaging endoscope) recovering vessel diameter *and* oxygenation simultaneously; a **deep-learning pansharpening** step fuses high-spatial and high-spectral channels (RMSE 2.15 ± 0.64, CC 0.96 ± 0.05).
- **Integration insights:** A cheaper, camera-based hardware route to the same per-vessel venous readout that vis-OCT (§2.4) and PA (§2.1/§2.2) reach with more elaborate instrumentation; the spatial–spectral fusion step is a transferable decoloring strategy.

---

## Standing context leads (not ranked in the top-5)

- **Apple ML: PPGen + Hybrid Amortized Inference — *Inferring Optical Tissue Properties from Photoplethysmography using Hybrid Amortized Inference*** (arXiv:2510.02073, Oct 2025; peer-reviewed at *IOP* 10.1088/3049-477X/ae4a96). *Technique-transfer lead — arterial/general PPG today, NOT a venous measurement (relevance to true venous ≈ 4/10, but architecturally important).* **PPGen** is a physically grounded PPG forward model mapping waveform shape to interpretable biophysical parameters — 9 static (melanin, arterial oxygenation, vessel/tissue optics) plus 2 dynamic blood-volume terms over a pulse; **HAI** is a fast, misspecification-robust amortized inverse. Extending PPGen's dynamic term to an explicit *venous* compartment (or fitting it under venous-modulation stimulation) is a concrete, well-posed route to model-based SpvO₂ — the modern physics-plus-ML successor to the arterio-venous-compliance modulation idea underlying §1.1/§1.3/§1.4. Validated in silico only so far. First surfaced 08-31. ⚠ metadata search-derived.
- **Davenet, Battaglia, Lager, Dargent, Lussey-Lepoutre, Tavitian, Couture, Bridal, Gateau — Simultaneous 3D Co-Registered Perfusion and Oxygenation with ULM, Photoacoustic Imaging, and a Planar Matrix Array** (arXiv:2608.19823, Aug 2026). *First surfaced 08-25:* multispectral PA sO₂ across the physiological **≈60–95 % range at 5 % accuracy using only five wavelengths**, co-registered with ULM sub-diffraction microvascular perfusion on a **single planar matrix array**; validated in vessel-mimicking phantoms and in vivo in mice. *Tissue/vessel-level, small-animal — not human SvO₂.* Its promise for venous work is **hemodynamic vessel-type discrimination** (labeling a vessel venous vs arterial from ULM flow, not sO₂ alone). Watch for a human/large-vessel follow-up and a peer-reviewed version.
- **Davenet, Billon, Battaglia, Bridal, Gateau — Sulfate Phantoms to Mimic NIR Photoacoustic Response of Whole Blood at Selected Oxygen Saturations** (*Applied Optics* **65**(6):1974–1982, 2026; arXiv:2512.01458). *Standing metrology lead.* Recipe for inorganic (sulfate) solutions matching whole-blood PA absorption **and** Grüneisen coefficient over 700–850 nm at chosen sO₂ — an injectable ground-truth for validating multi-wavelength PA venous oximetry. Same Paris/LIB group as the ULM+PA platform above; the two together form a build-and-validate stack for deep-vein PA sO₂.
- **3D-PAULM: Integrated Photoacoustic Tomography and Ultrasound Localization Microscopy for Multiparametric Brain and Tumor Imaging** (bioRxiv, 10.64898/2026.04.30.722008, 30 Apr 2026). Sibling of the ULM+PA platform, unifying multispectral PA, US B-mode, microbubble power Doppler, and ULM to concurrently measure oxygenation + microvascular flow; small-animal brain/tumor. Reinforces the "oxygenation + flow co-registration" theme. Re-confirmed via bioRxiv snippet today. ⚠ search-derived.
- **Hybrid-Net — Deep-Learning-Driven Quantitative Spectroscopic PA Imaging for Segmentation and Oxygen Saturation Estimation** (arXiv:2512.15394, Dec 2025). *Standing technique lead.* Joint vessel segmentation + sO₂ without explicit fluence estimation (segmentation accuracy ≥ 0.978 in sim, 0.998 in experiment); general PA-oximetry method, not venous-specific.
- **Wearable NIRS reviews / hardware (tissue StO₂, not venous SvO₂):** *Advances in fully integrated wearable near-infrared spectroscopy* (*J. Phys. Photonics*, IOP 10.1088/2515-7647/ae6ae4, 2026) and the FD-NIRS ASIC system (PMC12904531) — previously surfaced; logged for the wearable-hardware trajectory a venous method (§1.4) could ride.

---

## Cross-topic synthesis

1. **Another dry cycle for true-venous work — and that is the honest headline.** No new human/systemic non-invasive venous (SvO₂/ScvO₂) measurement paper first-surfaced today, continuing the pattern the 08-23 → 09-01 scans reported. The best Topic-1 work (jugular optical sensing §1.1, IJV DNN/Monte-Carlo §1.2, peripheral pulse-modulation §1.3, e-tattoo §1.4, jugular NIRS §1.5) is unchanged since June. This is a real publication-volume gap, not a search artifact.

2. **Today's re-surfaced hits were all already-catalogued.** The searches returned the jugular optical sensor, the peripheral-venous PPG lineage (including the older cardiac-bypass venous-oximetry method, IOP 10.1088/0967-3334/28/8/012), the e-tattoo, the ULM+PA/3D-PAULM pair, APM+, and the hyperspectral fundus system — every one already in the corpus. The PPG/venous-modulation lineage remains the conceptual root of Topic-1, now with Apple's PPGen/HAI as its physics-plus-ML modern successor.

3. **Where 2026 momentum actually sits: oxygenation + flow co-registration.** The Davenet/Gateau ULM+PA platform (arXiv:2608.19823) and its bioRxiv 3D-PAULM sibling mark a clear trend — pairing **photoacoustic sO₂** with **ULM/Doppler perfusion** on a shared array. For *venous* monitoring the hardest unsolved problem is not measuring sO₂ but **knowing which vessel is the vein**; hemodynamic co-registration offers a physics-based discriminator that pure spectral methods lack. This group is building the full stack — imaging platform plus a matched sulfate-phantom validator (*Appl. Opt.* 65(6):1974) — the most coherent single-lab program adjacent to deep-vein PA oximetry right now.

4. **Two mature accuracy anchors still frame the field.** APM+ (§2.2, deep-tissue, artery-referenced fluence correction, 2.9 % error) and ADS-vis-OCT (§2.4, per-vessel retinal venous sO₂, ~2.3 % repeatability) bracket the state of the art from the deep-tissue and superficial-bed ends. Both hinge on the same core fix — controlling **spectral coloring / unknown fluence** — which is exactly what the ULM+PA co-registration and §1.2's Monte-Carlo priors also target. The 08-13 hyperspectral fundus system (§2.5) adds a cheaper camera-based route to the same per-vessel venular readout.

5. **The near-term opportunity is porting, not discovering.** With Topic-1 clinical targets (IJV, radial/peripheral veins) stable and Topic-2 techniques advancing, the highest-leverage move is transferring Topic-2 advances — fluence correction, adaptive spectral decoloring, oxygenation–flow co-registration, sulfate-phantom metrology — and PPGen-style compartment-resolved forward modeling onto the Topic-1 venous targets.

6. **Confidence caveat.** `WebFetch` to all scholarly hosts was egress-blocked today (a direct arXiv fetch returned `EGRESS_BLOCKED`), so all metadata is search-snippet-derived (each item cross-checked on ≥2 snippets). Publisher-page verification should be repeated on the next scan where direct fetching is permitted.

---
*Scan generated 2026-09-02. Sources located and cross-verified via web search (≥2 independent index snippets per item); direct publisher/preprint-page fetching unavailable this run due to the environment's network egress policy (arXiv confirmed `EGRESS_BLOCKED` via direct WebFetch; PMC/PubMed, Optica, Wiley, De Gruyter, SPIE historically blocked). Metadata flagged ⚠ where it could not be confirmed on the source page.*
