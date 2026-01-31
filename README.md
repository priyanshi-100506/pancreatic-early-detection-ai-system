`Multi-Modal Temporal Risk Stratification for Early-Stage PDAC

1. Clinical Hypothesis: The "Temporal Drift"
The core innovation is modeling the "velocity" of change in metabolic markers. This system identifies the divergence in a patient's historical baseline before a clinical diagnosis is made.

1.1 Longitudinal Biomarker Trajectories

Glucose Drift: Identifying the non-linear upward trajectory in blood glucose.

Weight Velocity: Monitoring the unexplained decline in BMI (Cachexia).


<img width="637" height="802" alt="image" src="https://github.com/user-attachments/assets/c5d9404f-eb54-425c-a8db-2ea623b2f3d5" />


2. Technical Architecture & Clinical Reasoning
The system integrates a 1D-CNN Encoder with tabular feature fusion. The model doesn't just predict; it ranks clinical markers based on their predictive power.

2.1 Biomarker Importance
Analysis reveals that CA19-9 drift and Glucose/Weight slopes are the primary drivers of the risk score, significantly outweighing static factors like age.


<img width="421" height="259" alt="image" src="https://github.com/user-attachments/assets/25d223db-d294-44cf-a33f-eeb8843180d7" />


3. Explainable AI (XAI) for Clinical Trust
To ensure the "Right to Explanation" in medical settings, we utilize SHAP (SHapley Additive exPlanations) and Saliency Mapping to validate the model's logic.

3.1 Global & Local Interpretability

Global Trends: Visualizing which biomarker trends the AI prioritizes across the entire cohort.


Patient Report Card: A "Force Plot" showing the tug-of-war between features pushing a specific patient's risk up or down.


<img width="498" height="556" alt="image" src="https://github.com/user-attachments/assets/4b75ff7f-2c08-407b-8b06-9a9734e0002c" />


4. Performance Validation
Medical screening requires a balance between sensitivity and the cost of false alarms. We optimize the system for rare disease prevalence.

4.1 Lead-Time & Threshold Optimization

Model Performance vs. Lead-Time: Demonstrating how prediction accuracy (AUROC) increases as the patient approaches the 3-month diagnostic window.


Clinical Decision Frontier: Optimizing the "Alert Line" where Precision (Certainty) and Recall (Catching Cases) intersect.


<img width="351" height="238" alt="image" src="https://github.com/user-attachments/assets/6fcb94ef-bd2f-4ad3-ab61-e83a01b14ed7" />
<img width="649" height="438" alt="image" src="https://github.com/user-attachments/assets/5570374a-b6eb-4414-be77-4a1bc57de493" />



5. Advanced Clinical Actionability
The system categorizes high-risk patients for immediate clinical follow-up using manifold projections and risk progression heatmaps.

5.1 Risk Progression for Top Cases
A temporal heatmap tracks the risk levels of the top 10 suspected cases, providing a clear dashboard for surgical or imaging triage.


<img width="480" height="325" alt="image" src="https://github.com/user-attachments/assets/3dc84fe3-b698-4114-8578-090a54c65168" />
<img width="498" height="292" alt="image" src="https://github.com/user-attachments/assets/a361b0ce-2190-4b1e-a40b-e7436a233574" />


5. Implementation Summary
This system demonstrates that AI can provide a Lead-Time Advantage by identifying "Endogenous Drift" 6–9 months before traditional symptoms, potentially shifting the diagnostic window toward early-stage surgical resection.

This research prototype serves as a technical proof-of-concept for the integration of deep temporal learning in clinical oncology workflows.

