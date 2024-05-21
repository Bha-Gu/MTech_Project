# A novel hybrid intrusion detection method integrating anomaly detection with misuse detection.
Kim et al. offered another hybrid-based IDS, and the NSL-KDD data set was subjected to decision tree and 1-class SVM analysis. 
The C4.5 decision tree (DT), which was also utilized to split up the regular training data into smaller subsets, was used to develop the misuse detection model. 
Then, a model for detecting anomalies was built utilizing a single-class SVM in each deconstructed region. 
This model can indirectly leverage knowledge of past attacks to improve its performance when creating profiles of typical behavior. 
The experimental findings showed that the proposed model might enhance the IDS’s performance and speed in identifying unknown threats while also reducing the training and testing procedures’ time complexity. 
The model’s overall average training and testing times were 56.58 and 11.20 s, respectively. 
However, because the original C4.5 decision tree does not take into account clusters in the normal data set, it can split a well-formed normal cluster during the decomposition processes. 
This can impede the well-formed normal cluster that is associated with a single decision boundary in the 1-class SVM model and reduce the model’s capacity for profiling. 
Additionally, when there is an unequal distribution of data, training and testing take longer. 
As a result, the suggested method’s capacity for time reduction falls short of expectations. 
In order to enhance the model’s performance without reducing its capacity to identify unidentified attacks, different classifiers must be investigated.