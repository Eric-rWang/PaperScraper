# Daily Venous Oxygen Research Scan — 2026-07-26

**Scope:** (1) Non-invasive monitoring of venous blood oxygen (SvO₂ / ScvO₂ / peripheral venous oxygenation); (2) Optical imaging techniques for non-invasively obtaining venous blood oxygen (photoacoustic imaging/tomography, NIRS, diffuse optical imaging/tomography, hyperspectral imaging, visible-light OCT, spatial-frequency-domain imaging).

**Ranking basis:** relevance to **non-invasive, VENOUS** (not arterial) blood-oxygen measurement. Tissue-level oximetry (StO₂/VO₂) and arterial-only work are down-weighted and flagged; arterial techniques are included only where the method is directly transferable to the venous compartment.

**Honesty note on sparseness.** Genuinely novel *venous-specific* non-invasive optical work continues to be published at low volume. Yesterday's scan (07-25) surfaced **no** new primary venous demonstration. Today's sweep did turn up **four items not previously catalogued in this series**, though three are transferable-technique / adjacent-anatomy leads rather than direct deep-vein SvO₂ demonstrations, and one (the JBO superior-sagittal-sinus PA paper) is a strong new *venous-structure* demonstration. These are marked **★ NEW**. The standing venous anchors recur because nothing newer displaces them; they are marked *previously surfaced* with their prior scan reference.

**Verification note.** WebSearch results were used to confirm titles/authors/venues/DOIs. Direct `WebFetch` verification of arXiv, PubMed/PMC, and IOPscience pages returned HTTP 403 (site-side bot blocks, not a proxy fault), so metadata below is corroborated across multiple independent search-result snippets rather than a single fetched page. Items where a field could not be independently cross-checked are flagged **[metadata unverified]**.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / peripheral venous)

### 1.1 — Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins *(previously surfaced — scan 06-10 §1.1; flagship optical-venous device paper)*
- **Authors:** Alqahtani et al.
- **Year / Venue:** 2024 · *Current Directions in Biomedical Engineering* (De Gruyter), CDBME 2024-2072
- **Link / DOI:** https://www.degruyterbrill.com/document/doi/10.1515/cdbme-2024-2072/html · DOI 10.1515/cdbme-2024-2072
- **Relevance:** 9/10
- **Novelty:** Pulse-oximeter-style optical sensor placed over the external jugular vein (EJV); resolves the venous pulse waveform and returns SvO₂ estimates of 71.1 / 72.2 / 70.4 % on three subjects — squarely in the healthy 60–90 % range.
- **Integration insights:** The clearest "wearable pulse-oximeter-for-veins" concept in the corpus. Its limitation — three subjects, no blood-gas gold-standard calibration — is exactly the gap the deeper-tissue PA and MRI-model threads aim to close. Remains the reference point against which new venous-optical devices should be benchmarked.

### 1.2 — Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific 3-D Monte-Carlo Models *(previously surfaced — scan 06-10 §1.2)*
- **Authors:** (IJV DNN + Monte-Carlo group)
- **Year / Venue:** 2024 · *Optics Letters* 49(10):2669
- **Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669
- **Relevance:** 8/10
- **Novelty:** Couples subject-specific 3-D Monte-Carlo light-transport models with a DNN to convert surface optical signal into IJV oxygen-saturation *change*, personalising the forward model per anatomy.
- **Integration insights:** Directly addresses the field's central obstacle — unknown, depth- and wavelength-dependent fluence — via learned inversion over an anatomy-specific forward model. The subject-specific-model idea is portable to PA and diffuse-optics venous pipelines.

### 1.3 — A New Non-Invasive Method for the Assessment of Central Venous Oxygen Saturation (Mespere VO100 jugular NIRS) *(previously surfaced — scan 06-10 §1.3)*
- **Authors:** (critical-care evaluation group)
- **Year / Venue:** 2023 · *Journal of Cardiothoracic and Vascular Anesthesia*, S1053-0770(23)00782-6
- **Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826 · PubMed 37827917
- **Relevance:** 8/10
- **Novelty:** Clinical evaluation of a transcutaneous jugular-NIRS device (Mespere VO100) as a continuous non-invasive surrogate for catheter-measured ScvO₂ in critically ill patients.
- **Integration insights:** The most clinically mature commercial embodiment of jugular-NIRS venous oximetry; a real-world reference for what accuracy/robustness a bedside venous device must reach. Anchors the "does NIRS-over-jugular track ScvO₂?" validation question that several 2023–24 trials (NCT04624009, NCT04778150) also probe.

### 1.4 — ★ NEW — Transabdominal Fetal Oximetry via Diffuse Optics: Principled Analysis and Demonstration in Pregnant Ovine Models *(newly catalogued this cycle — diffuse-optics technique that explicitly models the venous compartment; target output is fetal SpO₂, not deep-vein SvO₂)*
- **Authors:** Weitai Qian, Rishad Raiyan Joarder, Soheil Ghiasi, et al. (UC Davis)
- **Year / Venue:** 2025 (posted 25 Sep 2025) · arXiv preprint (also TechRxiv; indexed PubMed 41040802 / PMC12486049) **[venue = preprint; peer-reviewed home unverified]**
- **Link / DOI:** https://arxiv.org/abs/2509.21594 · https://pmc.ncbi.nlm.nih.gov/articles/PMC12486049/
- **Relevance:** 6/10 *(venous relevance is indirect: arterial-target measurement whose forward model accounts for the venous compartment)*
- **Novelty:** Full theoretical pipeline for estimating fetal SpO₂ from transabdominal diffuse-light (PPG) intensity through thick maternal tissue; introduces the **Exponential Pulsation Ratio (EPR)** feature and a multi-detector ML fusion model. Reports MAE 4.81 % (simulation) / 6.85 % (in-vivo ovine), Pearson r = 0.81 / 0.71. The forward model explicitly encodes venous blood at ~75 % lower saturation than arterial.
- **Integration insights:** Relevant to venous monitoring in two ways: (a) it is a rigorous demonstration that deep-tissue diffuse-optics oximetry through many centimetres of overlying tissue is tractable — the same depth barrier that a deep-vein SvO₂ device must beat; and (b) its explicit arterial/venous compartment separation and pulsation-ratio feature are directly transferable to the problem of isolating the *venous* pulsatile signal. A candidate methodological building block, not a venous demonstration.

### 1.5 — ★ NEW — Multi-Layer Self-Calibrated Algorithm for Transabdominal Fetal Pulse Oximetry: Simulation and In-Vivo Validation *(newly catalogued this cycle — layer-resolved diffuse-optics inversion; transferable, not venous-specific)*
- **Authors:** Jingyi Wu et al. (Carnegie Mellon University, MIT, collaborators)
- **Year / Venue:** 2025 (published 11 Nov 2025) · *Journal of Physics: Photonics* 8(1), Focus Issue on Photonics in Medical Diagnostics and Monitoring
- **Link / DOI:** https://iopscience.iop.org/article/10.1088/2515-7647/ae1a27 · DOI 10.1088/2515-7647/ae1a27 · https://pmc.ncbi.nlm.nih.gov/articles/PMC12603613/
- **Relevance:** 5/10 *(fetal arterial target; value is the layer-resolved self-calibration method)*
- **Novelty:** First **layer-resolved, self-calibrated** algorithm for transabdominal fetal pulse oximetry, validated with Monte-Carlo photon simulation and an in-vivo sheep experiment; tracks fetal SpO₂ dynamics without external calibration.
- **Integration insights:** Self-calibration and explicit multi-layer modelling are precisely the levers a non-invasive deep-vein device needs to remove unknown overlying-tissue contributions. The "layer-resolved, calibration-free" framing complements §1.2's subject-specific Monte-Carlo approach and §1.4's EPR feature — three independent 2025 attacks on the same fluence/geometry problem.

*(Standing non-optical venous references intentionally held below the top 5 this cycle: the McDiarmid noninvasive mixed-SvO₂ heart-failure model (imaging-derived iSvO₂, scan 07-07 §1.1) and the self-supervised intra-cardiac MR-oximetry preprint (scan 07-13 §1.1). Both remain relevant as validation/ground-truth analogues but are MRI-based, not optical.)*

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

### 2.1 — Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans *(previously surfaced — scan 06-10 §2.1; the Topic-2 anchor)*
- **Authors:** (IJV photoacoustic group)
- **Year / Venue:** 2023 · arXiv:2303.10775
- **Link / DOI:** https://arxiv.org/abs/2303.10775
- **Relevance:** 9/10
- **Novelty:** Dual-wavelength photoacoustic tomography + ultrasound imaged the IJV in seven healthy volunteers, yielding an average venous saturation of 72 ± 7 % — a true, deep-vein, human, non-invasive SvO₂ measurement by optics.
- **Integration insights:** Still the strongest single proof that spectroscopic PA can quantify a named deep vein in humans. The benchmark every new PA-venous method (including today's §2.2) is measured against.

### 2.2 — ★ NEW — Automatic Photoacoustic Monitoring of Perinatal Brain Hypoxia with Superior Sagittal Sinus Detection *(newly catalogued this cycle — venous-structure PA oximetry; strongest genuinely new venous item this scan)*
- **Authors:** Baichuan Jiang, Ernest Graham, Mathias Unberath, Russell H. Taylor, Raymond C. Koehler, Jeeun Kang, Emad M. Boctor (Johns Hopkins)
- **Year / Venue:** 2025 (published 11 Jul 2025) · *Journal of Biomedical Optics* 30(7):076004
- **Link / DOI:** https://doi.org/10.1117/1.JBO.30.7.076004 · https://pmc.ncbi.nlm.nih.gov/articles/PMC12245645/
- **Relevance:** 8/10 *(measures a venous sinus, not arterial; neonatal-piglet model rather than human)*
- **Novelty:** Validates **transcranial** photoacoustic imaging of oxyhemoglobin saturation at the **superior sagittal sinus** — a cerebral *venous* sinus — in the neonatal piglet brain, and automates the PA workflow (vessel detection + probe guidance) toward fully autonomous continuous perinatal monitoring.
- **Integration insights:** Directly on-topic: the superior sagittal sinus, like the internal jugular vein, is a cerebral venous compartment whose saturation reflects brain O₂ extraction. This is a second independent venous-structure PA target beyond the IJV (§2.1) and adds the missing operational piece — **automated vessel detection/segmentation for hands-free continuous monitoring** — that the IJV work and the jugular-optical device (§1.1) still require an operator for. Transcranial venous PA + automation is a plausible template for an unattended bedside deep-vein SvO₂ monitor.

### 2.3 — Arterial Blood-Mediated Deep-Tissue Photoacoustic Oximetry (APM+) *(previously surfaced — upgraded 07-15 §2.2; in-vivo human radial-vein sO₂)*
- **Authors:** Sastry et al.
- **Year / Venue:** 2026 · *Advanced Science* (Wiley)
- **Link / DOI:** https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.76366 · DOI 10.1002/advs.76366
- **Relevance:** 8/10
- **Novelty:** Uses arterial blood as an internal optical reference to correct for unknown local fluence, enabling absolute deep-tissue PA oximetry — demonstrated in vivo including human radial-vein sO₂.
- **Integration insights:** Its internal-reference calibration is one of the most promising answers to the absolute-quantification problem, and it explicitly reaches a peripheral vein in humans. Complementary to §2.2's automation and §2.1's IJV target; a strong candidate to *stack* with layer-resolved inversion (§1.5) for a calibrated venous system.

### 2.4 — Adaptive Spectroscopic Visible-Light OCT for Clinical Retinal Oximetry *(previously surfaced — scan 06-11 §2.2)*
- **Authors:** (vis-OCT retinal-oximetry group)
- **Year / Venue:** 2023 · *Communications Medicine* 3, 88
- **Link / DOI:** https://www.nature.com/articles/s43856-023-00288-8 · PMC10126115
- **Relevance:** 7/10 *(retinal vein saturation — true venous, but a specialised vascular bed)*
- **Novelty:** Adaptively removes vessel-specific spectral contaminants so vis-OCT measures oxygen saturation accurately per vessel; ex-vivo phantom agreement within 1 % bias against a blood-gas machine across 0–100 % sO₂. Reported retinal venous sO₂ ≈ 48 % vs arterial ≈ 92 %.
- **Integration insights:** Highest-accuracy optical venous-saturation demonstration in the corpus, and it explicitly resolves arterial vs venous vessels — but confined to the transparent optical path of the retina. The per-vessel spectral-contaminant correction is conceptually transferable to deep-tissue spectroscopic PA, where analogous spectral coloring corrupts sO₂ estimates.

### 2.5 — ★ NEW — Towards Robust Quantitative Photoacoustic Tomography via Learned Iterative Methods *(newly catalogued this cycle — qPAT inversion technique; transferable, not venous-specific)*
- **Authors:** Anssi Manninen et al. **[full author list unverified]**
- **Year / Venue:** 2025 (posted Oct 2025) · arXiv:2510.27487 **[venue = preprint]**
- **Link / DOI:** https://arxiv.org/abs/2510.27487 · https://arxiv.org/html/2510.27487
- **Relevance:** 6/10 *(general qPAT / absorption-and-sO₂ recovery method; no venous demonstration)*
- **Novelty:** Learned iterative reconstruction for **quantitative** photoacoustic tomography that stays robust with **limited training data**, recovering absorption (and hence sO₂) more reliably than end-to-end networks under data scarcity.
- **Integration insights:** Absolute sO₂ from PA hinges on quantitative recovery of the optical absorption coefficient under unknown fluence — the exact target here. Robustness under limited training data matters because venous-specific in-vivo ground-truth datasets are scarce (see the sparseness note). A methodological complement to the Hybrid-Net fluence-free approach (standing lead, arXiv:2512.15394) and APM+'s internal-reference calibration (§2.3).

*(Standing Topic-2 references held below the top 5: the PACT venous-flow / oxygenation-heterogeneity paper (scan 06-11), the sulfate blood-phantom metrology paper (scan 07-07 §2.2), the APRECOT MSOT anatomical-prior preprint and the DPF diffuse-optics model (scan 07-17 §2.4–2.5), and the retinal hyperspectral-imaging system (scan 07-07 §2.3). No new versions today.)*

---

## Cross-Topic Synthesis

**1. Today's signal: venous-specific optical work is still thin, but the venous *anatomy* list is quietly growing.** For months the only named deep-vein human optical measurement was the internal jugular vein (§2.1) plus the peripheral radial vein (§2.3). Today adds a genuinely new venous *structure* — the **superior sagittal sinus**, measured transcranially by photoacoustics in a neonatal model (§2.2). Cerebral venous compartments (IJV, sagittal sinus) are emerging as the most tractable optical-venous targets because their saturation carries clinically prized information (brain O₂ extraction) and they sit at accessible depths.

**2. The central obstacle is unchanged — absolute quantification under unknown, depth- and wavelength-dependent fluence — and every live thread attacks it from a different side.** Internal-reference calibration (APM+ §2.3); subject-specific Monte-Carlo forward models with learned inversion (§1.2); layer-resolved self-calibration (§1.5, ★new); fluence-free deep learning (Hybrid-Net, standing); robust quantitative inversion under scarce data (§2.5, ★new); and per-vessel spectral-contaminant removal (§2.4). No single paper solves it; a clinically accurate deep-vein SvO₂ system will most likely **stack** several — e.g. APM+ internal-reference calibration + layer-resolved inversion + robust learned qPAT.

**3. The new fetal diffuse-optics pair (§1.4, §1.5) is a useful "adjacent hard problem."** Transabdominal fetal oximetry has to recover blood oxygenation through many centimetres of overlying maternal tissue and to separate arterial from venous contributions — the same two difficulties (depth, compartment isolation) a non-invasive deep-vein SvO₂ device faces. Its tools (Exponential Pulsation Ratio; multi-layer self-calibration) are portable even though the clinical target is arterial.

**4. Automation is the newly visible frontier.** Beyond *can* optics read a vein, §2.2 asks *can it do so unattended* — automated sagittal-sinus detection and probe guidance for continuous monitoring. Coupling automated venous-vessel detection with a calibrated quantitative-PA or diffuse-optics inversion is the plausible path from today's operator-dependent proofs-of-concept (§1.1, §2.1) to a real bedside venous monitor.

**5. Honest bottom line.** No new *primary human deep-vein SvO₂* demonstration appeared today. The four ★NEW items are one strong venous-structure animal demonstration (§2.2) and three transferable technique/adjacent-anatomy leads (§1.4, §1.5, §2.5). The core human venous anchors (§1.1, §1.2, §1.3, §2.1, §2.3, §2.4) recur because nothing newer displaces them.
