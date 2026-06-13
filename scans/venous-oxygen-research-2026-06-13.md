# Venous Oxygen Research Scan — 2026-06-13

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.
**Prior scans in this repository:** 2026-06-10 and 2026-06-11. All 20 papers entered in those two scans are excluded from re-selection here unless a genuinely newer version or finding warrants it (none did this run). The landmark venous-PA and IJV-NIRS papers (Garcia-Uribe 2023, Sun 2024, Kong 2024, Zhang PAVT 2024, Jeleff 2023, McDiarmid CMR 2026, Lahade FD-NIRS 2026, Liu TD-HSI 2025, Feng PA-thrombosis 2025, Wu vis-OCT review 2025, etc.) remain the strongest works in the field but are *not* repeated — see prior files.
**Search window emphasis:** New or not-previously-surfaced work, with priority on 2025–2026. Sources searched this run: PubMed/PMC, arXiv, Optica (BOE, Optics Letters), SPIE (incl. Neurophotonics, JBO), Frontiers, MDPI, De Gruyter, IEEE Xplore, Springer, ScienceDirect, Taylor & Francis, AAAS, American Diabetes Association.

**Honest note on sparseness (important):** Genuinely *venous-specific* non-invasive optical oximetry is a low-volume niche, and the strongest entries were already captured in the two prior scans. To avoid re-surfacing those, this scan reaches into (a) adjacent venous-monitoring methods that are non-optical or PPG-based, (b) recent reviews, and (c) optical-imaging papers whose technique is directly transferable to venous oxygenation even when demonstrated on tissue or retina. Relevance scores are deflated accordingly and the tissue-vs-true-SvO₂ distinction is flagged per entry. Several Topic-1 entries cluster around one research group (Canterbury PPG line) and one analytics platform — this reflects the real shape of the literature, not padding.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### Paper 1.1
**Title:** Investigation of a Novel Noninvasive Risk Analytics Algorithm With Laboratory Central Venous Oxygen Saturation Measurements in Critically Ill Pediatric Patients
**Authors:** Sarah A. Teele, Avihu Z. Gazit, Craig Futterman, William G. La Cava, David S. Cooper, Steven M. Schwartz, Joshua W. Salvin
**Year:** 2025 (published online January 16, 2025)
**Venue:** *Critical Care Explorations*, 7(1):e1204
**Link / DOI:** https://doi.org/10.1097/CCE.0000000000001204
**Metadata verified:** Title, full author list, journal, DOI, and PMC ID (PMC11741213) confirmed via PMC, the George Washington University Himmelfarb repository, and an author-hosted PDF (cavalab.org). Volume/issue/article number cross-checked.
**Relevance score:** 7 / 10
⚠️ *Not an optical method — this is a parameter-derived analytics index (IDo₂); included because Topic 1 covers non-invasive venous-oxygen monitoring broadly. Estimates probability of low ScvO₂ rather than measuring it directly.*

**Novelty:** Validates the "inadequate delivery of oxygen" (IDo₂) index — a continuously computed probability that a patient's ScvO₂ has fallen below a preset threshold — against **20,424 laboratory ScvO₂ measurements from 3,018 critically ill neonates, infants, and children**. This is, by sheer measurement count, one of the largest datasets ever assembled linking a non-invasive continuous index to gold-standard venous co-oximetry. The algorithm fuses routinely monitored vitals/waveforms into a single venous-adequacy risk score without any blood draw.

**Integration insights:** The IDo₂ work defines the *clinical decision target* that an optical venous oximeter must ultimately beat or complement: a continuously available, blood-draw-free estimate of whether ScvO₂ is adequate. Its enormous labeled dataset is exactly the kind of ground-truth corpus needed to train and benchmark optical (NIRS/PA) venous estimators — an optical front-end feeding measured SvO₂ into an IDo-style risk layer would convert a probabilistic surrogate into a measured one. It also reinforces the recurring theme from prior scans (McDiarmid CMR, Jeleff Mespere) that the venous-oxygen field is being pulled forward by critical-care and cardiac populations where invasive ScvO₂/SvO₂ is already the reference standard.

---

### Paper 1.2
**Title:** The Role of Continuous Monitoring of Venous Drainage Flow and Integrated Oxygen Extraction (ERiO₂) via Bilateral Near-Infrared Spectroscopy in Cerebral Perfusion During Aortic Arch Surgery
**Authors:** Ignazio Condello, Giuseppe Speziale, Flavio Fiore, Giuseppe Nasso
**Year:** 2025 (published January 27, 2025)
**Venue:** *Medicina* (MDPI), 61(2):226
**Link / DOI:** https://doi.org/10.3390/medicina61020226
**Metadata verified:** Title, full authors, journal, volume/issue/article number, and PMC ID (PMC11857250) confirmed via MDPI and PMC. DOI follows the standard MDPI article-ID pattern (medicina61020226), consistent with the verified volume/issue/article number.
**Relevance score:** 6 / 10
⚠️ *Tissue-level rSO₂ combined with a venous-drainage oxygen-extraction metric; small cohort (n = 10). Venous compartment is explicitly targeted via the venous-line oxygen-extraction ratio.*

**Novelty:** Introduces **ERiO₂ — an integrated oxygen-extraction ratio computed from continuously monitored venous drainage flow** (via the cardiopulmonary-bypass venous line and the "Landing" perfusion-monitoring system) paired with bilateral cerebral NIRS (Masimo). During aortic-arch surgery with the Kazui selective-cerebral-perfusion technique, the method links measured venous return to regional cerebral oxygenation in real time, yielding a continuous extraction signal rather than a static saturation snapshot.

**Integration insights:** This is one of the few recent papers that treats the *venous side of the circuit as the primary signal* rather than an afterthought. The oxygen-extraction framing (arterial supply − venous return) is precisely the quantity that tissue-level optical methods approximate when they report StO₂; ERiO₂ gives a measured analogue against which optical OEF estimates could be calibrated intra-operatively. For optical venous oximetry, the conceptual takeaway is that **extraction ratio, not absolute SvO₂ alone, may be the more robust and clinically actionable optical endpoint** — a NIRS/PA system that outputs OEF sidesteps some absolute-calibration burden while preserving clinical meaning.

---

### Paper 1.3
**Title:** Development of an Electro-Pneumatic Calf Muscle Actuator to Estimate Peripheral Venous Oxygen Saturation Using Photoplethysmography
**Authors:** University of Canterbury group (J. F. Hill / C. G. Pretty / J. G. Chase line; full author list not independently confirmed — *flagged*)
**Year:** 2024
**Venue:** *Proc. IEEE Engineering in Medicine & Biology Society (EMBC) 2024* — IEEE Xplore document 10782659
**Link / DOI:** https://ieeexplore.ieee.org/document/10782659/
**Metadata verified:** Title, year, and IEEE Xplore document ID confirmed via IEEE and ResearchGate listings. Exact author list, page numbers, and DOI **not** independently verified — *flagged.* Attribution to the Canterbury PPG group inferred from the directly continuous line of work (cdbme-2023-1037; Hill 2024 jugular paper in prior scan).
**Relevance score:** 6 / 10
*(Directly venous-specific PPG method; peripheral venous SvO₂; engineering proof-of-concept.)*

**Novelty:** Builds an **electro-pneumatic calf-muscle actuator** that mechanically drives reproducible venous-blood-volume modulations (an instrumented venous muscle-pump test), making the otherwise non-pulsatile venous bed pulsatile so that a PPG sensor can extract a venous-specific AC signal and estimate peripheral venous oxygen saturation. This is the hardware-engineering successor to the group's 2023 functional-electrical-stimulation proof-of-concept (Paper 1.5), replacing involuntary muscle stimulation with a controllable pneumatic actuator for repeatability.

**Integration insights:** The core problem in optical venous oximetry is that veins lack the intrinsic pulsation that lets pulse oximetry isolate arterial blood. This line of work solves that by *inducing* a controlled venous modulation — a strategy directly portable to the jugular reflectance geometry (Hill 2024, prior scan) and combinable with NIRS or hyperspectral readouts instead of single-wavelength PPG. An actuator-driven venous modulation could likewise gate a photoacoustic or SFDI acquisition to a known venous-volume phase, improving venous-specificity of any optical modality. This is among the most *mechanistically venous-specific* approaches in the entire scan.

---

### Paper 1.4
**Title:** Editorial: Diffusive Optics for Medical Imaging
**Authors:** Bruno Urban, António M. Morgado
**Year:** 2026 (published April 30, 2026)
**Venue:** *Frontiers in Photonics*, vol. 7, article 1842429 (Biophotonics section)
**Link / DOI:** https://doi.org/10.3389/fphot.2026.1842429
**Metadata verified:** Title, journal, volume, article number, and publication date confirmed via Frontiers listing and search cross-check. Author given names abbreviated from the editorial byline (Urban B., Morgado A. M.) — full given names inferred; *flagged.* Direct page fetch returned HTTP 403; metadata cross-checked across two independent search responses.
**Relevance score:** 5 / 10
*(Editorial/overview, not primary data; explicitly frames pulsatile diffuse-optics decomposition into SaO₂ / SvO₂ / OEF — directly on-topic conceptually.)*

**Novelty:** A 2026 editorial framing the current state of diffusive optics for medicine (diffuse optical tomography, spatial-frequency-domain imaging, time-domain diffuse optical spectroscopy, diffuse correlation spectroscopy). Its venous relevance is the explicit articulation that **resolving the pulsatile component of the diffuse-optical signal enables decomposition into arterial (SaO₂), venous (SvO₂), and oxygen-extraction-fraction (OEF) terms**, rather than reporting only a blended StO₂.

**Integration insights:** This editorial is useful primarily as a *map of the modality landscape* and as confirmation that the venous-decomposition idea (pulsatile gating → SvO₂/OEF) is now mainstream within the diffuse-optics community, not a fringe ambition. It situates the wearable FD-NIRS hardware (Lahade 2026, prior scan) and SFDI work (Huang SFDI-net, El Masry, prior scans) within a single methodological family, and it reinforces the Topic-1 theme that **OEF is emerging as the practical venous-oxygen endpoint for diffuse optics**. Treated as context, not as a primary finding — hence the modest score.

---

### Paper 1.5
**Title:** Muscle Stimulation for Peripheral Venous Oxygen Saturation Estimation Using Photoplethysmography: A Proof-of-Concept
**Authors:** University of Canterbury group (Pretty / Chase line; full author list not independently confirmed — *flagged*)
**Year:** 2023 (published September 20, 2023)
**Venue:** *Current Directions in Biomedical Engineering*, 9(1) (De Gruyter)
**Link / DOI:** https://doi.org/10.1515/cdbme-2023-1037
**Metadata verified:** Title, journal, year, and DOI confirmed via De Gruyter and ResearchGate. Full author list not independently verified — *flagged.* Not previously surfaced in this repository.
**Relevance score:** 5 / 10
*(Venous-specific PPG; small n = 3 proof-of-concept; predecessor to Paper 1.3. Older but not previously catalogued.)*

**Novelty:** Uses **functional electrical stimulation (FES)** of the calf muscle to generate rhythmic, reproducible contractions that pump venous blood and create a measurable venous PPG modulation, from which peripheral venous saturation is estimated. Demonstrated in three healthy young males. This is the conceptual seed of the 2024 actuator paper (Paper 1.3) and is part of the same coherent Canterbury research programme that produced the jugular reflectance sensor (Hill 2024, prior scan Paper 1.1).

**Integration insights:** Included to document the *origin and trajectory* of the induced-venous-modulation approach: FES (2023) → controllable electro-pneumatic actuator (2024) → jugular reflectance sensing. The shared principle — deliberately make the venous bed pulsatile so an optical sensor can isolate it — is the most transferable idea across the two topics, and a candidate front-end for combining with NIRS, hyperspectral, or photoacoustic detection to achieve venous specificity without occlusion cuffs. Honestly scored low for age and tiny cohort, but methodologically central.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

### Paper 2.1
**Title:** Imaging of the Retinal Hypoxia: A Journey from Oxygen Microelectrode to the First Hypoxia Imaging in the Living Retina
**Authors:** Md Imam Uddin (Uddin Laboratory for Ocular Imaging, Vanderbilt University)
**Year:** 2025 (published October 2025)
**Venue:** *Progress in Retinal and Eye Research*, article 101411
**Link / DOI:** https://doi.org/10.1016/j.preteyeres.2025.101411
**Metadata verified:** Title, author, journal, year, and DOI confirmed via ScienceDirect, the Vanderbilt Uddin Lab publications page, and PubMed cross-check. Single-author attribution per the lab listing; co-authors (if any) not confirmed — *flagged.* Direct ScienceDirect fetch returned HTTP 403; metadata cross-checked across multiple search responses.
**Relevance score:** 7 / 10
*(Review; retinal venous oximetry covered in depth alongside emerging photoacoustic and molecular hypoxia imaging. Retinal veins are the one human site where true vessel-specific venous sO₂ is routinely imaged non-invasively.)*

**Novelty:** Comprehensive 2025 review tracing retinal-oxygen measurement from invasive oxygen-sensitive microelectrodes (Linsenmeier) to modern non-invasive *in vivo* hypoxia imaging. Consolidates the technique families relevant to venous oxygenation — spectroscopic retinal oximetry, visible-light OCT, phosphorescence-lifetime imaging, and photoacoustic ophthalmoscopy — and frames retinal venular saturation/oxygen-extraction as a disease biomarker.

**Integration insights:** The retina remains the proving ground for vessel-specific optical venous oximetry, and this review is the most current synthesis of the methods that work there. It directly informs the translational question posed in prior scans (vis-OCT review, 2026-06-11 Paper 2.5): which retinal venous-oximetry techniques can migrate to accessible peripheral veins (external jugular, basilic, cephalic). It also explicitly couples spectroscopic oximetry with photoacoustic and phosphorescence approaches — exactly the multimodal direction Paper 2.2 instantiates — making it the connective-tissue reference for Topic 2 this scan.

---

### Paper 2.2
**Title:** Multimodal Retinal Imaging by Visible-Light Optical Coherence Tomography and Phosphorescence Lifetime Ophthalmoscopy in the Mouse Eye
**Authors:** Stephanie Nolen, Zhongqiang Li, Jingyu Wang, Mirna El Khatib, Sergei A. Vinogradov, Ji Yi
**Year:** 2025 (published September 27, 2025)
**Venue:** *Neurophotonics* (SPIE), 12(3):035015
**Link / DOI:** https://doi.org/10.1117/1.NPh.12.3.035015
**Metadata verified:** Title, full author list, journal, volume/issue/article number, publication date, and DOI confirmed via SPIE Digital Library, PMC (PMC12476265), and PubMed (PMID 41019609); preprint at bioRxiv 2025.05.29.656845. Affiliations: Johns Hopkins University and University of Pennsylvania.
**Relevance score:** 7 / 10
*(Vessel-resolved venous sO₂ via vis-OCT plus intravascular pO₂ via PLIM; murine, requires injected phosphorescent probe for the pO₂ channel. The vis-OCT channel is fully endogenous and venous-resolving.)*

**Novelty:** Combines **visible-light OCT (endogenous spectroscopic sO₂, vessel-resolved) with phosphorescence-lifetime ophthalmoscopy (PLIM-SLO) for intravascular and capillary pO₂** in a single co-registered platform, using the Oxyphor 2P probe for the PLIM channel. This cross-validates two independent optical oxygen readouts — saturation (vis-OCT) and partial pressure (PLIM) — in the same retinal vessels, including veins, and enables computation of oxygen extraction and metabolic rate.

**Integration insights:** The pairing answers a central credibility problem for optical venous oximetry: vis-OCT spectroscopic sO₂ has historically lacked an independent in-vivo gold standard at the single-vessel level. By co-registering it with phosphorescence pO₂, this work provides exactly that cross-modal validation — a template for validating *any* new optical venous-oximetry method against an orthogonal optical reference rather than against a blood draw. While the PLIM channel needs an exogenous probe (limiting direct human venous translation), the vis-OCT channel is label-free and directly venous-resolving, and the dual-readout OEF/metabolic-rate framing aligns with the Topic-1 ERiO₂/OEF theme (Paper 1.2).

---

### Paper 2.3
**Title:** Machine Learning Enabled Multiple Illumination Quantitative Optoacoustic Oximetry Imaging in Humans
**Authors:** Thomas Kirchner, Michael Jaeger, Martin Frenz
**Year:** 2022 (published online April 5, 2022)
**Venue:** *Biomedical Optics Express*, 13(5):2655–2667
**Link / DOI:** https://doi.org/10.1364/BOE.455514
**Metadata verified:** Title, full authors, journal, volume/issue/pages, year, and DOI confirmed via PMC (PMC9203099), PubMed (PMID 35774340), and arXiv (2202.01482). Affiliation: University of Bern.
**Relevance score:** 6 / 10
⚠️ *2022 paper — older, and not venous-specific (images forearm vessels including arteries and veins); included because it is not previously surfaced and the multiple-illumination "learned spectral decoloring" approach is directly transferable to venous sO₂. Tissue/vessel-level, in humans.*

**Novelty:** Tackles the dominant accuracy barrier for quantitative optoacoustic oximetry — unknown local fluence ("spectral coloring") — by acquiring the **same tissue under multiple illumination geometries** and training a machine-learning model (learned spectral decoloring) to invert toward true sO₂. Demonstrated *in humans*, in vivo, on forearm vasculature, recovering quantitative blood oxygenation without an explicit fluence model.

**Integration insights:** This is methodologically upstream of the deep-learning PA-inversion papers already catalogued (Hybrid-Net, SPOI-AE, qPACT-virtual in prior scans): multiple-illumination decoloring is a *hardware-side* complement to those *algorithm-side* fluence solutions, and the two can be combined. Because it is validated in human limbs — where superficial veins are imaged alongside arteries — it is a concrete demonstration that quantitative optoacoustic venous sO₂ is attainable in humans once vessel segmentation (cf. Hybrid-Net) localises the venous pixels. Its placement of the fluence problem at the acquisition stage is a useful counterpoint to purely post-hoc network corrections.

---

### Paper 2.4
**Title:** Surgical Hyperspectral Imaging: A Systematic Review
**Authors:** Hafsa Moontari Ali, Yiming Xiao, Marta Kersten-Oertel
**Year:** 2025 (published December 2025)
**Venue:** *Computer Assisted Surgery*, 30(1):2546819 (Taylor & Francis)
**Link / DOI:** https://doi.org/10.1080/24699322.2025.2546819
**Metadata verified:** Title, full authors, journal, volume/issue/article number, year, and PubMed ID (40824764) confirmed via Taylor & Francis and PubMed. Affiliation: Concordia University, Montréal.
**Relevance score:** 5 / 10
*(Review; tissue-level perfusion/oxygenation mapping, not vessel-specific venous sO₂. HSI is a named in-scope modality; venous oxygenation appears as a perfusion-monitoring sub-application.)*

**Novelty:** PRISMA systematic review of 85 surgical hyperspectral-imaging studies, cataloguing hardware/scanning mechanisms, preprocessing and analysis pipelines (classification, segmentation, tissue characterisation, perfusion analysis), and clinical feasibility. Identifies **intraoperative perfusion and oxygenation mapping** — generating tissue oxygenation/perfusion maps to detect ischemia and post-operative complications — as a maturing HSI application alongside tumour-resection guidance.

**Integration insights:** Establishes the current performance envelope and processing-pipeline conventions for clinical HSI oxygenation mapping, the wide-field complement to the single-vessel transmissive HSI work surfaced in the 2026-06-11 scan (Liu TD-HSI). For venous oxygenation specifically, the relevant gap it exposes is that surgical HSI still reports blended StO₂/perfusion rather than venous-resolved sO₂ — motivating the fusion of HSI's real-time wide-field maps with venous-isolating front-ends (induced venous modulation, Papers 1.3/1.5; or transmissive geometry, prior scan). A scoping reference rather than a primary advance — scored accordingly.

---

### Paper 2.5
**Title:** Imaging Hypoxia in the Diabetic Retina: A Potential Early-Detection Imaging Biomarker Before Detectable Retinopathy in Diabetes
**Authors:** Md Imam Uddin, Blake Dieckmann, David E. Burgos
**Year:** 2026 (online ahead of print 2025; assigned to Diabetes vol. 75)
**Venue:** *Diabetes* (American Diabetes Association), 75(3):538
**Link / DOI:** https://doi.org/10.2337/db25-0394
**Metadata verified:** Title, full authors, journal, and DOI confirmed via the American Diabetes Association (diabetesjournals.org) and ResearchGate. Volume/issue/page (75(3):538) reported in one search response and consistent with the db25 manuscript prefix; year straddles 2025 online / 2026 issue — *flagged.*
**Relevance score:** 5 / 10
⚠️ *Uses an exogenous molecular hypoxia probe (HYPOX-4), not endogenous optical venous oximetry — venous-oxygenation relevance is indirect (hypoxia ≈ low venous/tissue oxygen). Included as the most recent primary retinal-oxygen-imaging paper and as the disease-application counterpart to the Paper 2.1 review.*

**Novelty:** Demonstrates that diabetic retinas are significantly hypoxic versus controls and that this hypoxia is detectable with the **HYPOX-4 early-detection imaging probe before any structural retinopathy is visible**, positioning retinal hypoxia (a downstream correlate of impaired oxygen delivery and extraction) as a pre-clinical imaging biomarker.

**Integration insights:** Less a venous-oximetry method than a statement of clinical stakes: it shows that *oxygenation imaging can precede structural disease*, the same value proposition that motivates non-invasive venous/extraction monitoring in critical care and heart failure. The probe-based approach contrasts with the label-free endogenous methods (vis-OCT, spectroscopic oximetry, photoacoustics) that are the real translational path for systemic venous oxygenation — making it a useful boundary case that clarifies why label-free venous oximetry (Papers 2.1–2.3) is the strategically important direction. Scored modestly for the indirect, probe-dependent link.

---

## Cross-Topic Synthesis

This scan deliberately avoided the field's strongest papers (already catalogued on 2026-06-10 and 2026-06-11) and instead mapped the *periphery* of the venous-oxygen literature. Several coherent signals emerge:

**1. The endpoint is shifting from absolute SvO₂ toward oxygen-extraction / OEF.** Three independent Topic-1 entries converge on extraction rather than raw saturation: the ERiO₂ integrated-extraction metric in cardiac surgery (Paper 1.2), the IDo₂ "inadequate oxygen delivery" probability index (Paper 1.1), and the pulsatile diffuse-optics SaO₂/SvO₂/OEF decomposition highlighted in the 2026 Frontiers editorial (Paper 1.4). For optical engineering this is liberating: an instrument that reports OEF (supply − return) is clinically meaningful while being less hostage to the absolute-calibration problem that has stalled standalone optical SvO₂. The retinal multimodal work (Paper 2.2) reaches the same OEF/metabolic-rate endpoint from the imaging side.

**2. "Make the vein pulsatile" is the most transferable venous-specific idea.** The Canterbury induced-modulation line (FES → electro-pneumatic actuator → jugular reflectance; Papers 1.3, 1.5, plus Hill 2024 in the prior scan) solves the foundational obstacle to all optical venous oximetry — veins do not pulse like arteries — at the *signal-generation* stage rather than the inversion stage. This front-end is modality-agnostic and could gate NIRS, hyperspectral, SFDI, or photoacoustic acquisition to a known venous-volume phase. It is arguably the highest-leverage under-explored concept across both topics.

**3. Cross-modal optical validation is maturing (retina leads).** Paper 2.2 co-registers vis-OCT saturation with phosphorescence pO₂ in the same vessels — an orthogonal *optical* gold standard, not a blood draw. This is the validation template the systemic venous field lacks: prior-scan human PA/NIRS venous studies validate against invasive co-oximetry in small cohorts, whereas retinal work can now cross-check two optical readouts in vivo. Migrating that validation philosophy to peripheral veins would accelerate trust in non-invasive systemic venous oximeters.

**4. The fluence problem is being attacked from both ends.** Paper 2.3 (multiple-illumination learned decoloring, an *acquisition-side* solution, validated in humans) complements the *algorithm-side* deep-learning inversions already catalogued (Hybrid-Net, SPOI-AE, qPACT-virtual). A combined acquisition-plus-network pipeline is the credible route to quantitative venous sO₂ at depth — and remains unbuilt.

**5. Honest state of the field.** No brand-new (June-2026) paper this scan reports a *direct* non-invasive measurement of true systemic venous sO₂ in humans that surpasses the landmark works already on file. The genuinely new 2025–2026 material is concentrated in (a) venous-monitoring endpoints and analytics (Papers 1.1, 1.2), (b) induced-modulation hardware (Paper 1.3), and (c) retinal/optical-imaging methods and reviews transferable in principle (Papers 2.1, 2.2, 2.4, 2.5). Relevance scores top out at 7/10 this run, accurately reflecting that the strongest venous-specific optical work was published earlier and captured in prior scans. The most promising unexplored combinations remain: induced venous modulation (Papers 1.3/1.5) + wearable FD-NIRS (prior scan) + a fluence-robust inversion (Paper 2.3 / prior-scan networks), validated cross-modally in the style of Paper 2.2.

### Open questions carried forward
- **No human systemic-vein analogue of Paper 2.2's cross-modal optical validation exists** — every non-retinal venous optical study still validates against invasive co-oximetry in small cohorts.
- **Induced-venous-modulation front-ends (Papers 1.3/1.5) have not been combined with any imaging modality beyond single-wavelength PPG** — pairing them with NIRS/HSI/PA is an obvious, untaken step.
- **OEF, not absolute SvO₂, may be the right optical target** (Papers 1.2, 1.4, 2.2) — but no wearable optical device yet reports calibrated OEF at a defined venous site.
- **HSI and SFDI remain wide-field but venous-blended** (Paper 2.4) — vessel-specific venous isolation in thick human tissue is still unsolved outside the retina and thin murine windows.
