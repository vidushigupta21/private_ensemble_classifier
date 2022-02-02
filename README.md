# private_ensemble_classifier
**Origin**
Since the 1990s, Machine Learning (ML) has considerably modified the health care system. According to the World Health Organization, more that 264 million people globally have depression and APA, (American Psychological Association) found out that primary care physicians are often the one diagnosing mental disorders without adequate training. it's proven that the approach of physicians regularly checking patient's mental health and disorders together with psychologists and other professionals to treat patients have led to reduced costs and better patient outcomes.
This can add-on to a lot of extra cost, extra training and is generally noy often logistically feasible. Using machine learning and data from patient’s medical file, one's mental health status can be classified with very little human participation and with lower time and less cost. Privacy leakage can occur at any point in the machine learning lifecycle, from model training through model deployment. As a result, safeguarding users’ privacy is critical in healthcare issues.

**Objectives**
The goal of this project is to gather data about people from the patient’s medical record to classify the mental illness using ensemble learning as our main approach. This will require very little human participation from doctors and has lower time and money costs associated Prevent privacy leakage in the classification process, while ensuring data utility prediction accuracy. Provide assistance to medical practitioners to keep track of patients.
**Proposed solution**
The project focuses on building an ensemble learning differentially private ML classification model that will identify early symptoms of possible mental illness with the help of various ML classification algorithms. That would also provide a useful tool to assist physicians in therapy.
**Contributions**
-Patient empowerment
-Reduce Stigma
-Self-Monitoring
-Enhance Provider/Patient Communication
-Provide Psycho-education
-Privacy to patients
**Approach**
The approach for this project is to take a combination of best performing classifiers to create an ensemble. So that adding randomness to their output for privacy protection would not affect the data utility greatly.
**Method**
-the data is pre-processed with feature engineering, filling missing values, and scaling is done with the goal of increasing accuracy of the models.
-split the data into train, test and validation set and train each base classifier on the train dataset.
-The meta-model is fit on the predictions made by each base model on a holdout dataset. meta-model can be any of the best performing ML model, such as logistic regression for classification.
-By not training the blender model directly on the private data, we prevent it from directly learning key individual features of a single person from the dataset.
-we add a bit of randomness to the result of base classifiers and skew the final result so that the true label doesn’t easily change by dropping just one base learner.
-The performance of blendor model was evaluated using various evaluation metrics such as accuracy, AUC score, recall, f1 score.
