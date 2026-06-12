# Venous Oxygen Research Scan — 2026-06-12

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.
**Prior scans in this repository:** 2026-06-10 (first run, 10 papers) and 2026-06-11 (10 papers). All 20 prior entries are excluded from selection here unless a genuinely newer version/finding warrants re-entry (none did).
**Search scope:** PubMed/PMC, arXiv, Optica (BOE, Optics Letters, Communications Medicine), Nature, IEEE Xplore/EMBC/CHASE, Wiley (J. Biophotonics), Springer (BioMedical Engineering OnLine, J. Clin. Monit. Comput.), ScienceDirect, Justia (patents), university group pages (UT Austin Lu Group, OHSU/Northwestern vis-OCT).

**⚠️ Honest note on sparseness (important this run):** The two prior scans already captured essentially all of the freshest (Oct 2025 – Jun 2026) venous-relevant optical work — the 2026 FD-NIRS ASIC papers, TD-HSI, the PA spectral-coloring and physics-informed-inversion preprints, the qPACT virtual framework, the CMR iSvO₂ study, and the vis-OCT review. **No brand-new (post-2026-06-11) venous-specific optical paper surfaced today** despite targeted searching. Rather than pad with arterial-only SpO₂ work, this scan deliberately surfaces **genuinely venous-specific papers that were never entered in the prior two scans**, even where they are older (2016–2023). Several are foundational venous-oximetry methods that the recent work builds on; their relevance scores are calibrated honestly. One cluster (the UT Austin optical e-tattoo line, Topic 1) is venous-specific, directly on-mission, and carries a **January 2025 continuation as a granted-published US patent application** — the newest artifact in this scan.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### Paper 1.1
**Title:** Towards Simultaneous Noninvasive Arterial and Venous Oxygenation Monitoring with Wearable E-Tattoo
**Authors:** Philip Tan, Eric Wang, Shreya Tamma, Sarnab Bhattacharya, Nanshu Lu
**Year:** 2023 (conference); continuation published as US patent application **US 2025/0025074 A1**, 23 Jan 2025
**Venue:** *2023 45th Annual International Conference of the IEEE Engineering in Medicine & Biology Society (EMBC)*
**Link / DOI:** https://doi.org/10.1109/EMBC40787.2023.10340010 (PMID 38083768) · Patent: https://patents.justia.com/patent/20250025074
**Metadata verified:** Title, full author list, venue, DOI, and PMID confirmed via IEEE Xplore (doc 10340010), PubMed (38083768), and the UT Austin Lu Group listing. Patent number, filing/publication date, and inventor list (Tan, Wang, Tamma, Bhattacharya, Lu) confirmed via Justia.
**Relevance score:** 8 / 10
*(Directly venous-specific; point-sensor PPG rather than imaging, but the artery/vein discrimination problem is the core of optical venous oximetry.)*
**Note:** Never surfaced in prior scans (predates them, 2023). Included because it is venous-specific, on-mission, and has a newer 2025 patent continuation. Same Lu Group as the deep-neck e-tattoo (Paper 1.3).

**Novelty:** A soft, skin-conformal optical "e-tattoo" laminating an array of multi-wavelength PPG emitters/detectors directly over a co-located artery and vein. The work demonstrates *in vivo* that PPG can resolve a distinct **venous pulsatile component** — challenging the long-standing assumption that PPG only senses arterial pulsation — and proves the signal origin is venous. It then characterises the dominant obstacle to simultaneous SaO₂/SvO₂ extraction: **arterio-venous optical crosstalk** from the close anatomical proximity of artery and vein, studied via simulation, in vitro, and in vivo, with a proposed spatial-filtering mitigation.

**Integration insights:** This is the most directly on-mission Topic 1 entry in this scan: a wearable, vessel-pair-targeted optical sensor whose explicit goal is non-invasive SvO₂. It is the conformal-electronics counterpart to the rigid jugular reflectance sensor (Hill et al. 2024, prior scan 1.1) and the Mespere VO100 (Jeleff et al. 2023, prior scan 1.3). The crosstalk analysis is the key transferable contribution — every surface optical venous method (NIRS, PPG, SFDI) faces the same arterial-contamination problem that vessel-specific modalities (PA, vis-OCT) sidestep. The spatial-filtering approach here is complementary to the subject-specific Monte-Carlo + DNN inversion of Sun et al. 2024 (prior scan 1.2): one attacks crosstalk in hardware/geometry, the other in the inversion model. The 2025 patent signals an active translational push toward a commercial wearable venous oximeter.

---

### Paper 1.2
**Title:** Proof of Concept Non-Invasive Estimation of Peripheral Venous Oxygen Saturation
**Authors:** Musabbir Khan, Chris G. Pretty, Alexander C. Amies, Joel Balmer, Houda E. Banna, Geoffrey M. Shaw, J. Geoffrey Chase
**Year:** 2017
**Venue:** *BioMedical Engineering OnLine*, 16(1):60
**Link / DOI:** https://doi.org/10.1186/s12938-017-0351-x (PMC5437414)
**Metadata verified:** Title, full author list, journal, article number, year, and DOI confirmed via Springer/BMC and PMC; author list cross-checked against the German National Library (d-nb.info) record.
**Relevance score:** 7 / 10
*(Directly venous-specific; procedural artificial-modulation method, not continuous imaging.)*
**Note:** Foundational paper from the University of Canterbury group (Pretty, Chase) that later produced the jugular reflectance sensor in prior scan 1.1 (Hill et al. 2024). Never previously entered.

**Novelty:** Introduces an **Artificial Pulse Generation (APG)** pulse-oximetry method that exploits the *compliance difference between arteries and veins*: a digit pressure cuff imposes a respiration-like external modulation that renders the otherwise non-pulsatile peripheral venous blood pulsatile. The induced venous PPG component is then isolated and a calibration model estimates regional venous saturation (SpvO₂) in parallel with arterial SpaO₂. Median paired accuracy against gold-standard reference was reported at 0.29% (venous) and 0.65% (arterial).

**Integration insights:** This is the conceptual ancestor of the e-tattoo crosstalk work (Paper 1.1) and a direct cousin of the venous-occlusion equilibration approach (Zachia Alan et al. 2022, prior scan 1.5): all three create a *controlled physiological perturbation* to coax a venous-specific optical signal out of a mixed tissue bed. APG is attractive because it works at any accessible peripheral PPG site (finger, wrist) with conventional pulse-oximeter hardware, making it a low-cost screening complement to imaging-grade methods (PA, vis-OCT). Its main limitation — reliance on an external cuff and per-subject calibration — defines exactly the gap that wearable conformal sensors (Paper 1.1) and model-based inversion (Sun et al. 2024) aim to close.

---

### Paper 1.3
**Title:** Wearable Optical E-Tattoo for Deep Neck Hemodynamic Monitoring
**Authors:** Philip Tan, Shreya Tamma, Sarnab Bhattacharya, James W. Tunnell, Nanshu Lu
**Year:** 2022
**Venue:** *Proc. 2022 IEEE/ACM Conference on Connected Health: Applications, Systems and Engineering Technologies (CHASE)*
**Link / DOI:** https://doi.org/10.1145/3551455.3559604 (IEEE Xplore doc 9983611)
**Metadata verified:** Title, full author list, venue, and ACM DOI confirmed via the UT Austin Lu Group PDF listing and IEEE Xplore; author list cross-checked against Semantic Scholar.
**Relevance score:** 6 / 10
*(Venous-relevant precursor; demonstrates artery/vein PPG discrimination on the neck but is framed as hemodynamic — not yet SvO₂ — monitoring.)*
**Note:** Precursor to Paper 1.1; never previously entered.

**Novelty:** Establishes the **PPG-penetration-depth feasibility** underpinning the e-tattoo program. Using computational and in-vitro phantom models plus in-vivo testing, it rebuts the assumption that PPG cannot reach the carotid artery and internal/external jugular vein on the neck, and demonstrates that a conformal optical e-tattoo can distinguish arterial from venous pulses at the deep-neck site — the same anatomical target as the photoacoustic IJV oximetry of Garcia-Uribe et al. 2023 (prior scan 2.1).

**Integration insights:** The neck is the highest-value venous oximetry site because IJV/ScvO₂ is the clinical surrogate for central venous oxygenation. This paper shows a *wearable, low-cost* modality can reach that depth optically — positioning conformal PPG as a continuous-monitoring complement to the depth-resolved-but-bench-top PA approach. Combined with Paper 1.1's crosstalk mitigation and the Mespere/jugular-NIRS clinical validations (prior scan 1.1, 1.3), it sketches a coherent translational path: deep-neck conformal optics → arterial/venous separation → calibrated SijvO₂.

---

### Paper 1.4
**Title:** Comparison of Non-Invasive Peripheral Venous Saturations with Venous Blood Co-Oximetry
**Authors:** A. M. Belhaj, J. P. Phillips, P. A. Kyriacou, R. M. Langford
**Year:** 2017 (Epub 21 Nov 2016)
**Venue:** *Journal of Clinical Monitoring and Computing*, 31(6):1213–1220
**Link / DOI:** https://doi.org/10.1007/s10877-016-9959-9 (PMID 27873173, PMC5655584)
**Metadata verified:** Title, full author list, journal, volume/issue/pages, year, DOI, and PMID confirmed via Springer and PubMed/PMC listings.
**Relevance score:** 6 / 10
*(Directly venous-specific clinical validation; PPG-based point measurement, not imaging.)*
**Note:** Never previously entered; complements Paper 1.2 by providing the co-oximetry validation arm for non-invasive peripheral venous saturation.

**Novelty:** A clinical validation study comparing **non-invasively derived peripheral venous oxygen saturation against gold-standard venous blood co-oximetry**. The work (City, University of London — Kyriacou's biomedical photonics group) tackles the central credibility question for all surface venous oximetry: does the optically estimated venous saturation actually track the laboratory venous blood value? It reports agreement statistics (bias/limits-of-agreement) between the non-invasive estimate and co-oximetry across subjects.

**Integration insights:** Validation against co-oximetry is the accuracy bar that every method in this program must clear — and very few have (the largest optical venous validation remains Jeleff et al.'s 79-patient jugular-NIRS study, prior scan 1.3; the largest non-invasive SvO₂ validation overall is the 628-patient CMR iSvO₂ study, prior scan 1.1). This paper supplies an independent peripheral-venous validation reference point and a methodological template (Bland–Altman vs. co-oximetry) that future wearable (Paper 1.1) and PA venous-oximetry studies should replicate. It also reinforces that the Canterbury APG approach (Paper 1.2) and the London PPG approach are convergent: both seek calibrated SpvO₂ from peripheral PPG.

---

### Paper 1.5
**Title:** A New Method for Noninvasive Venous Blood Oxygen Detection
**Authors:** Xu Zhang, Min Zhang, Shuicai Zheng, et al.
**Year:** 2016
**Venue:** *BioMedical Engineering OnLine*, 15:84
**Link / DOI:** https://doi.org/10.1186/s12938-016-0208-8 (PMID 27436186, PMC4952148)
**Metadata verified:** Title, journal, article number, year, DOI, and PMID confirmed via Springer/BMC, PubMed, PMC, and Wikidata (Q37111362). **Full author given names beyond the first three not independently confirmed — flagged.**
**Relevance score:** 5 / 10
*(Directly venous-specific in intent; early-stage method, limited validation; included to document the external-stimulation lineage.)*
**Note:** Never previously entered; foundational external-stimulation venous-oximetry concept.

**Novelty:** A light-absorption (NIRS-style) method that applies an **external mechanical stimulation signal to generate a cyclical fluctuation in the vein**, deliberately creating a venous-frequency modulation to overcome the poor signal-to-noise ratio that plagues non-pulsatile venous measurement. SvO₂ is then recovered continuously and in real time; under induced hypoxia the system tracked the overall decline in venous saturation.

**Integration insights:** This is the same physical insight that drives the Canterbury APG method (Paper 1.2) and, in a different guise, the venous-occlusion equilibration approach (prior scan 1.5): **impose a known venous-specific modulation, then demodulate to isolate the venous compartment.** It documents the independent emergence of "active modulation" as the dominant strategy for venous-selective optical sensing — a strategy that conformal wearables (Paper 1.1) now seek to implement passively (via geometry/spatial filtering) rather than with an external actuator. Mainly of historical/lineage value; relevance capped at 5/10 due to limited validation depth.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

### Paper 2.1
**Title:** Adaptive Spectroscopic Visible-Light Optical Coherence Tomography for Clinical Retinal Oximetry
**Authors:** Ian Rubinoff, Roman V. Kuranov, Raymond Fang, Zeinab Ghassabi, Yuanbo Wang, Lisa Beckmann, David A. Miller, Gadi Wollstein, Hiroshi Ishikawa, Joel S. Schuman, Hao F. Zhang
**Year:** 2023 (published 24 April 2023)
**Venue:** *Communications Medicine* (Nature Portfolio), 3:57
**Link / DOI:** https://doi.org/10.1038/s43856-023-00288-8 (PMID 37095177, PMC10126115)
**Metadata verified:** Title, full author list, journal, article number, year, DOI, and PMID confirmed via Nature Communications Medicine, PubMed/PMC, Duke Scholars, and OHSU Pure listings.
**Relevance score:** 8 / 10
*(True vessel-specific venous sO₂ in humans — retinal veins — with quantified accuracy; depth/site limited to retina.)*
**Note:** The 2025 vis-OCT *review* (prior scan 2.5, Wu et al.) cited this body of work; this is the **primary clinical research paper** underpinning it and is entered here for the first time.

**Novelty:** Introduces **adaptive spectroscopic vis-OCT (ADS-vis-OCT)**, which models and removes the "spectral contaminants" (SCs) that have been the chief barrier to reliable vis-OCT oximetry, isolating the true oxygen-dependent backscattering signal. In 18 human participants it achieves **RMSE of 2.1% between major-artery sO₂ and pulse oximetry**, with repeatability (SD of repeated measurements) of **2.5% in smaller arteries and 2.3% in veins** — across vessels of varying diameter. This is among the strongest published accuracy/repeatability results for non-invasive *vessel-specific* sO₂ in humans.

**Integration insights:** Retinal vis-OCT is the one setting where true (not tissue-averaged) venous sO₂ is routinely measured non-invasively and vessel-by-vessel in humans — making it the methodological gold standard the rest of the field aspires to. The SC-removal strategy is the conceptual analogue of the photoacoustic "spectral coloring" correction (Feng et al. 2025, prior scan 2.2): both isolate the oxygen-dependent spectral signature from confounds introduced by overlying/intervening tissue. The 2.3% venous repeatability sets a concrete precision target for PA, HSI, and SFDI venous-oximetry systems. The open translational question — restated from prior scans — is porting these vessel-specific spectroscopic methods from the optically thin, accessible retina to deeper, opaque peripheral veins (EJV, basilic, cephalic).

---

### Paper 2.2
**Title:** Multispectral Optoacoustic Tomography of Muscle Perfusion and Oxygenation under Arterial and Venous Occlusion: A Human Pilot Study
**Authors:** Angelos Karlas, Michael Kallmayer, Nikolina-Alexia Fasoula, Evangelos Liapis, Michail Bariotakis, Markus Krönke, Maria Anastasopoulou, Josefine Reber, Hans-Henning Eckstein, Vasilis Ntziachristos
**Year:** 2020
**Venue:** *Journal of Biophotonics*, 13(6):e201960169
**Link / DOI:** https://doi.org/10.1002/jbio.201960169 (TUM/Helmholtz Munich)
**Metadata verified:** Title, full author list, journal, volume/issue/article number, and DOI confirmed via Wiley Online Library listing and TUM author records (scispace/mediaTUM). Direct page fetch blocked; metadata cross-checked across three independent sources.
**Relevance score:** 7 / 10
*(Imaging method that explicitly isolates the venous compartment via venous occlusion and identifies veins vs. arteries; tissue-bed sO₂ rather than intraluminal SvO₂.)*
**Note:** Never previously entered; the most directly venous-relevant MSOT/optoacoustic clinical pilot not yet covered.

**Novelty:** A handheld hybrid **MSOT–ultrasound** human pilot (forearm, 4 volunteers) that maps spatially resolved HbO₂, Hb, total haemoglobin, and sO₂ during **separate arterial and venous occlusion** maneuvers — explicitly using the venous-occlusion paradigm to drive the tissue toward a venous-dominated oxygenation state, and resolving arteries vs. veins on the co-registered images without any contrast agent.

**Integration insights:** This is the optoacoustic analogue of the NIRS venous-occlusion test (Zachia Alan et al. 2022, prior scan 1.5) and the SFDI artery/vein-occlusion discrimination noted in this field — but with the spatial resolution to *image* which vessels and tissue regions are responding. It bridges the two prior-scan PA threads: the human IJV oximetry of Garcia-Uribe et al. 2023 (vessel-specific, neck) and the deep-flow PAVT/PACT work of Zhang/Kong et al. 2024 (haemodynamics). The venous-occlusion protocol is the practical bridge from tissue-level optoacoustic sO₂ toward venous-specific values, and the handheld MSOT-US form factor is closer to clinical deployment than tomographic bench systems. Limitation: extracted sO₂ is still a tissue/regional readout, not intraluminal SvO₂.

---

### Paper 2.3
**Title:** Motion Rejection and Spectral Unmixing for Accurate Estimation of In Vivo Oxygen Saturation Using Multispectral Optoacoustic Tomography
**Authors:** Mitradeep Sarkar, Mailyn Pérez-Liva, Gilles Renault, Bertrand Tavitian, Jérôme Gateau
**Year:** 2023
**Venue:** *IEEE Transactions on Ultrasonics, Ferroelectrics, and Frequency Control* (also arXiv:2309.08223)
**Link / DOI:** https://doi.org/10.1109/TUFFC.2023.3306592 (PMID 37603493) · https://arxiv.org/abs/2309.08223
**Metadata verified:** Title, author list, venue, DOI, and PMID confirmed via IEEE Xplore (doc 10225542), PubMed (37603493), arXiv, and HAL (hal-04207382).
**Relevance score:** 5 / 10
*(Not venous-specific; an accuracy-enabling method for optoacoustic sO₂ that is directly transferable to venous imaging.)*
**Note:** Never previously entered.

**Novelty:** Addresses two of the largest error sources in in-vivo optoacoustic sO₂: **physiological/probe motion** and **spectral unmixing inaccuracy**. Proposes a motion-rejection scheme combined with an improved unmixing pipeline, validated in vivo, to recover more accurate sO₂ estimates than standard linear unmixing under realistic movement.

**Integration insights:** Motion is a first-order obstacle for any *venous* optoacoustic measurement at the neck or limb — respiration, swallowing, and arterial pulsation all corrupt multi-wavelength frames that must be co-registered for sO₂. This method is complementary to the deep-learning fluence-free approaches captured in prior scans (Hybrid-Net, Shang et al. 2025, prior scan 2.4; SPOI-AE, Ter Martirosyan et al. 2026, prior scan 2.3): those fix the *fluence/inversion* problem, this fixes the *motion/acquisition* problem. A clinical venous-oximetry PA pipeline plausibly needs all three (motion rejection → fluence-aware inversion → spectral-coloring correction).

---

### Paper 2.4
**Title:** Hyperspectral Imaging for Non-Invasive Blood Oxygen Saturation Assessment
**Authors:** Group incl. School of Information Science and Technology, Fudan University (full author list not resolved from indexing — flagged)
**Year:** 2024 (February)
**Venue:** *Photodiagnosis and Photodynamic Therapy* (Elsevier); article in *Optical and Quantum Electronics*-adjacent indexing — see note
**Link / DOI:** https://doi.org/10.1016/j.pdpdt.2024.104003 (PMID 38336148) · https://www.sciencedirect.com/science/article/pii/S1572100024000425
**Metadata verified:** Title, year, DOI, PMID, and lead affiliation (Fudan University) confirmed via PubMed and ScienceDirect. **Full author list and exact volume/page not resolved — flagged; the ScienceDirect PII (S1572100024…) corresponds to *Photodiagnosis and Photodynamic Therapy*.**
**Relevance score:** 5 / 10
*(Tissue/vascular HSI sO₂; not venous-isolated, but the diffuse-reflectance HSI approach can map veins and is transferable to venous oximetry.)*
**Note:** Never previously entered; complements but does not duplicate the transmissive HSI paper of prior scan 2.1 (Liu et al. 2025) — this is a reflectance/illumination-engineering system.

**Novelty:** Presents an HSI system with **active sequential bandpass illumination integrated into conventional optical instruments**, capturing concurrent spatial+spectral data for non-invasive sO₂ mapping of subcutaneous vasculature (arteries, capillaries, veins), with calibration benchmarked against pulse oximetry.

**Integration insights:** Reflectance HSI is the widely deployable counterpart to the higher-precision transmissive HSI of prior scan 2.1; the illumination-engineering angle (sequential bandpass, retrofittable to existing instruments) lowers the hardware barrier to wide-field venous mapping. Like SFDI (prior scan 2.5), HSI samples a venous-weighted tissue bed; pairing it with a venous-occlusion or APG modulation (Papers 1.2, 1.5) would push it from tissue-StO₂ toward venous-selective sO₂. The unresolved author/volume metadata is flagged and should be reconfirmed before citing formally.

---

### Paper 2.5
**Title:** Clinical Validation of Deep Learning for Real-Time Tissue Oxygenation Estimation Using Spectral Imaging
**Authors:** Jens De Winne, Siri Willems, Siri Luthman, Danilo Babin, Hiep Luong, Wim Ceelen
**Year:** 2025
**Venue:** *MICCAI 2025* (provisionally accepted); arXiv:2505.18010; Springer LNCS chapter 10.1007/978-3-032-05127-1_12
**Link / DOI:** https://arxiv.org/abs/2505.18010 · https://doi.org/10.1007/978-3-032-05127-1_12
**Metadata verified:** Title, full author list, arXiv ID, and MICCAI 2025 acceptance confirmed via arXiv and Springer LNCS listing.
**Relevance score:** 5 / 10
*(Tissue-level StO₂ via spectral imaging; not venous-specific, but a recent, clinically validated DL inversion pipeline directly portable to venous imaging.)*
**Note:** Never previously entered; the most recent (2025) Topic 2 method found this run.

**Novelty:** Trains a fully connected network and a CNN on **Monte-Carlo-simulated spectra** for real-time tissue-oxygenation estimation from intraoperative spectral imaging, and adds a **domain-adversarial training** step to bridge the simulation-to-real (sim2real) gap. Clinically, the DL estimates show **higher correlation with capillary lactate** (an ischemia ground truth) than traditional linear unmixing.

**Integration insights:** This is the same Monte-Carlo-trained-DNN inversion paradigm as Sun et al. 2024's jugular-NIRS pipeline (prior scan 1.2), now validated against a clinical ischemia biomarker rather than a co-oximetry reference. The **domain-adversarial sim2real** technique is the key transferable contribution: every Monte-Carlo-trained venous-oximetry model (NIRS, PA, HSI) faces the same simulation-to-patient distribution shift, and adversarial domain adaptation is a concrete remedy. Validation against lactate also points to the clinical *why* — tissue/venous oxygenation as a perfusion-adequacy and ischemia readout, the same rationale (sepsis, shock, oxygen extraction) motivating the e-tattoo work in Topic 1.

---

## Cross-Topic Synthesis

### What is genuinely new this run
The defining find is the **UT Austin optical e-tattoo lineage** (Papers 1.1, 1.3, + Jan-2025 patent), which is squarely venous-specific and was absent from both prior scans. It reframes the venous-oximetry problem as a **conformal, wearable, vessel-pair** sensing problem and names the central obstacle — **arterio-venous optical crosstalk** — explicitly. This complements, rather than competes with, the depth-resolved vessel-specific approaches (photoacoustic IJV oximetry; retinal vis-OCT) captured previously.

### Convergent themes (updated)

1. **"Active modulation" is the recurring venous-selectivity trick.** Independently, the Canterbury APG method (1.2), the external-stimulation method (1.5), the NIRS/optoacoustic venous-occlusion tests (prior scan 1.5; Paper 2.2), and the e-tattoo's pulsatile-venous extraction (1.1) all impose or exploit a *known venous modulation* to separate the venous compartment from arterial and tissue backgrounds. This is the single most consistent idea across two decades of venous-oximetry work and the conceptual bridge from tissue-StO₂ to true SvO₂.

2. **Spectral-confound removal is the shared accuracy frontier across modalities.** ADS-vis-OCT's spectral-contaminant removal (2.1), PA spectral-coloring correction (prior scan 2.2), and improved optoacoustic unmixing (2.3) are the same battle fought in three modalities: isolate the oxygen-dependent spectral signal from tissue-induced distortion. ADS-vis-OCT's human accuracy (RMSE 2.1%, venous repeatability 2.3%) is the precision bar the others target.

3. **Monte-Carlo-trained DNNs + sim2real adaptation are becoming the standard inversion stack.** Sun et al. 2024 (jugular NIRS, prior scan), Karlas-style MSOT, and the MICCAI-2025 domain-adversarial spectral-imaging model (2.5) all train on simulated photon transport and must close the simulation-to-patient gap. Domain-adversarial training (2.5) is the newest concrete tool for that gap and is portable to every venous-oximetry modality.

4. **The neck remains the highest-value, hardest target.** Deep-neck e-tattoo PPG (1.3), jugular reflectance/NIRS (prior scan 1.1, 1.3), and photoacoustic IJV oximetry (prior scan 2.1) all converge on IJV/ScvO₂. Wearable optics now reach the depth; the open problems are crosstalk (1.1), motion (2.3), and absolute calibration vs. co-oximetry (1.4).

### Honest gaps and open questions
- **No new 2026 venous-specific optical paper appeared today.** The recent-publication frontier was already harvested by the 2026-06-10/11 scans; today's value is in surfacing previously-missed venous-specific methods and the e-tattoo patent.
- **Validation scale is still the field's weakest link.** The largest *optical* venous validation remains ~79 patients (Jeleff 2023); peripheral PPG validations (1.4) and the e-tattoo (1.1) are small-n. The 628-patient CMR iSvO₂ benchmark (prior scan 1.1) is unmatched optically.
- **Crosstalk has a named problem but no settled solution.** Paper 1.1 characterises arterio-venous crosstalk and proposes spatial filtering; whether geometry/spatial filtering alone (vs. active modulation or model-based unmixing) suffices for clinical-grade SvO₂ is unresolved.
- **Metadata to reconfirm:** Paper 2.4 (full author list / exact volume) and Paper 1.5 (author given names beyond the first) are flagged as not fully resolved and should be reverified before formal citation.
