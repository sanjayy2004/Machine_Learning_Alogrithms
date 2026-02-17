🏏 K-Means Clustering: Cricket Batsmen Analysis
KMEANS.ipynb implements unsupervised clustering on ODI cricket batting stats for 79 top players, grouping them by performance metrics like Runs, Average, and Strike Rate. It uses Scikit-learn's KMeans on scaled features (Mat, Inns, NO, Runs, Ave, BF, SR, 100, 50, 0, exp) after EDA and preprocessing.
​

📊 Dataset Overview
Loads "C-1-3 1 3.csv" with 79 rows × 13 columns: Player, Span, Mat (matches), Inns (innings), NO (not outs), Runs, HS (high score), Ave (average), BF (balls faced), SR (strike rate), 100s, 50s, 0s.
​

Top players include:

SR Tendulkar (INDIA): 18,426 Runs, 44.83 Ave, 86.23 SR (23 years).
​

KC Sangakkara (Asia/ICC/SL): 14,234 Runs, 41.98 Ave, 78.86 SR.
​

RT Ponting (AUS/ICC): 13,704 Runs, 42.03 Ave, 80.39 SR.
​

Player	Runs	Ave	SR	Years
SR Tendulkar	18,426	44.83	86.23	23
​
KC Sangakkara	14,234	41.98	78.86	15
​
RT Ponting	13,704	42.03	80.39	17
​
ST Jayasuriya	13,430	32.36	91.20	22
​
🔧 Preprocessing Steps
Parses Span into start/end years, computes exp (experience).
​

Drops Span/start/end; no nulls/duplicates found.
​

Scales numeric features (Mat, Inns, NO, Runs, Ave, BF, SR, 100, 50, 0, exp) using StandardScaler for KMeans.
​

🤖 K-Means Implementation
Tests k=2–7 via Elbow (inertia/SSD) and Silhouette scores; plots both for optimal k selection.
​

Fits KMeans on scaled data.
​

Adds clusterid column; visualizes clusters in 3D scatter (Runs vs Ave vs SR) and 2D/3D plots.
​

📈 Key Visualizations
Elbow Plot: SSD drops sharply, suggesting k=3–4.
​

Silhouette Plot: Highest score picks optimal clusters.
​

3D Cluster Plot: Color-coded by clusterid (0–2); shows player distribution.
​

Cluster Table: Group summaries (e.g., high-Runs/low-SR vs aggressive SR).
​


​

💡 Insights & Extensions
Identifies batsman archetypes (e.g., accumulators vs strikers). Add PCA for 2D viz, silhouette per cluster, or domain-specific metrics like consistency (std dev of scores).
​
