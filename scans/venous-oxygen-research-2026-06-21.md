# Venous Oxygen Research Scan — 2026-06-21

**Scan scope:** Non-invasive venous blood oxygen monitoring + optical imaging techniques for venous oxygen saturation.
**Prior scans in this repository:** 2026-06-10 (10 papers), 2026-06-11 (10 papers), 2026-06-14 (≈7 entries), 2026-06-16 (2 entries), 2026-06-17 (4 entries), 2026-06-18 (3 entries), 2026-06-19 (1 entry). Every paper entered in those seven scans — plus all items in their "honorable mentions" / "reviewed and excluded" / "previously surfaced" sections — is excluded here unless a genuinely newer version or finding warrants re-entry. None did.
**Search window:** This is the **eighth scan** in the series, run **two days** after 2026-06-19 (no scan on 06-20). Emphasis on work published or first-surfacing after 2026-06-19, with a fallback to the best-available venous-specific work **not yet catalogued** anywhere in this repository. Sources searched today: PubMed/PMC, arXiv, bioRxiv/medRxiv, Optica (Biomed. Opt. Express, Optics Letters, Applied Optics), SPIE / *J. Biomed. Opt.* / *Neurophotonics*, *Photoacoustics*, Springer / Graefe's Archive / *BioMed. Eng. OnLine*, Frontiers, Nature, ScienceDirect, MDPI, De Gruyter Brill, IOVS/ARVO, ClinicalTrials.gov, ResearchGate, Semantic Scholar.
**Verification caveat:** As in every prior scan, essentially all PMC/PubMed, Springer, SPIE, Optica-fulltext, bioRxiv/arXiv and Frontiers pages returned **HTTP 403** to direct fetches in this environment. Every reference below was cross-checked across **at least two independent search-index sources**; per-item notes state what was confirmed and what could not be read directly on a publisher page.

---

## ⚠️ Read this first — honest sparseness report

This is the **eighth scan** of a genuinely low-volume niche, run two days after 06-19. As in every preceding single-day cycle, **no brand-new (post-2026-06-19) venous-specific paper surfaced today** — for either topic. Rather than pad with arterial-only SpO₂ work, this scan does the honest thing and reports an empty cycle for new entries, while recording what searches re-returned, plus one previously-uncatalogued *context* item and the standing trial/review leads.

- **Topic 1 (systemic non-invasive venous monitoring): empty for new entries.** Every result returned was already catalogued in a prior scan (jugular NIRS, Mespere VO100, spiroximetry, the venous-occlusion test, the MRI references, the 2016/2017 venous-modulation methods, the artificial-venous-pulse PPG family, the e-tattoo, hDOS). No new publication appeared. One additional NIRS-for-SjvO₂ *trial* (NCT04624009) surfaced and is recorded as a lead alongside the standing trial set.
- **Topic 2 (optical imaging): empty for new entries.** No genuinely new (post-2026-06-19) photoacoustic, NIRS-imaging, DOT, SFDI, HSI, or vis-OCT primary study surfaced. The strongest recent items (Gu et al. vis-OCT, the HSI retina system, Hybrid-Net, the venous-range sulfate phantoms, the IJV-PA proof-of-concept, the Frontiers carotid-stenosis retinal-oximetry study) are all already in the repository. One previously-uncatalogued **2020** retinal-oximetry-in-pregnancy study and one **2025** OCT-angiography preeclampsia review are noted as context only (neither is new; the latter is flow, not oximetry).

The standing picture is unchanged from 06-14 → 06-19: **MRI is the absolute-reference venous calibrator, the retina is the proving ground for vessel-specific optical venous saturation, the venous-occlusion test is the practical surrogate, and human deep-vein optical sO₂ at clinical scale remains the unfilled prize.** No padding was added to reach five entries per topic, per the scan's honesty mandate.

---

## Topic 1 — Non-Invasive Monitoring of Venous Blood Oxygen (SvO₂ / ScvO₂ / Peripheral Venous Oxygenation)

> **Sparseness flag — no new entries this cycle.** No venous-specific non-invasive *monitoring* paper published or first-surfacing after 2026-06-19 met the bar. Searches re-returned only (a) papers already entered in prior scans and (b) pre-2024 methodological references already noted as leads. Topic 1 is therefore reported honestly as empty for new publications this cycle — the sixth straight short-cycle scan with no Topic-1 publication.

**Previously surfaced — standing venous-monitoring references (NOT re-entered):**
- **Hill, Campbell, Chase & Pretty 2024**, optical SvO₂ sensing at the external jugular vein — *Curr. Dir. Biomed. Eng.* 10(4):295–298 (DOI 10.1515/cdbme-2024-2072). Prior scan **2026-06-10 §1.1**. (Re-confirmed today via De Gruyter Brill + ResearchGate.)
- **Sun et al. 2024**, IJV SijvO₂ via NIRS + subject-specific Monte Carlo + DNN — *Optics Letters* 49(10):2669–2672. Prior scan **2026-06-10 §1.2**.
- **Jeleff et al. 2023**, Mespere VO100 jugular NIRS vs invasive ScvO₂, 79 ICU patients — *J. Cardiothorac. Vasc. Anesth.* (PMID 37827917). Prior scan **2026-06-10 §1.3**. (Re-confirmed today via JCVA/ScienceDirect.)
- **Oh et al. 2023**, cerebral-NIRS surrogate tracking of mixed SvO₂ — *Sci. Rep.* (DOI 10.1038/s41598-023-49078-1). Prior scan **2026-06-10 §1.4**.
- **Zachia Alan et al. 2022**, thenar StO₂ → ScvO₂ during the venous-occlusion test — *Critical Care Science* (DOI 10.5935/0103-507X.20220023-en). Prior scan **2026-06-10 §1.5**.
- **McDiarmid et al. 2026**, cardiac-MRI T₂ iSvO₂, 628-patient HF cohort — *JACC: Advances* 5(1):102484. Prior scan **2026-06-11 §1.1**.
- **Skow et al. 2025**, MRI susceptometry-based venous oximetry during exercise — *Am. J. Physiol. Heart Circ. Physiol.* 328(6) (DOI 10.1152/ajpheart.00134.2025). Prior scan **2026-06-14 §1.1**.
- **Lahade et al. 2026**, wearable FD-NIRS (ASIC), forearm-occlusion arterio-venous transition — *Biomed. Opt. Express* 17(2):555–571 (DOI 10.1364/BOE.585068). Prior scan **2026-06-11 §1.2**.
- **Tan et al. 2023**, wearable arterial+venous optical e-tattoo (EMBC 2023, PMID 38083768). Prior scan **2026-06-17 §1.1**.
- **"hDOS" 2025** (Durduran group), automated hybrid diffuse-optical platform built around the venous-occlusion test — *J. Biomed. Opt.* 2025 / medRxiv 2025.06.03.25328859. Prior scan **2026-06-17 §1.2**.
- **Zhang et al. 2016**, light-absorption SvO₂ via induced venous fluctuation (RMSE 5.31, r 0.72 vs invasive) — *BioMed. Eng. OnLine* 15 (DOI 10.1186/s12938-016-0208-8; PMC4952148). Prior scan **2026-06-17 §1.3**. (Re-confirmed today via PMC.)
- **Zhang et al. 2017**, proof-of-concept non-invasive peripheral SvO₂ — *BioMed. Eng. OnLine* 16 (DOI 10.1186/s12938-017-0351-x; PMC5437414). Prior scan 2026-06-17 honorable mention.
- **Peripheral-venous-saturation-vs-co-oximetry validation** (PMC5655584, *J. Clin. Monit. Comput.* 2016/2017, PMID 27873173) and the **artificial-venous-pulse PPG** family. Re-surfaced today; same Zhang/peripheral-PPG lineage already catalogued — not re-entered.

**Re-confirmed methodological leads (still no new 2025–2026 publication):** near-infrared "spiroximetry" (respiration-frequency-filtered venous NIRS for cerebral SvO₂; substantive papers remain 2002/2013/2014, PMC4126245 / PMID 24439329); dynamic low-pressure venous-filling NIRS (Yoxall/Weindling lineage, PMID 10938779); NIRS-estimated peripheral venous saturation in newborns vs co-oximetry (PMID 12119534); jugular transcutaneous NIRS for ScvO₂ in pediatric cardiac surgery (PMC7491293). All venous-specific in principle; carried forward as leads, not entered.

**Standing trial leads (carried forward, no results yet):**
- **NCT01891188** — *"Using NIRS to Noninvasively Evaluate Hepatic Venous Saturation"* (hepatic regional StO₂ vs SvHO₂); record updated Jan 2026. First surfaced 2026-06-18; no results paper.
- **NCT06511999** — *"Continuous Jugular Venous Oxygen Saturation (SjO₂) Measurement After Cardiac Arrest"* (U. Pittsburgh; recruiting; est. completion Dec 2027). First surfaced 2026-06-19; no results yet.
- **NCT05161884** — *"Validation of a Non-invasive Assessment of ScvO₂ by Using MRI"* (MRI-reference validation; consistent with the standing MRI-as-calibrator thesis). No results paper.
- **NCT04624009 (newly recorded this cycle)** — *"Non-Invasive Measurement of SjvO₂ Using Near Infrared Spectroscopy in Critically Ill Patients."* A venous-specific NIRS validation effort (jugular venous saturation vs reference) in the critically ill. Cross-confirmed via ClinicalTrials.gov; **no results publication located** — recorded as a lead, not an entry. (Consistent with the Mespere VO100 / jugular-NIRS thread already catalogued.)

---

## Topic 2 — Optical Imaging Techniques for Non-Invasive Venous Blood Oxygen

> **Sparseness flag — no new entries this cycle.** No genuinely new (post-2026-06-19) primary optical-imaging study reporting venous saturation surfaced. Every venous-attributed photoacoustic / NIRS-imaging / DOT / SFDI / HSI / vis-OCT result returned today maps to work already catalogued in this repository. Topic 2 is reported honestly as empty for new publications this cycle. Two previously-uncatalogued *context* items (one 2020, one 2025) are noted below, but neither is new and neither is a blood-gas-calibrated venous-sO₂ result, so neither is entered.

**Previously surfaced — standing optical venous-imaging references (NOT re-entered):** Garcia-Uribe/Wang IJV-PA proof-of-concept (arXiv:2303.10775; 2026-06-10 §2.1 — re-confirmed today as still the only direct human named-vein photoacoustic oximetry result, sijvO₂ 72 ± 7% in 7 volunteers); Kong et al. PACT intra-vessel flow (2026-06-10 §2.2); Zhang et al. PAVT deep hemodynamics (PMC11136879; 2026-06-10 §2.3); Shang et al. **Hybrid-Net** (2026-06-10 §2.4 — the Dec-2025 arXiv:2512.15394 re-surfaced today; not re-entered); Huang et al. SFDI-net (2026-06-10 §2.5); Liu et al. transmissive HSI single-vessel sO₂ (2026-06-11 §2.1); Feng et al. PA thrombosis oximetry (2026-06-11 §2.2); Ter Martirosyan et al. SPOI-AE (2026-06-11 §2.3); Cam et al. qPACT virtual-imaging framework (2026-06-11 §2.4); Wu et al. vis-OCT review (2026-06-11 §2.5); Basiri et al. SP-SFDI retinal venous αSO₂ (2026-06-14 §2.1); Zafar et al. multispectral PAM (2026-06-14 §2.2); Davenet et al. venous-range sulfate phantoms (arXiv:2512.01458; 2026-06-14 §2.3); *Taiwan J. Ophthalmol.* vis-OCT translation review (2026-06-14 §2.4); Zhang & Wang PA-for-PAD review (2026-06-14 §2.5); BMC Ophthalmology macular venular oximetry (2026-06-16 §2.1); Kirchner/Jaeger/Frenz MI-MS-LSD human accompanying-vein oximetry (2026-06-16 §2.2); Quantitative PACT oximetry review (2026-06-17 §2.1); Gu et al. vis-OCT diseased mouse models with explicit venous-sO₂ finding (2026-06-18 §2.1); JHU/Penn multimodal vis-OCT + PLIM (2026-06-18 §2.2); dual-camera high-resolution HSI retina system (2026-06-18 §2.3); Frontiers carotid-stenosis automated retinal oximetry, A–V difference (2026-06-19 §2.1).

**Honorable mentions (verified to the extent noted, context only, not ranked):**
- *Retinal vessel diameters, flicker-induced retinal vasodilation and retinal oxygen saturation in high- and low-risk pregnancy* — *Acta Ophthalmologica* / PMC8519143, **PMID 33326186 (2020/2021)**. A dynamic-vessel-analyzer study reporting altered retinal **arterial and venous** oxygen saturation in high-risk pregnant women, proposed as a biomarker for pregnancy complications. **Newly surfaced in this scan series but not new (2020); venous in readout** but fundus-DVA vessel-level oximetry, not systemic SvO₂. Recorded as context for the retinal-venous-oximetry thread, not entered. (Cross-confirmed via PubMed + PMC; full text 403.)
- *Evaluating the Chorioretinal Microcirculation in Preeclampsia with OCT-Angiography: A Narrative Literature Review* — *J. Clin. Med.* (MDPI) 14(11):3913, **2025**. Recent and retina-adjacent, but its readouts are OCT-angiography **flow/vessel-density** alterations, **not oxygen saturation** — so noted, not entered.
- *Retinal oximetry: new insights into ocular and systemic diseases* — *Graefe's Archive* 2025, DOI 10.1007/s00417-025-06831-8. Review of fundus/OCT retinal oximetry; relevant background for the retinal venous thread. Carried as context (Springer 403; first noted 2026-06-19).
- *Hyperspectral imaging for non-invasive blood oxygen saturation assessment* — *Sens. Bio-Sens. Res.* 2024 (PMID 38336148) and the custom 400–1000 nm HSI artery/capillary/vein perfusion-mapping system (ScienceDirect S153718912400106X). HSI venous-relevant by modality but **not new and not venous-specific** in reported endpoints. Carried as transferable-technique context.
- *Distribution-informed and wavelength-flexible data-driven photoacoustic oximetry* — arXiv:2403.14863 (2024), PMC11151660. Learned-oximetry method, not venous-specific. Previously noted.

---

## Cross-Topic Synthesis

### What this scan actually establishes
On a short cadence in a low-volume niche, the venous-specific non-invasive oxygen literature **again produced no brand-new publication for either topic** — the correct and expected outcome, now observed for the sixth consecutive short-cycle scan, and itself a signal worth recording. The only forward motion this cycle is bibliographic: **one additional venous-specific NIRS validation *trial* (NCT04624009)** joins the standing trial set, and **two previously-uncatalogued *context* items** (a 2020 pregnancy retinal-oximetry study; a 2025 OCT-angiography preeclampsia review) were logged and correctly excluded — the first because it is old and vessel-level, the second because it measures flow, not saturation.

1. **Topic 1 remains trials-only for forward motion.** Four venous-relevant trials are now tracked — hepatic-vein NIRS (NCT01891188), post-arrest jugular SjO₂ (NCT06511999), MRI-reference ScvO₂ (NCT05161884), and SjvO₂ NIRS in the critically ill (NCT04624009, new this cycle). None has a results publication. The published venous-monitoring corpus is unchanged.
2. **Topic 2 remains anchored in the retina and in a single human-vein PA proof-of-concept.** No new modality result appeared; today's hits (Hybrid-Net, sulfate phantoms, IJV-PA, the HSI/vis-OCT retina systems, the carotid-stenosis retinal study) all map to catalogued work. The 2023 IJV-PA result (arXiv:2303.10775, sijvO₂ 72 ± 7%) is still the only direct human named-vein photoacoustic oximetry result on record.
3. **No new modality breakthrough; the standing thesis holds.** MRI remains the only blood-gas-validated, cohort-scale venous-SvO₂ reference; the retina remains the proving ground for vessel-specific optical venous saturation; the venous-occlusion test remains the practical surrogate.

### Persisting gaps (carried forward, unchanged and still open)
- **No new in-vivo human venous-PA sO₂ result.** Clinical-scale validation of human deep-vein optical/photoacoustic sO₂ still does not exist.
- **The MRI validation-scale gap still dominates.** Two MRI venous-SvO₂ methods (T₂ iSvO₂; susceptometry) are blood-gas-validated at cohort scale, and an MRI-reference ScvO₂ validation trial is registered; no optical method approaches that bar.
- **Vessel-specific venous separation remains proven mainly in the retina (and thin/murine tissue).** Extension of single-vessel venous separation to an accessible systemic vein in thick human tissue is still unshown.
- **Comorbidity / confounding remains an explicitly documented obstacle** (Frontiers carotid-stenosis study, 2026-06-19): retinal venous-saturation / A–V endpoints did not track stenosis severity cleanly because of individual comorbidities — a standing warning for any optical venous-oximetry biomarker program. The 2020 pregnancy study logged today is consistent: venous-saturation shifts are real but population-modified.
- **Topic 1's only forward motion is trials, not papers** — now four registered, none with results.

### Bottom line
A genuinely **empty cycle for new publications**, reported honestly rather than padded. The cycle's value is one new venous-specific NIRS trial lead (NCT04624009) and the logging/exclusion of two context items. Nothing this cycle alters the standing picture: **MRI is the absolute-reference calibrator, the retina is the proving ground (and a documented cautionary case for confounding), the venous-occlusion test is the practical surrogate, and human deep-vein optical sO₂ at clinical scale remains the unfilled prize.** No arterial-only padding was added to reach five entries per topic, per the scan's honesty mandate.
