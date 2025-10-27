---
content_type: page
description: Suggestions for final projects for 6.S897 Machine Learning for Healthcare.
learning_resource_types:
- Projects
ocw_type: CourseSection
parent_title: Projects
parent_type: CourseSection
parent_uid: 8f308296-4b99-c74b-3eca-95954f1f7ea2
title: Final Project Suggestions
uid: fd4248e5-f68f-2233-10cd-dc3d049961b4
---

Students will produce a final project using a health insurance claims database such as IBM MarketScan, Optum, Center for Medicare & Medicaid Services claims data, or state All-Payer Claims Databases.

Below we describe two types of projects, those focused more on answering a specific clinical question and those focused more on developing novel ML methods. That said, we imagine that many projects may involve a bit of each, and that’s OK!

MIMIC Projects
--------------

### Clinical Projects

MIMIC-III provides a wealth of data to tackle a variety of clinical tasks in the ICU. Here are a few examples of potential clinical questions:

*   Identify organ failure
    *   In the ICU, we are concerned about organ failure in the heart, kidney, liver, and lung. What predictors could be useful for organ failure?
    *   We would want an early enough prediction to be productive and sufficient data in the lab tests (e.g. liver enzymes, creatinine and BUN, blood pressure) in earlier data.
*   Effects of interventions
    *   Which interventions should we do and at what time?
    *   Potential interventions include vasopressors, mechanical ventilation, dialysis, and cardiac assist devices.

Below are some examples of research papers that used the MIMIC-III dataset:

*   Che et al, 2018. "{{% resource_link "8632c439-c517-443d-87df-cf0bce5ed4ac" "Recurrent Neural Networks for Multivariate Time Series with Missing Values" %}}." _Nature Scientific Reports._ 
*   Dernoncourt et al, 2016. "{{% resource_link "f1823fa0-445d-4280-b1a8-532b928e21ff" "De-Identification of Patient Notes with Recurrent Neural Networks" %}}." _JAMIA_. 
*   Ghassemi et al, 2014. "{{% resource_link "c9acdcc5-5f24-4224-aae7-fdcee8bd6970" "Unfolding Physiological State: Mortality Modelling in Intensive Care Units" %}}." _KDD_. 
*   Boag et al, 2018. "{{% resource_link "34a31f17-2c35-40fa-996f-8bceb19cbf2b" "Racial Disparities and Mistrust in End of Life Care" %}}." _MLHC_.
*   Johnson et al, 2017. "{{% resource_link "46721b60-5b4f-44b3-b431-ca1122801293" "Reproducibility in Critical Care: A Mortality Prediction Case Study" %}}." _MLHC_. 
*   Schulam et al. 2016. "{{% resource_link "0a14cd7c-a2fa-4f5f-a4b4-bd688d9d8ac3" "Integrative Analysis using Coupled Latent Variable Models for Individualizing Prognoses (PDF)" %}}." _JMLR_. 
*   Young et al. 2018. "{{% resource_link "d7527a4d-14d3-4300-be9e-44a03808ee00" "Uncovering the Heterogeneity and Temporal Complexity of Neurodegenerative Diseases with Subtype and Stage Inference" %}}." _Nature Communications_. 

### Machine Learning Methodology

Similar to above, you can also explore how to extend known machine learning methodology given the challenges of clinical data:

*   Clinical natural language processing (NLP)
    *   How can we better extract entities from the clinical notes such as diseases, symptoms, and treatments? We saw in problem set 3 how existing methods can be flawed. Once we do have these entities, how can we identify relations between the extracted clinical concepts?
    *   Can we construct a timeline from the clinical notes? How would these extracted entities relate with the coded events in the patient chart?
*   Time series
    *   How can we better predict a patient’s progression? Challenges could include missing data, unknown alignment of patients, and heterogeneity of conditions.
    *   How can we interpret a patient’s progression? Clinicians may be interested in how a patient progresses through known concepts (e.g. ICD-9 codes) and also what the specific stages of progression might be.

Projects Using IBM MarketScan Data
----------------------------------

Although not publicly available, students were provided access to the IBM MarketScan research database in the 2019 version of the course. These ideas can easily be extended to other research databases such as Optum, Center for Medicare & Medicaid Services claims data, or state All-Payer Claims Databases. Since the MarketScan research database has coverage of a patient’s full longitudinal clinical trajectory, it is a gold mine for research and already thousands of papers have been published using it. Students should expect to access the data including basic demographics, diagnoses, procedures, outpatient prescription orders, laboratory test orders, and enrollment information.

### Clinical Projects

This type of MarketScan project will focus on studying a new clinical question using machine learning and causal inference methods studied in class.

*   Early detection of a medical condition, e.g. rheumatoid arthritis or Sjogren’s syndrome
*   Causal inference of the effect of an intervention
*   Subtyping or clustering to better understand a population, e.g. individuals rehospitalized within 30-days

Below are examples of papers that have explored some of the above questions. We encourage students to use these for inspiration, but to tackle new clinical questions that weren’t already answered in these (e.g., studying a different disease or a different outcome).

*   _Example of Prediction_: Razavian et al., 2015. "{{% resource_link "42912bb2-9513-41c0-8111-c451bd436dc8" "Population-Level Prediction of Type 2 Diabetes From Claims Data and Analysis of Risk Factors: Big Data." %}}"
*   _Example of Causal inference_: Brat et al., 2018. "{{% resource_link "dbbd58da-0cb9-41c4-afb3-20e2ff5a4df1" "Postsurgical Prescriptions for Opioid Naive Patients and Association With Overdose and Misuse: Retrospective Cohort Study." %}}"
*   _Example of Characterization_: Hripcsak et al., 2016. "{{% resource_link "94b65f9a-abe0-489f-bb3a-1927a05a179f" "Characterizing Treatment Pathways at Scale Using the OHDSI Network, PNAS." %}}"
*   _Example of Subtyping_: Doshi-Velez et al., 2014. "{{% resource_link "dbc805a1-68cb-4f07-a9c8-3e4b4a2c8787" "Comorbidity Clusters in Autism Spectrum Disorders: An Electronic Health Record Time-Series Analysis, Pediatrics." %}}"

### Machine Learning Methodology

The projects mentioned here focus on developing new machine learning methods:

*   Develop better deep learning algorithms for claims data.
    *   Example: widening the gap between the deep learning and baseline methods from {{% resource_link "d79174a7-ccaa-4727-9468-d89ff105124c" "Rajkomar et al., 2018" %}} and {{% resource_link "97cc7d65-7371-4ec9-bf08-3cc960ba6c08" "Choi et al., 2016 Doctor AI (PDF)" %}}. You could design {{% resource_link "0c456534-8e81-4b18-8059-93b54389edee" "new architectures" %}} that are better suited for medical data, unsupervised learning algorithms (see e.g. {{% resource_link "bcbe0199-e91f-4e00-a46c-0d8e24364a43" "Choi et al., 2016 Relationships" %}} and {{% resource_link "bfa5b135-eacd-49e5-a2fb-80e4a3bb16dc" "Beam et al., 2018" %}}), etc.
*   Develop synthetic data generation methods that produce realistic data but have provable privacy guarantees (this is a good project for a group with a theoretical computer science bent).
    *   Recent work has been interested in using deep learning for this, e.g. {{% resource_link "decf83f6-88da-420a-924e-e52403a4733c" "Choi et al., 2017" %}} and {{% resource_link "b9a04e65-49fc-4543-aa09-42222becf206" "Hyland et al., 2017" %}}. However, there is a natural trade-off between truly capturing the data density (not just being able to reproduce aggregate statistics from synthetic data) and not leaking private information from the training data. How does one formalize this mathematically?
*   Learn models of what a "normal" treatment policy is for a disease (note: it may be sequential).
    *   How do these differ across populations, either geographic or based on patient characteristics? Can you automatically discover different treatment strategies for the same condition? Can you identify patients that are outliers or are receiving abnormal treatment (these may because of fraud, improper treatment, medical errors, etc.)?
*   Develop algorithms for inferring causality (e.g., one condition causes another, or a medication causes a side-effect) from longitudinal claims data, e.g. by using ideas from Granger causality, the recently developed {{% resource_link "ba47e2a6-853b-4bf0-b869-e312c91620f4" "entropic causality" %}}, causal Bayesian networks, or {{% resource_link "a33351f2-f4b5-426f-88c6-eaa82c77b096" "Hawkes processes (PDF)" %}}.
*   Develop algorithms to identify and explain non-stationarity, e.g. through changepoint detection and interpretable ML algorithms.

Other Datasets
--------------

*   {{% resource_link "7e5a1369-2da0-4a49-b273-b35d419e4b4c" "Multiple Myeloma Research Foundation Compass" %}}
*   {{% resource_link "c7a68ec7-a2df-4c10-8458-7c8f08e75a4b" "The Parkinson’s Progression Markers Initiative" %}}
    *   Specific project suggestion: Learning a representation of MRI images that will help with downstream tasks, e.g. classifying healthy, prodromal, early-stage Parkinson’s, vs late-stage Parkinson’s, or time to outcome. Possible methodologies to consider include {{% resource_link "68f86d5f-9c6a-4fa7-b48f-a2c2aef62e98" "3-D CNN" %}}, {{% resource_link "084bb6d4-bac7-4ca3-b4b4-be531fb3b710" "voxel-based logistic regression" %}}, or principal components. Can you interpret what the representation is capturing?
*   {{% resource_link "0eb3bc66-362c-4d39-a154-843efa7456a8" "eICU" %}}
    *   Same access requirements as MIMIC-III. eICU has clinical ICU data from 200+ hospitals.
*   Chest X-rays
    *   {{% resource_link "08787673-f702-471b-91e1-9f59421ec58a" "The MIMIC-CXR Database" %}}
    *   {{% resource_link "7069f54c-a650-4a62-b0a9-d9d0ac905be6" "CheXpert" %}}
    *   {{% resource_link "46173804-d62a-4625-b4c2-0d4149b99321" "Open-i service of the National Library of Medicine" %}}
        
*   {{% resource_link "d79f0b56-8f4f-4ccb-8076-9489544c2036" "The Osteoarthritis Initiative" %}}
*   A more extensive {{% resource_link "fd3f1c26-f09a-48dc-8e62-79d292a3f8fe" "list of medical datasets" %}}.