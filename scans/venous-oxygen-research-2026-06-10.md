# Venous Oxygen Research Scan — 2026-06-10

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.  
**Prior scans in this repository:** None — first run; no exclusions applied.  
**Note on sparseness:** Genuinely venous-specific non-invasive optical work remains a niche, low-volume field. Relevance scores are calibrated strictly against the goal of *non-invasive venous (not arterial) blood oxygen measurement via optical means*. Tissue-level StO₂ papers (which sample a mixed arterial/venous bed) are included where they offer a credible indirect path to venous-specific values; this is flagged in each entry.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

### Paper 1.1
**Title:** Estimation of Venous Oxygen Saturation Through Non-Invasive Optical Sensing at the Jugular Veins  
**Authors:** Jordan F. Hill, Jake Campbell, J. Geoffrey Chase, Christopher G. Pretty  
**Year:** 2024  
**Venue:** *Current Directions in Biomedical Engineering*, vol. 10, no. 4, pp. 295–298 (De Gruyter)  
**Link / DOI:** https://doi.org/10.1515/cdbme-2024-2072  
**Metadata verified:** Title, authors, year, journal, and DOI confirmed via De Gruyter listing and ResearchGate PDF (direct page fetch blocked; metadata cross-checked from two sources).  
**Relevance score:** 9 / 10

**Novelty:** Proof-of-concept pulse-oximeter-style reflectance sensor worn over the external jugular vein (EJV) to measure SvO₂ directly and continuously, without cuff or venous occlusion. Tested in three healthy subjects, correctly identified the EJV waveform and returned SvO₂ estimates in the expected 60–90% healthy range. This is one of very few human studies where the sensor is positioned *over a vein* rather than at a tissue bed.

**Integration insights:** The EJV is relatively superficial and lacks the arterial-pulse-only signal that confounds conventional pulse oximetry, making it an attractive site for venous-specific sensing. The small sample size (n = 3) and proof-of-concept scope mean clinical accuracy is unvalidated, but the hardware approach — reflectance PPG at a known venous landmark — is directly scalable. Pairing this sensor geometry with photoacoustic or structured-light illumination (Topics 2) could improve depth specificity and eliminate residual arterial contamination. Directly relevant to continuous, wearable venous monitoring.

---

### Paper 1.2
**Title:** Quantifying Changes in Oxygen Saturation of the Internal Jugular Vein In Vivo Using Deep Neural Networks and Subject-Specific Three-Dimensional Monte Carlo Models  
**Authors:** Chin-Hsuan Sun, Hao-Wei Lee, Ya-Hua Tsai, Jia-Rong Luo, Kung-Bin Sung  
**Year:** 2024  
**Venue:** *Optics Letters*, vol. 49, no. 10, pp. 2669–2672  
**Link / DOI:** https://opg.optica.org/ol/abstract.cfm?uri=ol-49-10-2669  
**Metadata verified:** Title, authors, volume/issue/pages, and Optica URL confirmed via search; DOI as canonical Optica path. Related SPIE proceedings version confirmed at DOI 10.1117/12.3002736.  
**Relevance score:** 9 / 10

**Novelty:** Multi-channel NIRS placed over the neck, combined with subject-specific 3-D Monte Carlo optical simulations (built from structural MRI/anatomy) and a deep neural network (DNN) trained on the simulation data, to quantify *changes* in SijvO₂ non-invasively and continuously. The Monte Carlo personalisation step substantially improves the accuracy over generic tissue models. Demonstrated in vivo.

**Integration insights:** The subject-specific simulation pipeline is the key innovation: it directly addresses the long-standing critique that simple Beer-Lambert NIRS models cannot separate IJV signal from overlying neck tissue. The DNN acts as a fast inversion layer. Combining this approach with photoacoustic excitation (rather than pure NIRS) could yield absolute sO₂ rather than change tracking. Highly complementary to the IJV photoacoustic work (Paper 2.1).

---

### Paper 1.3
**Title:** New Noninvasive Method for the Assessment of Central Venous Oxygen Saturations in Critically Ill Patients  
**Authors:** Alexandre Jeleff, Noémie Suh, Álmos Schranc, John Diaper, Karim Bendjelid, Eduardo Schiffer  
**Year:** 2023  
**Venue:** *Journal of Cardiothoracic and Vascular Anesthesia*, 2023 (PubMed ID 37827917)  
**Link / DOI:** https://www.sciencedirect.com/science/article/pii/S1053077023007826  
**Metadata verified:** Title, authors, journal, PubMed ID confirmed via PubMed listing and JCVA publisher page (direct fetch blocked; cross-checked via two search results). Exact volume/issue not confirmed — *flagged.*  
**Relevance score:** 8 / 10

**Novelty:** Clinical validation of the Mespere VO100 device — a commercial NIRS sensor placed over the external jugular vein — against invasive ScvO₂ from blood gas in 79 ICU patients (36 COVID-19 patients requiring ventilation, 43 post-liver-transplant). Strong linear correlation between SjvO₂ (NIRS) and ScvO₂ (lab) demonstrated in real-world critical care. This is the largest single-centre human validation of a dedicated non-invasive jugular venous oximetry device published to date.

**Integration insights:** Establishes clinical feasibility of non-invasive jugular NIRS for ScvO₂ monitoring in the ICU — the most direct clinical analogue of invasive central venous monitoring. The Mespere VO100 is effectively a commercialised implementation of the approach described in Paper 1.1 but at a larger scale. Key limitation is that the NIRS signal integrates tissue, arterial, and venous compartments; correction for arterial contamination (as in Paper 1.2) would improve specificity. Forms the clinical benchmark against which future photoacoustic (Paper 2.1) or wearable approaches should be validated.

---

### Paper 1.4
**Title:** Noninvasive Tracking of Mixed Venous Oxygen Saturation via Near-Infrared Spectroscopy Cerebral Oximetry: A Retrospective Observational Study  
**Authors:** Chahyun Oh, Sujin Baek, Soomin Lee, Man-Shik Shim, Sung Joon Han, Yoon-Hee Kim, Jeong Yeon Lee, Yunseo Ku, Boohwi Hong  
**Year:** 2023  
**Venue:** *Scientific Reports*, December 2023  
**Link / DOI:** https://doi.org/10.1038/s41598-023-49078-1  
**Metadata verified:** Title, full author list, journal, DOI confirmed via Nature.com and DOAJ listings.  
**Relevance score:** 7 / 10

**Novelty:** Retrospective analysis of simultaneous intraoperative rScO₂ (INVOS 5100C or Masimo O3 cerebral NIRS) and SvO₂ from pulmonary artery catheter during off-pump cardiac surgery. Demonstrates that trends — though not absolute values — in SvO₂ can be tracked non-invasively using commercially available cerebral oximeters. Head-to-head comparison of two NIRS platforms. *Note: this is tissue-level rScO₂ used as a surrogate for SvO₂, not a direct venous measurement.*

**Integration insights:** The study anchors the practical question: how close can cerebral NIRS get to true mixed SvO₂? The answer is "trend monitoring, not interchangeable absolute values." This gap motivates the more targeted approaches in Papers 1.1–1.3. For the optical imaging community, this paper delineates the accuracy ceiling of generic NIRS before vessel-specific methods (PAVT, photoacoustic, vis-OCT) become necessary.

---

### Paper 1.5
**Title:** Can Central-Venous Oxygen Saturation Be Estimated from Tissue Oxygen Saturation During a Venous Occlusion Test?  
**Authors:** Claudio da Silva Zachia Alan, Alexandre Augusto Pinto Lima, Jan Bakker, Gilberto Friedman  
**Year:** 2022  
**Venue:** *Critical Care Science* (formerly RBTI), 2022  
**Link / DOI:** https://doi.org/10.5935/0103-507X.20220023-en  
**Metadata verified:** Title, authors, journal, DOI confirmed via PMC9354100 and Critical Care Science publisher page listings.  
**Relevance score:** 7 / 10  
*(Tissue-level StO₂, not direct SvO₂; included as best NIRS venous-occlusion surrogate methodology available.)*

**Novelty:** In 22 ICU patients, shows that thenar StO₂ measured by InSpectra NIRS during a standardised venous occlusion test (cuff inflation ≥ 100 s) equilibrates to ScvO₂ values (R² 0.63–0.67 depending on probe spacing). Proposes the equilibration time-point as an implicit venous saturation readout. A procedural rather than continuous method, but fully non-invasive.

**Integration insights:** The venous occlusion test creates a momentary stagnant-blood window in which NIRS-measured StO₂ converges toward true venous sO₂ — effectively making the tissue bed behave like a pure venous reservoir. This same principle (controlled occlusion + optical readout) could be combined with photoacoustic or hyperspectral imaging for more accurate, depth-resolved venous sO₂ in larger vessels. The 100-second equilibration time also constrains the minimum duty cycle for any intermittent non-invasive venous oximetry protocol.

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

### Paper 2.1
**Title:** Noninvasive In Vivo Photoacoustic Measurement of Internal Jugular Venous Oxygenation in Humans  
**Authors:** Alejandro Garcia-Uribe, Todd N. Erpelding, Haixin Ke, Kavya Narayana Reddy, Anshuman Sharma, Lihong V. Wang  
**Year:** 2023  
**Venue:** arXiv preprint arXiv:2303.10775 (March 2023) — **no peer-reviewed journal publication confirmed; flagged as preprint.**  
**Link:** https://arxiv.org/abs/2303.10775  
**Metadata verified:** Title, full authors, arXiv ID, and submission date confirmed via ADS and arXiv search results. Publisher venue could not be confirmed beyond arXiv.  
**Relevance score:** 10 / 10

**Novelty:** First reported in-vivo human demonstration of two-wavelength photoacoustic + ultrasound imaging to measure blood oxygen saturation directly in the internal jugular vein (IJV). The IJV was located under real-time ultrasound guidance; dual-wavelength (660/805 nm) PA images yielded average sijvO₂ = 72 ± 7% across subjects — consistent with invasive reference values. Both transverse and longitudinal scan planes were demonstrated. Unlike NIRS, the technique is depth-resolved and vessel-specific with no arterial contamination.

**Integration insights:** This is the most direct proof-of-concept paper for the core research goal: non-invasive optical measurement of true venous (not tissue) oxygen saturation in humans. The co-registration with ultrasound addresses the problem of venous localisation that defeats surface NIRS. Key challenges before clinical translation: real-time frame rates, safe laser fluence at the neck, and co-registered guidance in ICU settings. Directly motivates the deep-learning PA work (Paper 2.4) which could replace hand-tuned spectral unmixing, and the PACT flow work (Paper 2.2) which extends the technique to haemodynamic mapping.

---

### Paper 2.2
**Title:** Oxygenation Heterogeneity Facilitates Spatiotemporal Flow Pattern Visualization Inside Human Blood Vessels Using Photoacoustic Computed Tomography  
**Authors:** Siying Kong, Hongzhi Zuo, Chuhua Wu, Ming-Yuan Liu, Cheng Ma  
**Year:** 2024  
**Venue:** *Biomedical Optics Express*, vol. 15, no. 5, pp. 2741–2752, May 2024  
**Link / DOI:** https://doi.org/10.1364/BOE.518895  
**Metadata verified:** Title, authors, journal, volume/issue/pages, DOI confirmed via Optica publisher listing and ResearchGate.  
**Relevance score:** 9 / 10

**Novelty:** Uses multi-wavelength PACT to exploit naturally occurring oxygenation heterogeneity *within* a flowing human vein as an intrinsic tracer. For the first time, recovered the parabolic laminar-flow velocity profile inside a deep vein in real time and in vivo, using no exogenous contrast. Also demonstrates dynamic sO₂ mapping during exercise (fist clenching) as deoxygenated blood enters major vessels.

**Integration insights:** The innovation is using natural sO₂ heterogeneity as a flow tracer — a dual-purpose readout giving both haemodynamics and oxygenation simultaneously. Affirms that PACT can quantify venous oxygenation in vessels more than a few mm below the skin. The exercise paradigm parallels the venous occlusion test (Paper 1.5): both create controlled physiological perturbations to boost venous signal. Directly demonstrates what multi-wavelength PA can reveal in a vein, making it a key reference point for quantitative venous oximetry development.

---

### Paper 2.3
**Title:** Photoacoustic Vector Tomography for Deep Haemodynamic Imaging  
**Authors:** Yang Zhang, Joshua Olick-Gibson, Anjul Khadria, Lihong V. Wang  
**Year:** 2024 (published online 30 November 2023)  
**Venue:** *Nature Biomedical Engineering*, vol. 8, pp. 701–711, 2024  
**Link / DOI:** https://doi.org/10.1038/s41551-023-01148-5  
**Metadata verified:** Title, authors, journal, volume/pages, DOI confirmed via Nature and Caltech library feed.  
**Relevance score:** 7 / 10

**Novelty:** Photoacoustic vector tomography (PAVT) breaks through the optical diffusion limit (≫1 mm) to image blood flow in veins more than 5 mm deep in the hands and arms of healthy volunteers without contrast. Compiles successive wide-field single-shot PA images to estimate pixel-wise flow velocity *and direction* deep in tissue. The same platform simultaneously provides haemoglobin concentration and, with multi-wavelength extension, sO₂. *Primary focus is haemodynamics, not oximetry, but the platform directly supports venous sO₂.*

**Integration insights:** PAVT establishes that PA imaging can reliably reach clinically relevant venous depths (> 5 mm) and characterise haemodynamics. The next step — adding spectral multiplexing — would yield deep venous sO₂ with the same system. As a Wang-lab paper, it is the natural extension of Paper 2.1 (IJV oxygenation) to a fully tomographic, high-depth, multi-parameter platform. Relevant for monitoring deep veins (e.g. femoral, subclavian) in future clinical systems.

---

### Paper 2.4
**Title:** Deep Learning-Driven Quantitative Spectroscopic Photoacoustic Imaging for Segmentation and Oxygen Saturation Estimation  
**Authors:** Ruibo Shang, Sidhartha Jandhyala, Yujia Wu, Kevin Hoffer-Hawlik, Austin Van Namen, Matthew O'Donnell, Geoffrey P. Luke  
**Year:** 2025  
**Venue:** arXiv preprint arXiv:2512.15394 (December 17, 2025) — **preprint; journal submission status unverified.**  
**Link:** https://arxiv.org/abs/2512.15394  
**Metadata verified:** Title, authors, arXiv ID, submission date confirmed via arXiv, ADS, and ResearchGate listings.  
**Relevance score:** 7 / 10

**Novelty:** Introduces Hybrid-Net, a convolutional deep neural network that *jointly* estimates blood sO₂ and segments vessels from two-wavelength spectroscopic PA data without explicit fluence estimation. In simulations across 0–35 dB noise, achieves segmentation accuracy ≥ 0.978 and sO₂ MSE ≤ 0.048; in phantom experiments, sO₂ MSE = 0.003. Avoids the ill-posed optical fluence inversion that limits classical spectral unmixing in deep tissue. *Not venous-specific, but the methodology is prerequisite for accurate venous sO₂ from PA.*

**Integration insights:** Accurate spectroscopic PA oximetry has been blocked by the fluence problem: the PA signal depends on both sO₂ and local optical fluence, which is unknown deep in tissue. Hybrid-Net tackles this by learning the combined problem end-to-end. The dual-output (segment + sO₂) design is directly applicable to IJV imaging pipelines (Paper 2.1, 2.2): after vessel segmentation, the sO₂ estimate is automatically localised to the vein. Integration with subject-specific Monte Carlo fluence models (as in Paper 1.2) is a natural next step for further accuracy improvement.

---

### Paper 2.5
**Title:** Deep-Learning–Enabled Spatial Frequency Domain Imaging of the Spatiotemporal Dynamics of Skin Physiology  
**Authors:** Guowu Huang, Yansen Hu, Weihao Lin, Chenfan Shen, Jianmin Yang, Zhineng Xie, Yifan Ge, Xin Jin, Xiafei Qian, Min Xu  
**Year:** 2025  
**Venue:** *Journal of Biomedical Optics*, vol. 30, no. 4, article 046008, April 2025  
**Link / DOI:** https://doi.org/10.1117/1.JBO.30.4.046008  
**Metadata verified:** Title, authors, journal, volume/issue/article number, DOI confirmed via SPIE Digital Library and PMC12014942.  
**Relevance score:** 6 / 10  
*(Tissue-level StO₂, includes venous compartment; not vessel-specific.)*

**Novelty:** SFDI-net — a CNN architecture — replaces the multi-image iterative fitting in conventional SFDI, enabling real-time, large field-of-view maps of tissue optical properties, oxygen saturation, hemoglobin concentration, melanin, scattering, surface roughness, and epidermal thickness from a single spatial-frequency illumination sequence. A 4× speedup over traditional SFDI fitting with no accuracy loss. Demonstrated on human skin.

**Integration insights:** SFDI inherently probes a mixed tissue bed (≈70–75% venous by blood volume in skin), so the StO₂ it measures is dominated by venous oxygenation — making it one of the more practically venous-weighted widefield optical techniques. The real-time capability enabled by SFDI-net makes it tractable for dynamic monitoring scenarios. The venous occlusion protocol (Paper 1.5) applied under SFDI imaging would create a pure-venous readout, combining SFDI's spatial mapping with a controlled venous window. Complementary to PA for superficial venous oxygenation mapping (e.g. skin flap viability, wound care).

---

## Cross-Topic Synthesis

### Convergent themes

**1. The IJV as the primary near-term target.** Papers 1.1–1.3 and 2.1 all focus on the jugular vein. The IJV is the clinical gold standard for cerebral venous oxygenation monitoring and is anatomically accessible for surface sensing. The 2024 NIRS + DNN paper (1.2) and the 2023 photoacoustic paper (2.1) each tackle the same vein with complementary modalities — NIRS for rapid continuous change tracking, photoacoustics for absolute vessel-specific sO₂. A hybrid system combining NIRS trend monitoring with periodic PA spot-checks of absolute sO₂ would be clinically powerful.

**2. Deep learning as the enabling layer.** Papers 1.2, 2.4, and 2.5 all use neural networks to bridge the gap between raw optical signals and quantitative oxygenation values. The shared bottleneck — inversion of the photon transport problem — is being addressed with DNNs trained on Monte Carlo simulations or physics-based synthetics. The Monte Carlo personalisation in Paper 1.2 and the fluence-free sO₂ estimation in Paper 2.4 are complementary solutions to the same underdetermined inversion.

**3. Oxygenation heterogeneity as an asset.** Paper 2.2 reframes a challenge (heterogeneous sO₂ in flowing blood) as a contrast mechanism for flow imaging. This is the photoacoustic analogue of Doppler velocimetry and suggests that dynamic venous sO₂ imaging could provide both velocity and oxygenation maps simultaneously — a richer haemodynamic picture than either alone.

**4. The arterial contamination problem.** Papers 1.4 and 1.5 both document the core limitation of tissue-level NIRS as a venous surrogate: arterial blood (which constitutes 25–30% of tissue blood volume) systematically biases the readout toward higher sO₂. Vessel-specific modalities (PA, vis-OCT for retinal veins) sidestep this entirely. Until non-invasive vessel-specific PA is mature for routine use, venous occlusion protocols (Paper 1.5) offer a procedural workaround.

**5. Wearable NIRS reaching for venous specificity.** A May 2026 review (*J. Phys.: Photonics*, DOI 10.1088/2515-7647/ae6ae4) documents rapid miniaturisation of NIRS hardware — fully wearable, wireless, battery-powered systems — that now rival clinical-grade benchtop devices. As this hardware platform matures, adding venous-selective algorithms (e.g., the jugular DNN pipeline from Paper 1.2 or the jugular sensor geometry from Paper 1.1) becomes increasingly practical for ambulatory or remote monitoring applications. This wearable trajectory is perhaps the highest-leverage near-term path to clinical deployment.

### Gaps and open questions

- **Absolute accuracy in humans:** Papers 2.1–2.3 demonstrate feasibility but head-to-head accuracy against co-oximetry in large human cohorts is missing. Clinical validation equivalent to Paper 1.3 (79 ICU patients) does not yet exist for photoacoustic venous oximetry.
- **Real-time deep-tissue PA oximetry:** The fluence problem limits all PA sO₂ approaches beyond a few mm depth. Paper 2.4 (Hybrid-Net) attacks this computationally; hardware solutions (multi-angle illumination, ultrasound-guided PA) are concurrently maturing.
- **Venous-specific SFDI / hyperspectral:** Neither SFDI (Paper 2.5) nor hyperspectral imaging has been demonstrated with vessel-specific venous isolation in a deep vein. The retinal vein analogues (vis-OCT) show it is tractable in accessible superficial vessels, but extrapolation to systemic deep veins remains an open challenge.
- **Wearable PA:** Photoacoustic imaging currently requires bench-top lasers and ultrasound transducer arrays. A wearable PA venous oximeter does not yet exist but is a logical convergence target combining the PA specificity of Paper 2.1 with the form-factor trajectory documented in the 2026 NIRS review.
