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

*   Che et al, 2018. "{{% resource_link "bd09049c-b5a8-4b64-999b-2095626c7423" "Recurrent Neural Networks for Multivariate Time Series with Missing Values" %}}." _Nature Scientific Reports._ 
*   Dernoncourt et al, 2016. "{{% resource_link "cc9b8fe7-49f1-47cb-858c-38a5bb4987fc" "De-Identification of Patient Notes with Recurrent Neural Networks" %}}." _JAMIA_. 
*   Ghassemi et al, 2014. "{{% resource_link "4acec29c-c9f6-46c4-8be8-7ed344b2ba5b" "Unfolding Physiological State: Mortality Modelling in Intensive Care Units" %}}." _KDD_. 
*   Boag et al, 2018. "{{% resource_link "b4ac8b37-43c5-4eaf-bc05-f8d24001712d" "Racial Disparities and Mistrust in End of Life Care" %}}." _MLHC_.
*   Johnson et al, 2017. "{{% resource_link "4b2c148f-c04e-4084-ab1a-d43214f70056" "Reproducibility in Critical Care: A Mortality Prediction Case Study" %}}." _MLHC_. 
*   Schulam et al. 2016. "{{% resource_link "808e6be1-c28e-4697-b1eb-fca4dc61c60d" "Integrative Analysis using Coupled Latent Variable Models for Individualizing Prognoses (PDF)" %}}." _JMLR_. 
*   Young et al. 2018. "{{% resource_link "95ab660e-af67-47a1-8eae-61849bc3aa70" "Uncovering the Heterogeneity and Temporal Complexity of Neurodegenerative Diseases with Subtype and Stage Inference" %}}." _Nature Communications_. 

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

*   _Example of Prediction_: Razavian et al., 2015. "{{% resource_link "31f07035-c7c7-43be-8316-8d4a57df33c2" "Population-Level Prediction of Type 2 Diabetes From Claims Data and Analysis of Risk Factors: Big Data." %}}"
*   _Example of Causal inference_: Brat et al., 2018. "{{% resource_link "5f54ea36-a78b-4328-9db6-117bf7db9c3a" "Postsurgical Prescriptions for Opioid Naive Patients and Association With Overdose and Misuse: Retrospective Cohort Study." %}}"
*   _Example of Characterization_: Hripcsak et al., 2016. "{{% resource_link "0377a959-2428-4017-95a1-3e2ca12a2ae5" "Characterizing Treatment Pathways at Scale Using the OHDSI Network, PNAS." %}}"
*   _Example of Subtyping_: Doshi-Velez et al., 2014. "{{% resource_link "7b35de72-8ca5-4132-9974-6a9d689a82e3" "Comorbidity Clusters in Autism Spectrum Disorders: An Electronic Health Record Time-Series Analysis, Pediatrics." %}}"

### Machine Learning Methodology

The projects mentioned here focus on developing new machine learning methods:

*   Develop better deep learning algorithms for claims data.
    *   Example: widening the gap between the deep learning and baseline methods from {{% resource_link "4c16172e-4b42-4903-b639-067a385741a7" "Rajkomar et al., 2018" %}} and {{% resource_link "5138c5fb-de6c-4cd6-a4b8-a7cd57e5bf48" "Choi et al., 2016 Doctor AI (PDF)" %}}. You could design {{% resource_link "555b6928-9de8-438b-a1d1-fd53566ee91a" "new architectures" %}} that are better suited for medical data, unsupervised learning algorithms (see e.g. {{% resource_link "42179a72-e519-47eb-9a4d-305f8e301609" "Choi et al., 2016 Relationships" %}} and {{% resource_link "5236a347-388a-4f5e-8d1e-bc02908d4653" "Beam et al., 2018" %}}), etc.
*   Develop synthetic data generation methods that produce realistic data but have provable privacy guarantees (this is a good project for a group with a theoretical computer science bent).
    *   Recent work has been interested in using deep learning for this, e.g. {{% resource_link "ba05648d-67c7-43a7-8685-c765d0558b45" "Choi et al., 2017" %}} and {{% resource_link "9c72b5c6-9639-4522-ac61-386f65df0e28" "Hyland et al., 2017" %}}. However, there is a natural trade-off between truly capturing the data density (not just being able to reproduce aggregate statistics from synthetic data) and not leaking private information from the training data. How does one formalize this mathematically?
*   Learn models of what a "normal" treatment policy is for a disease (note: it may be sequential).
    *   How do these differ across populations, either geographic or based on patient characteristics? Can you automatically discover different treatment strategies for the same condition? Can you identify patients that are outliers or are receiving abnormal treatment (these may because of fraud, improper treatment, medical errors, etc.)?
*   Develop algorithms for inferring causality (e.g., one condition causes another, or a medication causes a side-effect) from longitudinal claims data, e.g. by using ideas from Granger causality, the recently developed {{% resource_link "36dd2264-b019-481e-bcba-a370275b3f2a" "entropic causality" %}}, causal Bayesian networks, or {{% resource_link "1814db0a-c4ee-4ed3-bac2-1b546eb00050" "Hawkes processes (PDF)" %}}.
*   Develop algorithms to identify and explain non-stationarity, e.g. through changepoint detection and interpretable ML algorithms.

Other Datasets
--------------

*   {{% resource_link "28584375-2f50-4573-a1f6-3f572ee9c801" "Multiple Myeloma Research Foundation Compass" %}}
*   {{% resource_link "a396334c-7713-45a0-80ca-db5762ce58e1" "The Parkinson’s Progression Markers Initiative" %}}
    *   Specific project suggestion: Learning a representation of MRI images that will help with downstream tasks, e.g. classifying healthy, prodromal, early-stage Parkinson’s, vs late-stage Parkinson’s, or time to outcome. Possible methodologies to consider include {{% resource_link "bc99c949-1651-401e-81e0-e1563a2d1aad" "3-D CNN" %}}, {{% resource_link "5977ac27-eb3e-4e18-8cd0-cd633b3f84d1" "voxel-based logistic regression" %}}, or principal components. Can you interpret what the representation is capturing?
*   {{% resource_link "d3b180d0-cf27-4ed1-88e0-912e11cac1b7" "eICU" %}}
    *   Same access requirements as MIMIC-III. eICU has clinical ICU data from 200+ hospitals.
*   Chest X-rays
    *   {{% resource_link "0a075177-96e7-49c0-a728-4ab678879d81" "The MIMIC-CXR Database" %}}
    *   {{% resource_link "a9efd6fe-9cba-4daf-ba15-5abde24beba7" "CheXpert" %}}
    *   {{% resource_link "93998404-c9e9-4bd7-aa9e-c3725481324c" "Open-i service of the National Library of Medicine" %}}
        
*   {{% resource_link "50a242d7-53e3-4546-b32f-904f5ac4ec31" "The Osteoarthritis Initiative" %}}
*   A more extensive {{% resource_link "a365a2a8-a956-427c-9597-384e308d6c7b" "list of medical datasets" %}}.