Key Components
1. Synthetic Clinical Timeline Generator

Generates 60-month biomarker trajectories (glucose, CA19-9, duct dilation, weight, texture drift) based on established medical progression patterns for pancreatic disease.

2. Temporal Pattern Encoder (1D-CNN)

Learns 6-month biomarker windows to identify subtle deviations associated with early progression.

3. Gaussian Mixture Model (GMM) Risk Scoring

Provides probability-driven normal–abnormal likelihoods using unsupervised clustering.

4. YOLOv8 Imaging Anomaly Detection

Detects structural irregularities in synthetic CT-style images, including duct asymmetry, texture drift, and morphological anomalies.

5. Vector Database Retrieval (FAISS/Pinecone)

Uses embeddings from CNN and GMM to retrieve the most similar historical progression patterns.

6. Unified Risk Horizon Curve

Integrates CNN, GMM, YOLO, and similarity signals to project a forward-looking 24-month risk horizon.

Tech Stack

Python, NumPy, Pandas, TensorFlow/Keras, Scikit-Learn, Gaussian Mixture Models, YOLOv8, FAISS/Pinecone, Matplotlib.

