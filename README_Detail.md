# Fragment Affinity and ADMET Data

## Fragment Affinity Data for Four Targets

### BRD4
### NRP1
### SKP1
### STING

## ADMET Data

### BBB permeability
### Microsomal stability
### 3T3 phototoxicity

---

## 1-a: Fragment affinity data for BRD4

### Overview of Binding Affinity Evaluation

Binding affinity refers to how strongly and stably a compound interacts with a target protein—in this case, BRD4. BRD4 (Bromodomain-Containing Protein 4) is an epigenetic reader protein involved in transcriptional regulation and is known to play a role in various diseases, including cancer and inflammatory disorders.

Surface Plasmon Resonance (SPR) is a highly sensitive, label-free method capable of real-time detection of molecular interactions. It is particularly effective for the early screening of small-molecule fragments. In this study, we established an SPR assay targeting BRD4 and evaluated both binding activity and affinity for a total of 1,905 fragment compounds.

### Experimental Method

Fragment screening against BRD4 protein was conducted using surface plasmon resonance (SPR) on a Biacore 8K (Cytiva) system, targeting 1,905 compounds from the High Fidelity Fragment Library (HFFL). BRD4 protein was immobilized on a Neutravidin (NA) sensor chip at approximately 3,000–3,400 RU. To reduce non-specific interactions, 50 µM amino-PEG11-biotin was injected across both active and reference flow cells for blocking. Each compound (100 mM in DMSO) was transferred to a 384-well SPR plate using an Echo 650 dispenser, with 0.5 µL per well. After adding 2.5% buffer, the final compound concentration was 500 µM with 3% DMSO. The screening was performed with a 30-second association phase and a 60-second dissociation phase. Blank buffer was injected every five cycles and the reference compound JQ1 (0.5 µM) every 25 cycles to ensure data consistency. Hit selection was based on parameters such as binding response, dissociation profile, residual binding at the end of dissociation, theoretical Rmax comparison, and similarity to the reference compound. A total of 78 compounds were identified as hits.

These 78 hit compounds were subjected to dose-response experiments using SPR to determine their binding affinities (Kd). Each compound was tested at three concentrations: 50 µM, 150 µM, and 500 µM. The compounds were dispensed into 384-well plates using an Echo 650 in volumes of 50, 150, or 500 nL, and DMSO was added to ensure a final volume of 500 nL with 3% DMSO concentration. Subsequently, 100 µL of 2.5% buffer was added using a MultiDrop Combi dispenser. Each measurement included two blank injections followed by a compound injection, with 30-second association and 60-second dissociation phases. Post-injection, a wash step using 50% DMSO was performed. Solvent correction was carried out at the beginning, middle, and end of the experiment using 2.5% and 3.8% DMSO buffers mixed in 8 different ratios. Binding affinities were determined from steady-state response versus concentration plots. Curve fitting was constrained by fixing the offset at 0 RU and setting Rmax based on the theoretical maximum for each compound. A total of 29 compounds with Kd values below 1 mM were considered to exhibit reliable affinities. Additional evaluation metrics included surface occupancy and assessment of steady-state behavior in the binding curves.

### Data Analysis and Binary Classification

Steady-state binding affinity (KD) was determined based on the SPR response plotted against compound concentration. To ensure reliable fitting with only three data points, the offset was fixed at 0 RU, and the theoretical Rmax was individually set per compound. Compounds with KD values below 1 mM were considered reliable, while those showing no plateau or linear binding responses were deemed less reliable.

In addition to quantitative analysis, a binary classification was applied to the dataset. Specifically, fragments with KD values below 1 mM were labeled as positive (1), and those with KD values equal to or above 1 mM were labeled as negative (0).

---

## 1-b: Fragment affinity data for NRP1

### Overview of Binding Affinity Evaluation

Binding affinity refers to how strongly and stably a compound interacts with a target protein—in this case, NRP1. NRP1 (Neuropilin-1) is a cell surface co-receptor involved in various physiological functions including angiogenesis, neuronal guidance, and immune response.

Surface Plasmon Resonance (SPR) is a highly sensitive, label-free method capable of real-time detection of molecular interactions. It is particularly effective for the early screening of small-molecule fragments. In this study, we established an SPR assay targeting NRP1 and evaluated both binding activity and affinity for a total of 1,905 fragment compounds.

### Experimental Method

Fragment screening against NRP1 protein was performed using surface plasmon resonance (SPR) on a Biacore 8K (Cytiva), targeting 1,905 compounds from the High Fidelity Fragment Library (HFFL). NRP1 protein was immobilized on a Neutravidin sensor chip at approximately 6,100–6,600 RU, and 50 µM amino-PEG11-biotin was used for blocking non-specific binding across both active and reference flow cells. Each compound, initially prepared at 100 mM in DMSO, was transferred to a 384-well plate using Echo 650 (0.5 µL/well), and diluted with 2.5% buffer to a final concentration of 500 µM and 3% DMSO. The reference compound EG01377 was prepared at 20 µM. The screening was conducted over four days in separate runs. Each injection involved a 30-second association phase without dissociation, followed by a wash with 50% DMSO. Blank buffer was injected every five cycles, and the reference compound every 25 cycles and at both the start and end of the experiment. Signal responses, slopes, residual binding, and comparisons to theoretical Rmax were used as criteria to select 192 hits.

Subsequently, dose-response measurements were performed for the 192 hit compounds to determine their binding affinities to NRP1. Each compound was tested at three concentrations: 50, 150, and 500 µM. Using Echo 650, 50–500 nL of each compound was dispensed into wells, followed by DMSO addition to adjust the volume to 500 nL and dilution with 100 µL of 2.5% buffer. Two blank injections were performed before each compound injection, which was conducted under 30-second association and 60-second dissociation conditions. The reference compound EG01377 was injected at the beginning, middle, and end of the experiment to monitor chip stability. Solvent correction was applied using mixtures of 2.5% and 3.8% DMSO buffers at multiple ratios. Kd values were calculated from steady-state responses using a constrained fitting approach: global fitting for offset and theoretical Rmax for each compound. Out of the 192 compounds tested, 66 exhibited reliable affinities with Kd 30 RU, acceptable response slope, minimal stickiness ( 30 minutes were labeled as positive (1), and those with t₁/₂ ≤ 30 minutes were labeled as negative (0).

---

## 2-c: ADMET data for 3T3 phototoxicity

Phototoxicity is an in vitro assay used to assess the potential of a substance to induce photoirritation, for example using 3T3 mouse fibroblast cells.

In this study, an in vitro phototoxicity assay using NIH/3T3 mouse fibroblast cells was performed to evaluate the phototoxic potential of 50 chemical compounds. Each compound was tested at a single concentration of 20 µM, and cytotoxicity was assessed under two conditions: with and without ultraviolet A (UV-A) irradiation at an effective dose of 5.5 to 6 J/cm². Cell viability was determined using a resazurin-based fluorescence assay, and compounds that exhibited more than 40% difference in viability between irradiated and non-irradiated conditions were considered to have potential phototoxicity.

Following the initial screening, six compounds that showed suspected phototoxic effects were selected for further evaluation through a dose-response phototoxicity assay. In this phase, the compounds were tested across a concentration range of 0.1 µM to 250 µM, and dose-dependent cytotoxicity was measured under both irradiated and non-irradiated conditions. From the resulting data, the half-maximal inhibitory concentration (IC₅₀) values were calculated, and the Photo-Irritation Factor (PIF) was determined. The PIF is defined as the ratio of the IC₅₀ value obtained under non-irradiated conditions to that obtained under irradiated conditions, expressed as PIF = IC₅₀(−UV) / IC₅₀(+UV).

Based on the PIF values, compounds were classified according to the following criteria: compounds with a PIF less than 2 were considered non-phototoxic; those with a PIF between 2 and less than 5 were considered to have possible or borderline phototoxicity; and those with a PIF of 5 or higher were classified as phototoxic. In addition, a binary classification was performed in which compounds with a PIF less than 2 were labeled as positive (1), and those with a PIF of 2 or higher were labeled as negative (0).

