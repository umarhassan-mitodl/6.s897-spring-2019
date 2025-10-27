---
content_type: page
description: Questions to accompany class readings for 6.S897 Machine Learning for
  Healthcare.
learning_resource_types:
- Readings
ocw_type: CourseSection
parent_title: Readings
parent_type: CourseSection
parent_uid: b6a65dfb-0542-a2bd-f8cb-9752be672c9e
title: Reading Questions
uid: 4ff5320f-dbe1-919e-5251-edd7ae294617
---

Session 3 Reading Questions
---------------------------

*   What are some of the challenges of using retrospective data from electronic health records?
*   The paper states that "the presence of a white blood cell count test order is associated with a 2.1% lower survival rate (P\<0.001)." What does the P\<0.001 signify?
*   All else equal, would we expect the survival rate to be higher for a patient with a 5pm white blood test or a 5am white blood test?
*   All else equal, would we expect the survival rate to be higher for a patient with a Sunday white blood test or a Wednesday white blood test?
*   Besides time of lab test and the lab test value, what other healthcare process variables might give additional signal for prediction of 3-year survival?

Session 4 Reading Questions
---------------------------

*   \[Razavian et al, 2015\] The trained model used in this paper might not identify high risk patients well for a rural hospital in Wyoming. Name two potential reasons why.
*   \[Razavian et al, 2015\] In Figure 1, we see that Patient G is excluded because they experienced diabetes onset during the gap period. Why is there a gap period for this prediction task?
*   \[Pozen et al, 1984\] Based on the paper’s results, name three ways we would expect the CCU to change if we rolled out the model completely and physicians followed the model’s recommendations.

Session 5 Reading Questions
---------------------------

*   \[Caruana et al.\] What are the different approaches that the authors suggest for interpreting the results from learning with few versus very many features, and why are the different approaches needed?
*   \[Caruana et al.\] What utility does introducing a bias term serve in terms of improving the interpretability of the learned model?
*   \[Futoma et al.\] Before their "real-time validation" experiment, how do they decide how much data to consider for a negative example (i.e. one who never develops sepsis)?

Session 6 Reading Questions
---------------------------

*   \[Quinn et al, 2009\] What problem is the factorial model trying to solve that the SLDS model struggles with?
*   \[Hannun et al, 2016\] How does the performance of the DNN compare to the aggregated cardiologist score? How do the mistakes made by the DNN compare to those made by the cardiologists?

Session 7 Reading Questions
---------------------------

*   \[Leaman et al, 2015\] What makes identifying disorder mentions in clinical text difficult?

Session 10 Reading Questions
----------------------------

*   What is Echocardiography?
*   What is one reason why a doctor might want a VNAP to provide versioning?

Session 11 Reading Questions
----------------------------

*   What are the three models that the authors compare to build a health knowledge graph? (Give names of models, no need to elaborate.)
*   How are diseases and symptoms extracted from the clinical records?
*   Which symptom did the authors omit from the analysis?

Session 12 Reading Questions
----------------------------

*   What are patches and how are they used in the model outlined by the authors?
*   How did the authors incorporate a clinician into the pipeline?

Session 13 Reading Questions
----------------------------

*   What are sensitivity and specificity? Overall how do CAD systems and double-readings compare on sensitivity and specificity?
*   What are two challenges from using patch-centered methodologies?
*   What is tomosynthesis and how does it compare to traditional mammography?

Session 14 Reading Questions
----------------------------

*   Examine Table 1.1. Assume our universe only includes gods whose names begin with "H". This leaves us with 6 gods. What is P(Y^(a=0) = 1 | "H" gods)? What is P(Y^(a=1) = 1 | "H" gods)?
*   Examine Table 1.2. Assume our universe only includes gods whose names begin with "H". This leaves us with 6 gods. What is P(Y=1 | A=0, "H" gods)? What is P(Y=1 | A=1, "H" gods)?
*   Explain "confounding" in 15 words or less. Does not have to be a complete sentence.

Session 16 Reading Questions
----------------------------

*   The authors seek to model mechanical ventilation in the ICU as a off-policy reinforcement learning algorithm. What is the action space? What is the reward space? (Short answers okay!)
*   What is the main difference between on-policy and off-policy reinforcement learning? (can be short!) Why do the authors choose to use off-policy learning here?
*   Figure 6 shows the learned feature importance. Pick one value and explain whether or not it makes sense to be a high/low weight.

Session 17 Reading Questions
----------------------------

*   One difference between Komorowski et al 2018 and Prasad et al 2017 is the difference in reward function. What is the reward function here?
*   Name two limitations of the study.

Session 22 Reading Questions
----------------------------

*   Draft a paragraph on component or concepts in the white paper that the agency should:
    1.  Keep in future iterations
    2.  Remove or clarify in future iterations
    3.  Add (for missing components)Suggestions: consider topics covered in previous lectures including generalizability, evaluation, updating models, fairness, causality, etc.