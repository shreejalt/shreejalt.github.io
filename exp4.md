## Vehicle Trajectory Anomaly Detection

**Description:** The use case of this project was pretty simple. There are thousands of cameras running on a different sites and we need to find the vehicle
anomalies such as speeding, wrong side, accidents, etc. The best way to find these anomalies is to dynamically adapt with the site itself for the best results.
Therefore, I developed a fully unsupervised learning algorithm to learn the vehicle trajectory patterns for a given scene and finding the novelties using novel 
***prediction-reconstruction LSTMs, and multi radius OCSVMs***. All the results were on the private company dataset.


| Trajectory Type | Precision | Recall | FScore | Examples |
| --------------- | --------- | ------ | ------ | -------- |
| Normal          | 1.00      | 0.96   | 0.98   | 228      |
| Anomalous       | 0.95      | 1.00   | 0.97   | 150      |
 
