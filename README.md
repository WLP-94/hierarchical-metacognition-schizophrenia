# Hierarchical Metacognition in Schizophrenia
This repository contains anonymized research data from a series of behavioral and EEG studies investigating metacognition across different hierarchical levels in the schizophrenia spectrum.

**Project Overview**

The project examined metacognition from multiple levels of evaluation:

Local metacognition: monitoring and evaluating one's own performance on individual cognitive decisions.
Task-based global metacognition:  integrating accumulated task information to form global evaluations of expected performance.
Higher-order global metacognition:  evaluating one's cognitive abilities based on objective cognitive performance and information derived from others' evaluations.

Across three studies, behavioral performance, metacognitive measures, clinical characteristics, and EEG measures were examined to investigate how metacognitive processes may differ across levels of cognitive evaluation.

---

**Study 1: Local and Higher-Order Metacognition**

Study 1 examined local metacognition in individuals with schizophrenia and healthy controls using a perceptual decision-making task. Participants provided confidence judgments regarding their performance, allowing metacognitive sensitivity to be quantified.

The study also examined higher-order metacognition using the Meta-Cognition Assessment Scale–Abbreviated (MAS-A), together with clinical symptom measures.

Data file

study1/study1_data.xlsx

The file contains participant-level demographic, behavioral, metacognitive, clinical, and MAS-A measures.

Data structure: one row per participant.

-gender: 0-male, 1-female
-group: 1- schizophrenia, 0-healthy control
-d: perceptual sensitivity (d′)
-meta_d: metacognitive sensitivity (meta-d′)
-meta_d/d: meta-d′ / d′
-mean_confidence: mean confidence rating
-accuracy: choice accuracy
-MASA_total: total score of the Meta-Cognition Assessment Scale–Abbreviated (MAS-A)
-MASA_self_reflectivity: Self-Reflectivity subscale
-MASA_awareness_of_other: Awareness of Other subscale
-MASA_decentration: Decentration subscale
-MASA_mastery: Mastery subscale
-SAPS: Scale for the Assessment of Positive Symptoms
-SANS: Scale for the Assessment of Negative Symptoms
-YBOCS: Yale-Brown Obsessive Compulsive Scale
-PHQ9: Patient Health Questionnaire-9
-GAD7: Generalized Anxiety Disorder-7

Note: Participant identifiers in three studies are independent. The same identifier does not indicate that the participant is the same individual across studies.

---

**Study 2: Task-Based Global Metacognition**

Study 2 investigated task-based global metacognition through subjective performance estimation (SPE). Participants formed global evaluations of their expected performance based on information accumulated during the task.

The study examined how participants integrated performance-related information under different experimental conditions and whether feedback influenced global metacognitive evaluations.

Data files

study2/study2_participant.xlsx

Contains participant-level behavioral and metacognitive measures.

Data structure: one row per participant.

-gender: 0-male, 1-female
-group: 1- schizophrenia, 0-healthy control
-E_d: perceptual sensitivity (d′) in easy condition
-E_metad: metacognitive sensitivity (meta-d′) in easy condition
-E_metad/d: meta-d′ / d′ in easy condition
-D_d: perceptual sensitivity (d′) in difficulty condition
-D_metad: metacognitive sensitivity (meta-d′) in difficulty condition
-D_metad/d: meta-d′ / d′ in difficulty condition

study2/study2_SPE.xlsx

Contains data corresponding to individual SPE comparisons. Each row represents a participant within a specific SPE comparison.

The dataset retains the specific task blocks that formed each SPE comparison rather than collapsing across individual task blocks. This preserves the experimental structure of the SPE manipulation.

study2/study2_scales.xlsx

Contains clinical symptom measures collected in Study 2.

---

**Study 3: Metacognition and EEG in the Clinical High-Risk State**

Study 3 examined metacognitive processing in individuals at clinical high risk for psychosis (CHR-P) and healthy controls. The study combined behavioral metacognitive measures with EEG recordings.

The experimental design manipulated task difficulty, task type, and metacognitive level. EEG analyses focused on amplitude and power measures across multiple brain regions.

Data files

study3/study3_behavioraldata.xlsx

Contains behavioral and metacognitive measures across experimental conditions.

Data structure: participant × experimental condition.

-diff: the difficulity of task; easy-0, difficulty-1
-task: the type of task; memory task-0, perception task-1
-spechoice_tran: SPE task selection probability, transformed using the arcsine square-root transformation

study3/study3_scales.xlsx

Contains clinical and symptom-related measures collected in Study 3.

study3/study3_eeg_analysis.xlsx

Contains EEG measures used for the primary analyses. The dataset includes EEG amplitude and power measures across brain regions and experimental conditions.

The experimental factors represented in this dataset include:

* task difficulty (diff, easy-0, difficulty-1);
* task type (task, memory task-0, perception task-1); and
* metacognitive level (meta: local-0, global-1).

study3/study3_eeg_electrode/

Contains electrode-level EEG data.

* chr_per_channels.csv: electrode-level EEG data for the CHR group.
* health_per_channels.csv: electrode-level EEG data for the healthy control group.

The electrode-level data are provided separately from the analysis-level EEG dataset to preserve both accessibility for the primary analyses and access to more detailed spatial EEG information.

---

**Data Organization**

The datasets are provided primarily at the participant, experimental-condition, and analysis levels rather than as raw trial-by-trial behavioral recordings or continuous EEG recordings.

This organization was chosen to provide the data necessary to understand and reproduce the reported analyses while avoiding unnecessary disclosure of highly detailed participant-level information.


**Participant Identifiers and Privacy**

All datasets have been de-identified for research data sharing.

The repository does not contain names, contact information, hospital record numbers, or other direct personal identifiers.

The participant identifiers included in the datasets are research-specific identifiers and should not be used to infer participant identity.

Some datasets contain clinical and symptom-related measures. Users should therefore treat these data as sensitive research data and use them only for legitimate scientific and research purposes.

Users must not attempt to identify individual participants or link these datasets with other information for the purpose of participant re-identification.


**Missing Data**

Blank cells indicate missing or unavailable values unless otherwise specified by the structure of a particular dataset.

Blank entries may also indicate that a variable was not applicable to a particular participant or experimental group.


**Ethical Considerations**

The data were collected as part of research involving human participants.

Only de-identified variables considered appropriate for public data sharing are provided in this repository. The publicly available datasets do not include direct personal identifiers.

Users are responsible for complying with applicable ethical, privacy, and data protection requirements when accessing or using these data.


**Data Use and Citation**

These datasets are provided to support scientific transparency, replication, and secondary research.

If you use any of the data in a publication, presentation, thesis, or other scholarly work, please cite the associated research article and this data repository.

Associated publication

Citation information will be added here following publication.


**Repository citation**
A permanent repository citation/DOI will be added here when available.


**Contact**
For questions regarding the dataset, data interpretation, or appropriate use of the data, please contact the corresponding author of the associated research project.

