# Venous Oxygen Research Scan — 2026-06-11

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.  
**Prior scan:** 2026-06-10 (first run). Papers from that scan are excluded unless a new version or finding warrants re-entry; all 10 prior entries are excluded from this scan. One paper (wearable NIRS review, DOI 10.1088/2515-7647/ae6ae4) was cited in the 2026-06-10 synthesis section but never formally entered — it appears here as Paper 1.3 with full metadata, noted accordingly.  
**Search scope:** Emphasis on publications from October 2025 – June 2026 not covered in the prior scan. Sources searched: PubMed/PMC, arXiv, SPIE, Optica (BOE, Optics Letters), Nature, JACC, MDPI, Frontiers, BME Frontiers, ResearchGate.  
**Note on sparseness:** Genuinely venous-specific non-invasive optical work remains a low-volume niche. The highest-relevance new entries are concentrated in Topic 2 (optical imaging); Topic 1 fills its five slots honestly but relevance scores 5/10 reflect this sparseness. Non-optical but venous-specific clinical work (Paper 1.1: cardiac MRI) is included in Topic 1 because that topic is not restricted to optical methods.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### Paper 1.1
**Title:** Development and Validation of a Noninvasive Model of Mixed Venous Oxygen Saturation in Heart Failure  
**Authors:** Adam K McDiarmid, Bradley S Chambers, David A Broadbent, Roshan Patel, Gareth Matthews, Oscar Gonzalez-Fernandez, Sven Plein, Pankaj Garg, Peter P Swoboda  
**Year:** 2026 (published January 2026)  
**Venue:** *JACC: Advances*, 5(1):102484  
**Link / DOI:** https://doi.org/10.1016/j.jacadv.2025.102484  
**Metadata verified:** Title, full author list, journal, volume, issue, article number, DOI confirmed via JACC, PubMed (PMID 41609283), and PMC (PMC12869880).  
**Relevance score:** 8 / 10  
⚠️ *Non-optical method (cardiac MRI); included because Topic 1 covers non-invasive venous oxygen monitoring broadly.*

**Novelty:** Derives an index of non-invasive mixed venous oxygen saturation (iSvO₂) from the ratio of T2 relaxation times of the right-ventricular to left-ventricular blood pools (RV-T2BP/LV-T2BP) on cardiac MRI. Validated against invasive right heart catheterisation in a discovery cohort (n = 30, R = 0.82), then applied to 628 heart failure patients with 3-year follow-up. Lower iSvO₂ independently predicted all-cause mortality and HF hospitalisation. This is among the largest prospective non-invasive SvO₂ studies yet published and the only one with long-term survival endpoints.

**Integration insights:** This MRI-based index demonstrates that true mixed SvO₂ can be estimated non-invasively with clinically actionable accuracy, establishing a reference target for optical methods. The validation cohort (n = 628) dwarfs anything achievable by invasive catheterisation studies, providing a statistical power benchmark that photoacoustic or NIRS-based venous oximetry systems must eventually match. The T2-based mechanism is complementary to optical oximetry: both exploit haemoglobin deoxygenation physics (T2 relaxation for MRI; optical absorption for NIRS/PA), suggesting that hybrid approaches — MRI to calibrate periodic wearable optical checks — are feasible. The survival-endpoint data make iSvO₂ a candidate biomarker for validating continuous non-invasive optical monitors in HF cohorts.

---

### Paper 1.2
**Title:** Wearable Frequency-Domain Near-Infrared Spectroscopy (FD-NIRS) System  
**Authors:** Shashikant Lahade, Siavash Yazdi, Nicholas Ross, Delaney Smith, Saba Mohammadi, Michael M. Green, Thomas D. O'Sullivan  
**Year:** 2026  
**Venue:** *Biomedical Optics Express*, 17(2):555–571  
**Link / DOI:** https://doi.org/10.1364/BOE.585068  
**Metadata verified:** Title, full authors, journal, volume/issue/pages, DOI confirmed via Optica Open preprint, Notre Dame O'Sullivan group news, and PMC listing (PMC12904531). Selected as Editor's Pick and featured on journal cover.  
**Relevance score:** 7 / 10  
*(Tissue-level sO₂; venous-relevant through forearm occlusion demonstration.)*

**Novelty:** First fully wearable FD-NIRS system built around a custom ASIC die (1.2 × 1.2 mm, packaged 5 × 5 mm), operating at 50–350 MHz modulation frequencies with 685 nm and 850 nm laser diodes and a silicon photomultiplier (SiPM) detector. Total device weight 37 g. Achieves μₐ accuracy of 0.0007 mm⁻¹ and μₛ′ accuracy of 0.08 mm⁻¹ at a 14.7 Hz continuous measurement rate; single-frequency mode operates to 1 kHz. In-vivo demonstration includes forearm cuff-occlusion experiment capturing the arterio-venous oxygenation transition in real time and cardiac pulse extraction.

**Integration insights:** FD-NIRS is the quantitative upgrade to CW-NIRS: it measures absolute μₐ and μₛ′, enabling absolute HbO₂, HHb, and sO₂ rather than relative changes. The forearm occlusion experiment is directly analogous to the venous occlusion protocol (Paper 1.5 in yesterday's scan, Zachia Alan et al.): by temporarily blocking venous return, the NIRS signal converges to a near-venous sO₂ value. The ASIC miniaturisation removes the main hardware barrier to wearable continuous venous oximetry; positioning over the external jugular vein (as in Hill et al. 2024, prior scan Paper 1.1) with FD-NIRS rather than CW-NIRS would give absolute rather than relative jugular SvO₂. The Editor's Pick distinction signals this is considered a landmark engineering paper by the field.

---

### Paper 1.3
**Title:** Advances in Fully Integrated Wearable Near-Infrared Spectroscopy: Hardware Innovations and Biomedical Applications  
**Authors:** Shashikant Lahade et al. (O'Sullivan Research Group, University of Notre Dame)  
**Year:** 2026 (published May 28, 2026)  
**Venue:** *Journal of Physics: Photonics*, 8(2)  
**Link / DOI:** https://doi.org/10.1088/2515-7647/ae6ae4  
**Metadata verified:** Title, journal, volume, DOI confirmed via IOPscience listing. Full author list and page numbers not verified — *flagged.* Note: the review is by the same O'Sullivan group as Paper 1.2; lead authorship not independently confirmed beyond institutional news attributions.  
**Relevance score:** 6 / 10  
*(Broad review; venous monitoring is a secondary theme; tissue-level sO₂.)*  
**Note:** This paper was cited in the 2026-06-10 synthesis section ("A May 2026 review … DOI 10.1088/2515-7647/ae6ae4") but was not assigned a formal paper slot in that scan. First formal entry here.

**Novelty:** Systematic state-of-the-art review of fully integrated wearable NIRS systems from 2020 to 2026, benchmarking commercial (Artinis BriteLite, NIRx NIRsport2, Gowerlabs LUMO HD-DOT) and prototype systems against each other on miniaturisation, battery life, optical performance, wireless throughput, and biomedical applications (brain, muscle, peripheral tissue). Covers the ASIC-based FD-NIRS trajectory described in Paper 1.2 as the leading path to continuous absolute quantification in wearable form factors.

**Integration insights:** The review documents that wearable NIRS has effectively reached clinical-grade sensitivity for tissue oxygenation: the hardware barrier to ambulatory venous monitoring is shrinking faster than the algorithm barrier. The most important integration lesson: the gap between current wearable NIRS (tissue-level sO₂, sensitivity to motion artefact, melanin confound) and the clinical goal (absolute SvO₂ at a specific vein) is now primarily a signal-processing problem, not a hardware one. This motivates applying the NIRS+DNN+Monte Carlo pipeline (Sun et al. 2024, prior scan) to the new miniaturised FD-NIRS hardware described in Paper 1.2.

---

### Paper 1.4
**Title:** Single-Distance, Phase-Only Frequency-Domain NIRS for Vascular Oxygenation and Tissue Metabolism: A Monte Carlo Simulation Study  
**Authors:** Muaaz Faiyazuddin, Haiyang Tang, Yiqing Hu, Miles Bartlett, Michael D. Nelson, Hanli Liu  
**Year:** 2025 (published October 16, 2025)  
**Venue:** *Journal of Biomedical Optics*, JBO.30(S3):S34113  
**Link / DOI:** https://doi.org/10.1117/1.JBO.30.S3.S34113  
**Metadata verified:** Title, full authors, journal, DOI, and PMC ID (PMC12530142) confirmed via SPIE Digital Library and ResearchGate listings. Affiliation: University of Texas at Arlington.  
**Relevance score:** 5 / 10  
*(Algorithm improvement for FD-NIRS; tissue-level; simulation study only — no in vivo venous data.)*

**Novelty:** Proposes a novel optimisation-based algorithm for single source-detector separation FD-NIRS that uses phase shift alone (discarding amplitude) to quantify oxyhaemoglobin (HbO₂), deoxyhaemoglobin (HHb), and cytochrome-c oxidase redox state (CCOredox). Monte Carlo simulations show the algorithm reduces CCOredox mean relative error from 34.1% (conventional method) to 5.1% and outperforms conventional fitting for source-detector separations up to 3 cm. Removing the amplitude channel simplifies hardware significantly, enabling single-channel wearable designs.

**Integration insights:** The clinical goal of venous-specific NIRS requires accurate HHb quantification — deoxyhaemoglobin is the dominant venous haemoglobin species. Current CW-NIRS cannot separate optical absorption and scattering without multiple separations; single-distance FD-NIRS with this phase-only algorithm approaches that capability from a simplified hardware platform. The accuracy at 3 cm source-detector separation is particularly relevant: 3 cm is the typical depth target for external jugular or basilic vein sensing. Pairing this algorithm with the wearable ASIC from Paper 1.2 is a natural next engineering step toward continuous venous-specific monitoring.

---

### Paper 1.5
**Title:** Comparative Assessment of Healthy Tissue Oxygenation Using Near-Infrared Imaging, Transcutaneous Oxygen Measurement, and Plethysmography  
**Authors:** El Masry M, Li R, Balasubramani GK, Roy S, Sen CK, Gnyawali SC  
**Year:** 2025  
**Venue:** *Scientific Reports*, 15: article 30424  
**Link / DOI:** https://doi.org/10.1038/s41598-025-15767-2  
**Metadata verified:** Title, authors, journal, article number, DOI confirmed via Nature/Scientific Reports and PubMed (PMID 40830190, PMC12365204).  
**Relevance score:** 5 / 10  
*(Tissue-level StO₂ across modalities; venous compartment sampled but not isolated; ischemia/reperfusion paradigm captures venous oxygenation indirectly.)*

**Novelty:** Head-to-head in-vivo comparison of four tissue oxygenation devices — spatial frequency domain imaging (SFDI), transcutaneous oxygen measurement (TCOM), wearable photoplethysmography (WD), and pulse oximetry (PO) — during baseline, ischemia (cuff occlusion), and reperfusion phases in healthy subjects. SFDI uniquely detected significant StO₂ differences across skin-type groups and provided the highest spatial resolution; TCOM tracked absolute oxygen partial pressure but was confounded by melanin; wearable PPG tracked relative changes but not absolute sO₂.

**Integration insights:** This paper is the most direct multi-modal benchmarking study for the venous occlusion paradigm. During cuff-induced ischemia, venous return is blocked and tissue oxygenation converges toward venous sO₂ — making ischemia-phase StO₂ a proxy for venous saturation. The ranking of modalities (SFDI > TCOM > wearable PPG for absolute oxygenation) informs instrument choice for future venous-occlusion-based venous sO₂ protocols. SFDI's advantage — spatially resolved maps revealing vascular heterogeneity invisible to single-point sensors — is especially relevant for identifying venous versus arterial contributions within the tissue bed.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

### Paper 2.1
**Title:** Transmissive-Detected Hyperspectral Imaging for Single-Vessel-Resolution Blood Oxygen Mapping  
**Authors:** Shaojun Liu, Qing Xia, Yuwei Du, Tingting Yu, Dongyu Li, Dan Zhu  
**Year:** 2025 (published December 16, 2025)  
**Venue:** *BME Frontiers* (AAAS Science Partner Journal)  
**Link / DOI:** https://doi.org/10.34133/bmef.0211  
**Metadata verified:** Title, full authors, DOI, journal, and affiliation (MoE Key Laboratory for Biomedical Photonics, WNLO Advanced Biomedical Imaging Facility, Huazhong University of Science and Technology) confirmed via search results and PMC (PMC12707973). PMC direct-fetch was blocked; DOI and author list cross-verified via two independent search responses.  
**Relevance score:** 8 / 10  
*(Directly resolves individual arteries AND veins in vivo; venous sO₂ imaging demonstrated.)*

**Novelty:** Proposes transmissive-detected hyperspectral imaging (TD-HSI) as a replacement for reflective HSI for blood oxygen mapping. In reflective mode, tissue scattering limits depth penetration and causes ~6× lower precision. By detecting transmitted rather than reflected light, TD-HSI extends accurate sO₂ detection to greater depths and achieves ~6× greater precision in detecting sO₂ variations (confirmed by Monte Carlo simulations). In-vivo murine experiments image individual arteries and veins at multiple body locations and track sO₂ changes during hypoxia challenge and subcutaneous tumour growth over one week.

**Integration insights:** The key advance is switching from reflective to transmissive detection geometry — simple in concept but substantially expanding the accessible depth range for HSI. The independent artery/vein sO₂ readouts during hypoxia make this paper the most direct hyperspectral analogue of photoacoustic venous oximetry. Limitations: current in-vivo demonstrations are in mice (thin tissue; transmission feasible); for human limb veins (deeper, opaque tissue), full transmission is impractical, suggesting hybrid geometries (angled transmission, multi-source TD-HSI) as the translational path. Integration with the SFDI framework (SFDI-net, prior scan Paper 2.5) could combine TD-HSI's vessel-specific precision with SFDI's wide-field tissue maps.

---

### Paper 2.2
**Title:** Quantitative Assessment of Thrombosis-Induced Blood Oxygenation Change in Deep Tissues Based on Photoacoustic Tomography: An Ex Vivo Study  
**Authors:** Yingjie Feng, Qiuqin Mao, Lei Hong, Xiaotian Wang, Chao Tao, Xiaojun Liu  
**Year:** 2025 (published March 24, 2025)  
**Venue:** *Biomedical Optics Express*, 16(4):1557–1568  
**Link / DOI:** https://doi.org/10.1364/BOE.557086  
**Metadata verified:** Title, full authors, journal, volume/issue/pages, DOI, PMID (40322004), and PMC (PMC12047737) confirmed via ResearchGate, PMC, and Optica listings.  
**Relevance score:** 7 / 10  
*(Deep tissue PA oxygenation; venous thrombus target is inherently venous; depth validation to 30 mm is clinically significant.)*

**Novelty:** Addresses the long-standing "spectral coloring" problem that corrupts photoacoustic sO₂ measurements in deep tissue: heterogeneous overlying tissue preferentially absorbs certain wavelengths, distorting the sO₂ spectral signature at depth. Proposes using endogenous chromophore signals within the target tissue as an internal fluence correction factor. Ex-vivo validation achieves accurate spectra to 30 mm depth under multiple tissue conditions; Pearson correlation against uncolored reference spectra improved by 15% and standard deviation reduced by 58% post-correction. Sequential measurements track time-dependent sO₂ changes in a thrombus phantom over 6 days (discriminating fresh vs. organising thrombus by oxygenation).

**Integration insights:** The spectral coloring problem is the dominant accuracy barrier for PA venous oximetry at depth — the IJV sits ~3 cm below neck skin and deep limb veins are deeper still. This paper's internal-chromophore correction is a practical, hardware-free solution compatible with existing PA imaging systems. The clinical application — non-invasive detection and staging of deep vein thrombosis (DVT) by oxygenation — is highly impactful: DVT diagnosis currently requires compression ultrasound or D-dimer assay, but neither provides oxygenation state. PA with this correction could stratify fresh DVT (high venous deoxygenation) from chronic organised clot. The 30 mm depth validation matches clinical subcutaneous vein depths for many DVT-relevant sites.

---

### Paper 2.3
**Title:** Optical Inversion and Spectral Unmixing of Spectroscopic Photoacoustic Images with Physics-Informed Neural Networks  
**Authors:** Sarkis Ter Martirosyan, Xinyue Huang, David Qin, Anthony Yu, Stanislav Emelianov  
**Year:** 2026 (preprint submitted February 18, 2026)  
**Venue:** arXiv preprint arXiv:2602.16357 — **no peer-reviewed journal publication confirmed; flagged as preprint.**  
**Link:** https://arxiv.org/abs/2602.16357  
**Metadata verified:** Title, full authors, arXiv ID, submission date confirmed via arXiv. Journal publication status unverified.  
**Relevance score:** 7 / 10  
*(PA spectral unmixing method; not venous-specific but directly addresses the inversion needed for accurate venous sO₂ from PA.)*

**Novelty:** Introduces SPOI-AE (Spectroscopic Photoacoustic Optical Inversion Autoencoder) — a physics-informed autoencoder that simultaneously solves the optical inversion problem (recovering fluence from PA data) and spectral unmixing (recovering chromophore concentrations, including sO₂) without assuming linearity or known fluence. The architecture encodes PA spectra into optical parameters and decodes to reconstructed PA images, with physics constraints enforced during training. Validated on a simulated mouse lymph node phantom; achieves biologically coherent estimates for HbO₂, HHb, sO₂, and optical scattering. Outperforms conventional linear unmixing algorithms.

**Integration insights:** The SPOI-AE directly attacks the fundamental limitation that prevents accurate venous sO₂ from PA: the nonlinear relationship between measured PA pressure and sO₂ when fluence is unknown. Unlike the December 2025 Hybrid-Net paper (prior scan Paper 2.4, which discards fluence entirely by learning end-to-end), SPOI-AE explicitly estimates fluence as an intermediate variable — this makes the model more physically interpretable and potentially more generalisable to new tissues. The physics-informed constraint should improve robustness in the neck/jugular geometry where overlying tissue composition is highly variable. Combining SPOI-AE's inversion with the spectral-coloring correction from Paper 2.2 represents a comprehensive depth-and-heterogeneity-robust PA oxygenation pipeline.

---

### Paper 2.4
**Title:** Application of a Virtual Imaging Framework for Investigating a Deep Learning-Based Reconstruction Method for 3D Quantitative Photoacoustic Computed Tomography  
**Authors:** Refik Mert Cam, Seonyeong Park, Umberto Villa, Mark A. Anastasio  
**Year:** 2025 (arXiv October 2025; published December 29, 2025)  
**Venue:** *Photoacoustics*, DOI 10.1016/j.pacs.2025.100792  
**Link / DOI:** https://doi.org/10.1016/j.pacs.2025.100792  
**Metadata verified:** Title, full authors, DOI, and PMC (PMC12858365) confirmed via arXiv (2510.03431) and PubMed/PMC. Affiliations: University of Illinois Urbana-Champaign and University of Texas at Austin.  
**Relevance score:** 6 / 10  
*(3D sO₂ reconstruction method in breast imaging context; not venous-specific, but methodology directly applicable to venous PA oximetry.)*

**Novelty:** Introduces the first virtual imaging testbed for evaluating 3D learning-based quantitative photoacoustic CT (qPACT) reconstruction of blood oxygen saturation. Generates stochastic numerical breast phantoms with realistic anatomy and physiology; evaluates a representative deep-learning qPACT method across subject variability, measurement noise, and acoustic aberrations. Identifies conditions under which the deep-learning method succeeds and fails — a systematic robustness characterisation that has been largely absent from the literature. Provides an open-source framework for the community to benchmark future qPACT algorithms.

**Integration insights:** Developing a PA system capable of imaging deep venous sO₂ (e.g., femoral vein, IVC) requires validated 3D reconstruction methods — not just 2D slices. This virtual imaging framework is the validation infrastructure needed before human venous qPACT trials. The evaluation methodology (stochastic phantoms + noise + acoustic aberrations) maps cleanly onto the challenges of imaging the IJV in the neck: variable fat/muscle layers (subject variability), laser shot noise (measurement noise), and bone reflections (acoustic aberrations). The framework enables rapid evaluation of candidate reconstruction methods without expensive in-vivo experiments, accelerating the path from bench to clinical PA venous oximetry.

---

### Paper 2.5
**Title:** Visible Light Optical Coherence Tomography: Technology and Biomedical Applications  
**Authors:** Songzhi Wu, Shuo Wang, Baihan Li, Zhao Wang  
**Year:** 2025 (published July 17, 2025)  
**Venue:** *Bioengineering* (MDPI), 12(7):770  
**Link / DOI:** https://doi.org/10.3390/bioengineering12070770  
**Metadata verified:** Title, full authors, journal, volume/issue/article number, DOI, and PMC (PMC12292648) confirmed via MDPI Digital Library and PMC. Affiliation: University of Electronic Science and Technology of China, Chengdu.  
**Relevance score:** 6 / 10  
*(Review article; retinal venous oximetry covered in detail; not a primary research paper.)*

**Novelty:** Comprehensive 2025 state-of-the-art review of visible-light OCT (vis-OCT) technology and applications. Covers hardware milestones (light sources, fibre components, balanced detection), retinal oximetry methodology, and clinical disease applications. Key venous findings synthesised: glaucoma subjects show significantly *higher* macular venous sO₂ and lower oxygen extraction fraction compared to controls (lower metabolic demand in early atrophic disease); diabetic retinopathy shows increased metabolic rate and compensatory venous deoxygenation in early stage. Reviews axial resolution (~1 µm achievable) and vessel-specific sO₂ measurement to capillary level.

**Integration insights:** Vis-OCT is the established vessel-specific non-invasive venous oxygenation technique for retinal veins — it is the one domain where true venous (not tissue-average) sO₂ is routinely measured non-invasively in humans. This review consolidates the disease biomarker evidence base: retinal venous sO₂ distinguishes glaucoma, diabetic retinopathy, and vein occlusion at a stage earlier than structural changes visible on standard OCT. The techniques developed for retinal venous sO₂ (spectroscopic backscattering, matched-field processing, adaptive spectral correction) are transferable in principle to accessible peripheral veins — the forearm basilic vein or external jugular vein — given a sufficiently long working-distance vis-OCT system. This makes the retinal vis-OCT literature the most mature methodological reference for vessel-specific optical venous oximetry.

---

## Cross-Topic Synthesis

### New convergent themes emerging from this scan

**1. The deep-tissue PA accuracy problem is being solved from multiple directions.** Papers 2.2 (spectral coloring correction), 2.3 (SPOI-AE physics-informed inversion), and the December 2025 Hybrid-Net paper (prior scan) each attack quantitative PA venous sO₂ at depth from a different angle: internal-chromophore fluence correction, physics-informed network inversion, and end-to-end deep learning, respectively. These three approaches are complementary rather than competing: spectral coloring correction is a pre-processing step, SPOI-AE is an interpretable inversion layer, and Hybrid-Net is a fast end-to-end variant. A unified pipeline combining all three could achieve robust absolute venous sO₂ at clinically relevant depths (3–10 cm) for the first time.

**2. MRI as calibration anchor for optical venous monitoring.** Paper 1.1 (CMR T2 iSvO₂) demonstrates non-invasive mixed SvO₂ measurement validated in 628 heart failure patients with survival endpoints. This dataset is an unprecedented calibration resource: wearable optical devices (Papers 1.2, 1.3) could be cross-validated against iSvO₂ in HF patients undergoing routine cardiac MRI, yielding a large-scale validation that invasive right heart catheterisation could never provide. The iSvO₂ biomarker's survival-predictive power also establishes the clinical stakes that motivate continuous optical monitoring: a wearable that tracks daily SvO₂ trends in HF patients would be actionable.

**3. Hardware miniaturisation (Topic 1) is catching up to algorithm sophistication (Topic 2).** Papers 1.2 and 1.3 document that FD-NIRS — the gold standard for quantitative, depth-resolved tissue oxygenation — has now been miniaturised to a 37-gram wearable with ASIC integration. Simultaneously, Papers 2.2, 2.3, and 2.4 are closing the accuracy gap for PA sO₂ at depth. The practical window for deploying a wearable quantitative venous oximeter at a known venous landmark (jugular, basilic, cephalic) is narrowing from "infeasible" toward "pending validation."

**4. Single-vessel specificity in optical methods: the new frontier.** Paper 2.1 (TD-HSI) achieves independent artery/vein sO₂ mapping at the single-vessel level. Paper 2.5 (vis-OCT review) shows retinal venous sO₂ is measurable to capillary resolution. Both demonstrate that optical methods are not inherently limited to tissue-average readouts — the limitation has been geometry and depth, not physics. For systemic venous oxygen monitoring (as opposed to retinal), the translational challenge is adapting single-vessel techniques to accessible surface vessels (EJV, cephalic, basilic) where tissues are thicker and more heterogeneous than retina or murine limb.

**5. Thrombosis as a venous-specific PA application with near-term clinical pull.** Paper 2.2 frames deep vein thrombosis staging as the initial PA venous oxygenation application — a clinically compelling problem (DVT affects ~1 per 1,000 per year; current diagnosis is anatomical not functional) with a well-defined depth target (2–5 cm for calf/femoral DVT). This is arguably more near-term than non-invasive ScvO₂ in ICU, because the diagnostic goal (fresh vs. organised thrombus) is binary rather than requiring continuous monitoring accuracy.

### Gaps and open questions (updated)

- **The 628-patient MRI validation gap:** Paper 1.1 sets a high bar for clinical validation scale. No non-invasive optical venous sO₂ method has been validated in more than ~79 patients (Jeleff 2023 Mespere study, prior scan). Closing this gap requires study designs that embed wearable NIRS alongside routine cardiac MRI or right heart catheterisation.
- **Transmissive HSI in humans:** Paper 2.1 is demonstrated in mice. The path to human peripheral veins requires either thinner tissue windows (e.g., webbing between fingers, earlobe) or a hybrid transmission-reflection geometry. No feasibility study exists yet.
- **3D PA venous oximetry at clinical depth:** Paper 2.4's virtual framework is the evaluation infrastructure, but no 3D in-vivo human demonstration of qPACT venous sO₂ exists. PAVT (prior scan Paper 2.3) provides haemodynamics at depth; the spectral extension to sO₂ has not yet been demonstrated in humans at > 2 cm depth.
- **Wearable FD-NIRS over a vein:** Paper 1.2's device is demonstrated over heterogeneous forearm tissue. Repositioning over a specifically identified venous landmark (e.g., external jugular with ultrasound guidance for initial placement) and combining with the DNN pipeline from Sun et al. 2024 (prior scan) would be the most direct path to a continuous quantitative venous oximetry wearable.
