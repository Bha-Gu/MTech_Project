# A systematic literature review for network intrusion detection system (IDS)
### Abstract 
With the recent increase in internet usage, the number of important, sensitive, confidential individual and corporate data passing through internet has increasingly grown. With gaps in the security systems, attackers have attempted to intrude the network, thereby gaining access to essential and confidential information, which may cause harm to the operation of the systems, and also affect the confidentiality of the data. To counter these possible attacks, intrusion detection systems (IDSs), which is an essential branch of cybersecurity, were employed to monitor and analyze network traffic thereby detects and reports malicious activities. A large number of review papers have covered different approaches for intrusion detection in networks, most of which follow a non-systematic approach, merely made a comparison of the existing techniques without reflecting an in-depth analytical synthesis of the methodologies and performances of the approaches to give a complete understanding of the state of IDS. Nonetheless, many of these reviews investigated more about the anomaly-based IDS with more emphasis on deep-learning models, while signature, hybrid-based (signature + anomaly-based) have received minimal focus. Hence, by adhering to the principles of Preferred Reporting Items for Systematic Reviews and Meta-Analyses (PRISMA), this work reviewed existing contributions on anomaly-, signature-, and hybrid-based approaches to provide a comprehensive overview of network IDS’s state of the art. The articles were retrieved from seven databases (ScienceDirect, SpringerNature, IEEE, MDPI, Hindawi, PeerJ, and Taylor & Francis) which cut across various reputable journals and conference Proceedings. Among the 776 pieces of the literature identified, 71 were selected for analysis and synthesis to answer the research questions. Based on the research findings, we identified unexplored study areas and unresolved research challenges. In order to create a better IDS model, we conclude by presenting promising, high-impact future research areas.

### Accuracy ranges for Techniques for Anomaly based IDS

| Techniques         | No. of study | Accuracy range (%) |
| ------------------ | ------------ | ------------------ |
| CNN                | 6            | (87–99)            |
| RF                 | 6            | (83.1–99.9)        |
| AdaBoost           | 5            | (98.9–99.3)        |
| SVM                | 5            | (96.2–99.9)        |
| CNN + LSTM         | 4            | (76.8–95.6)        |
| AE                 | 3            | (87.2–99.7)        |
| DBN                | 3            | (87.2–98.1)        |
| DT                 | 3            | (85.2–99.9)        |
| ANN                | 3            | (76.9–99.9)        |
| NB                 | 2            | (99.0–99.7)        |
| AE + DNN           | 2            | (89.0–99.9)        |
| CNN + AE           | 1            | (100)              |
| Light GBM Ensemble | 1            | (99.9)             |
| SVM + NB           | 1            | (99.3)             |
| ABC + AFS + CART   | 1            | (99.0)             |
| KNN                | 1            | (99.0)             |
| LSTM + RNN         | 1            | (98.8)             |
| XGBoost + DNN      | 1            | (97.0)             |
| KELM               | 1            | (95.8)             |
| RNN                | 1            | (94.5)             |
| LSTM               | 1            | (87.0)             |
| XGBoost            | 1            | (87.0)             |
| LR + SVM           | 1            | (86.0)             |

### Dataset usage by studies
| Datasets        | No. of study |
| --------------- | ------------ |
| NSL-KDD         | 25           |
| KDDCup99        | 19           |
| UNSW-NB15       | 17           |
| CICIDS2017      | 8            |
| CSECIC-IDS2018  | 4            |
| ADFA-LD         | 2            |
| CICIDS-001      | 2            |
| DARPA           | 1            |
| ISCX-IDS        | 1            |
| Kyoto 2006 +    | 1            |
| Network TON-IOT | 1            |
| RTNTP18         | 1            |
| UGR16           | 1            |

### Strengths and limitations of ML/DL methods

| ML/DL methods | Pros                                                                                                                                                                                                                  | Cons                                                                                                                                                                                                                    |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| NB            | Few samples are required for training. It can perform binary and multi-label classification. It exhibit robustness towards irrelevant features                                                                        | interdependencies between features is not taken into account for classification purposes, therefore affects its accuracy                                                                                                |
| KNN           | It is Simple to use                                                                                                                                                                                                   | It is quite challenging to determine the optimal value of K and identify missing nodes. Also, Prediction computation can be expensive                                                                                   |
| DT            | It is simple and easy to use                                                                                                                                                                                          | Huge storage is required. High computational complexity. It is easier to use only when few DTs are used. Another difficult concern in DT is over-fitting                                                                |
| SVM           | Highly scalable for its simplicity. Capable of detecting network anomalies in real-time, works well with learning online. It is suitable for data with large number of feature attributes. Lesser storage is required | The optimal kernel function used in separating data when it is not linearly separable remains an obstacle towards achieving desired classification speed. In the vicinity of the hyperplane, SVM are sensitive to noise |
| RF            | It results in a more robust and accurate result that is resistant to overfitting. Fewer inputs are required and process of feature selection is not required                                                          | The use of RF may be impractical in real-time applications that require large dataset; this is because RF constructs several DTs                                                                                        |
| DBN           | Suitable for vital feature extraction with training on unlabeled data                                                                                                                                                 | High computational costs                                                                                                                                                                                                |
| EL            | It is robust to overfitting. Performs better than a single classifier. It reduces variance. Performs better in uncertain environments with a high number of features                                                  | Increased time complexity, due to the use of multiple classifiers in parallel                                                                                                                                           |
| RNN           | It is best-suited in environments where data are to be processed sequentially                                                                                                                                         | The problem of vanishing gradients, which hinders learning of long data sequences                                                                                                                                       |
| CNN           | It is suitable for effective feature extraction from raw data. It possess good potential in network security application                                                                                              | High computational complexity, Consequently, it is difficult to implement them in a situation with limited resources                                                                                                    |
| AE            | It is very effective for feature extraction and dimensionality reduction                                                                                                                                              | It is computationally heavy. It may yield undesired results when the training dataset is not representative of the testing dataset                                                                                      |
| RBM           | Feedback function of RBM facilitates the extraction of discriminative features from large and complex datasets which are then used to capture the behavior of the network traffic                                     | Single RBM lacks the capability of feature representation<br><br>High computational resources                                                                                                                           |
| LSTM          | designed to address concerns with bursting or vanishing gradients                                                                                                                                                     | Training is expensive in terms of both time and resources                                                                                                                                                               |
| ELM           | Extremely quick rate of learning. For real-time retraining, they are intriguing                                                                                                                                       | They are less reliable than conventional networks                                                                                                                                                                       |
| FCM           | It provides a more practical approach to addressing patterns and can identify potential outliers                                                                                                                      | The FCM can result in a local minimum                                                                                                                                                                                   |
| PCA           | Leads to a reduced training time                                                                                                                                                                                      | It is an attribute reduction technique that should be used in conjunction with additional prediction techniques to find incursions                                                                                      |
| XGBoost       | able to withstand overfitting, and full use of the computing resources                                                                                                                                                | May struggle when dealing with outliers                                                                                                                                                                                 |
| LightGBM      | Quick training and little memory utilization                                                                                                                                                                          | Light GBM divides the tree along the leaves, which might cause overfitting because it results in trees that are more complicated. Since light GBM is susceptible to overfitting, it is likely to overfit little data    |

### Challenges and potential future directions 
Network IDSs have been the subject of numerous studies and research papers that have been published. In response to RQ 6, the use of ML and DL algorithms for anomaly based network intrusion detection systems, in particular, still faces several open research hurdles and problems. 
 - The *problem* is that there ***isn’t*** a _common mechanism_ that ensures the proposed systems’ or *method’s validity*. The majority of research studies provide evaluation of the suggested systems using *simulated datasets*, which may not be applicable to real-world situations with real data and other challenges. As demonstrated by this study and others like it on the state of the art in IDS, 
	 - it is highly challenging to build an IDS which encompasses, at least, the most important aspects of an effective IDS, namely, 
	 - It can be quickly deployed online, is scalable, effective with real data, and meets the requirements of all stakeholders. 
	 - Instead, the majority of the published work presents results using *biased parameters*, covers only a *small portion of the system*, and shares evaluation results tested on *fabricated datasets*. 
 - In the context of signature-based IDS, a variety of techniques, such as pattern matching and rule-based algorithms, have been documented in the literature with the primary focus on accelerating the process of matching signatures (time complexity), 
	 - while researchers paid ***little*** *attention to space complexity* (memory consumption), especially when there is an increasing size in database. 
	 - Due to the many measurements, datasets, and simulation environments, it is difficult to compare the performances of these methodologies. 
	 - The pattern matching or signature search processes, however, need greater memory and search time in current techniques. 
	 - As a result, this necessitates an enhanced strategy that can optimize memory usage and processing time. 
 - For hybrid-based IDSs explored in the literature, only seven studies were found in this regard. 
	 - The studies under review didn’t provide sufficient information on the attacks detected, as multiclass classification was not employed. 
	 - In addition, there is a lack of sufficient background information on how the whole system has been integrated and evaluated. 
 - Furthermore, it is extremely difficult to define or achieve a demonstration of the accuracy and completeness of any proposed IDS. 
	 - As a result, this study’s key finding is that **it is challenging to create an all-encompassing IDS that provides high levels of accuracy, scalability, resilience, and threat prevention.** 
	 - The main problems and difficulties that scholars deal with now and in the future are discussed below. 
	 - *Future research* in this field has a *huge potential*, especially in *hybrid*-based intrusion detection that uses *Signature and Anomaly approaches*. 
	 - Although there has been a lot of study done in the IDS setting, the following factors of the *most recent* Network IDS *issues* can be *taken into account* in future studies: 
		 - A *high-quality dataset* is absolutely necessary to test and validate proposed NIDS. 
			 - Such a dataset should include a *sizable amount of network traffic data* with labels that describe both attack and regular behavior. 
			 - We advise that future investigations assess the effectiveness of intrusion detection techniques utilizing *more recent* intrusion detection *datasets*, such as CIRA-CIC-DoHBrw 2020 dataset. 
			 - In order to confirm the viability of their strategy, researchers should also try to experiment with some *genuine datasets*, such the ISOT CID dataset. 
			 - In addition, researchers should try to experiment with some *real datasets*, such as the ISOT CID dataset, to ensure the validity of their approach. 
		 - It is extremely *difficult* to develop an online, *real-time network IDS.* This is due to the fact that an IDS of this type would *need* to first *understand regular behavior* in order to detect anomalous or malicious behavior. The *learning phase* presupposes the *absence of noise and attack traffic,* which ***cannot be guaranteed***. If these problems are not resolved, such an IDS *can cause false alarms*. 
		 - The majority of anomaly-based NIDS attempt to build a *model* that *captures* the profile of ***every potential action*** or pattern of *regular traffic*. 
			 - This is particularly difficult, though, as it has been demonstrated that these models have a tendency to *favor the dominating class*, leading to large false-positive rates. 
			 - Additionally, it is ***impossible*** *to catch* ***every*** single potential *normal observation* that might be produced in a network, which raises the rate of false-negative results. 
			 - Another research goal is to completely prevent or reduce false-positive and false-negative rates in NIDS. 
		 - During various phases of the design and implementation of NIDS, computational complexity increases, such as feature reduction and data preprocessing, model training, and deployment, in particular, ML- and DL-based NIDS. 
			 - Consequently, creating an effective NIDS with minimal computational requirements is a challenge and a potential field for future research. 
		 - The feature selection and dimensionality reduction techniques employed in the proposed IDSs are appropriate for a particular sort of normal traffic and a specific type of attack detection, but they could not be effective if the environment for normal or attack sequences changes somewhat. 
			 - **Therefore, a major research goal is to develop a dynamic and computationally efficient technique for feature selection that can operate in all kinds of normal and attack traffic.** 
		 - For the purpose of training a model on a sizable dataset, DL and ML approach are frequently employed. 
			 - This has made it easier to handle cyber-attacks effectively. 
			 - However, some issues regarding the application of DL and ML approach for attack detection in networks require the attention of researchers; for instance, 
				 - the *issue of resource limitations* limits the application of DL/ML algorithms for network security. 
				 - *Scalability problems*, such as those related to various scenarios and IDS deployment options, are another difficulty with the use of ML/DL techniques in large, distributed networks. 
			 - *One possible solution* to limitations of individual deep or machine learning methods as recommended by some of the authors is the usage of an *ensemble of ML/DL algorithms* that outperform a single machine learning algorithm. 
			 - However, because these algorithms were computationally expensive, they caused *network latency problems*, which are un-affordable in critical network environments. 
		 - The methods of *semi-supervised* learning, *transfer* learning, and *reinforcement* learning (RL) have ***not*** yet *been thoroughly investigated* and tested for creating an IDS for network security. 
			 - Therefore, future research may focus on the semi-supervised learning, transfer learning, and reinforcement learning (RL) techniques for creating an IDS for network security so as to accomplish crucial goals like real-time, quick training, and unified models for anomaly detection. 
			 - Additionally, combining RL with DL would make for an intriguing research topic because their combined use may be advantageous in network systems with enormous data dimensionality and non-stationary situations. 
		 - Finally, it would be *interesting* *if* more studies can *focus* on development of a *hybrid* *system* that combines techniques of *signature* and *anomaly*-*based* IDS, as it is evident from literature that this aspect has ***not*** *been thoroughly investigated* and tested for creating IDS.

### Conclusion
In this work, a survey of anomaly-, signature-, and hybrid-based IDS has been presented. 
 - This work attempts to provide the researchers with the summarized but comprehensive and useful insight into the various security challenges currently being faced and possible solutions, with a focus on network intrusion detection. 
This study adheres to Preferred Reporting Items for Systematic Reviews and Meta-Analyses (PRISMA) standards. 
 - Literature on signature-based, anomaly-based, and hybrid-based network intrusion detection was organized and summarized according to a set of predefined keywords and RQs. 
 - A total of 71 articles were chosen for the review after the exclusion, inclusion, and quality criteria were applied. 
 - This study gave insight into what may be learned from existing research on hybrid-, anomaly-, and signature-based network intrusion detection. 
 - Additionally, it compared methodology, datasets, types of attacks detected, evaluation metrics, performance and limitations of each contribution. 
The analysis of the SLR has shown that there has been *a tremendous shift from signature-based towards the anomaly-based approach* in terms of research studies; 
 - however, *the field of hybrid-based approach has minimal focus* by researchers. 
 - The study further shows that different machine learning and deep learning algorithms have been deployed by researchers for intrusion detection, among which *the commonly used ones* include CNN, ANN, DBN, AE, AdaBoost, LSTM, RF, and SVM, while in terms of *accuracy*, *CNN+AE* was reported to *yield better performance*. 
In the analyzed studies, thirteen types of datasets were used for evaluating the models. 
 - *KDDCup99 and NSL-KDD* were the *most used dataset*, followed by the *UNSWNB15*. 
 - These datasets have been *criticized* by researchers for being *out of date* because they ***do not*** *reflect the contemporary sorts of assaults*, despite their high recorded popularity. 
 - To this end, the SLR analysis revealed *emerging datasets* that contain *modern day attacks*. 
 - These include CIRA-CIC-DoHBrw 2020, ISOT CID, CICIDS2017, ADFA-LD, ISCX-IDS, RTNTP18, UGR16, and CSE-CIC-IDS2018 datasets. 
 - **Therefore, it is important for researchers to utilize modern datasets in order to attain an effective IDS.** 
*For anomaly-based IDS*, it was evident that deep learning (DL) techniques are now the current trend. 
 - Majority of the reviewed literature applied deep learning techniques. 
 - In terms of performance, there was report of *nearly 100% performance, based on CNN and AE*. 
 - However, when considering the various attack types found in the datasets, it is essential to note that the *FAR needs to be reduced to the minimum.* 
 - We suggest that studies *explore other datasets* with more *recent types of attacks*. 
 - Additionally, some DL *techniques* are *yet to be explored*, which gives room for further research to be done in this area. 
 - A *hybrid* of two or more techniques *may yield high detection accuracy* for attacks but may result in *high training time and resource consumption.*
 - **Therefore, we recommend that future research look into how a practical, lightweight anomaly-based IDS should be modeled, considering all the challenges mentioned above.** 
Several *methods* have been *proposed* to *speed up the process* of matching *signatures*.
 - In the context of signature-based IDS, pattern matching and *rule-based algorithms* are the most used in the literature. 
 - However, it is *challenging to compare* the performances of these approaches due to the *different metrics, datasets, and simulation environments*. 
 - Nonetheless, due to the pattern matching or signature search operations, *existing* techniques bear *more memory and searching time*. 
 - **Therefore, this calls for an improved approach that is capable of optimizing processing time and memory consumption.** 
*For hybrid-based IDSs* explored in the literature, *only seven studies* were found in this regard. 
 - The *studies under review* ***did not*** provide *sufficient information* on the attacks detected as *multi-class classification was **not** employed*. 
 - In addition, there is a *lack of* sufficient background *information* on *how* *the* whole *system* has been *evaluated*. 
 - **Therefore, there is a need to design a hybrid system that overcomes the aforementioned reported issues.** 
Further analysis of the review reveals that while *processing time* and *memory usage* were *employed for signature-based IDS* performance evaluation; *accuracy, precision, and FAR* were the three *most often used* metrics *for anomaly based IDS*. 
 - *Future research* should think about *including all different performance indicators*, especially detection time, which will be crucial for real-time systems. 
 - *IDS models should* also be able to *adapt to the dynamic nature* of the network environment; **this calls for models that can autonomously learn their surroundings and update themselves**.

# Hybrid IDS papers
[[s2 ref 135|135]]
[[s2 ref 73|73]]
[[s2 ref 85|85]]
[[s2 ref 136|136]]
[[s2 ref 137|137]]
[[s2 ref 138|138]]
[[s2 ref 9|9]]

| Paper                                                                                                                                                                                                                                                                                                                                                                                 | Year | Methodology                             | Dataset                                            | Metrics                                                             | Pros                                                                                        | Cons                                                                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---- | --------------------------------------- | -------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| [[9](https://link.springer.com/article/10.1007/s10207-023-00682-2#ref-CR9 "Sohi, S.M., Seifert, J.-P., Ganji, F.: RNNIDS: enhancing network intrusion detection systems through deep learning. Comput. Secur. 102, 102151 (2021). <br>https://doi.org/10.1016/j.cose.2020.102151")]                                                                                                   | 2020 | RNN LSTM<br><br>Bro Signature Analyzer  | N/A                                                | TPR: 96.4<br><br>FNR: 4.1<br><br>FAR: 2.7                           | Good detection rate for zero-day attacks                                                    | High false positive                                                                                                                   |
| [[136](https://link.springer.com/article/10.1007/s10207-023-00682-2#ref-CR136 "Liu, J., et al.: Adaptive intrusion detection via GA-GOGMM-based pattern learning with fuzzy rough set-based attribute selection. Expert Syst. Appl. 139, 112845 (2020). <br>https://doi.org/10.1016/j.eswa.2019.112845")]                                                                             | 2020 | FRS-FS<br><br>GA-GOGMM                  | NSL-KDD, Nidsbench-based                           | DR: 96.5<br><br>FAR: 1.4                                            | Low false positive and missing rate                                                         | Low accuracy for known and unknown attacks                                                                                            |
| [[138](https://link.springer.com/article/10.1007/s10207-023-00682-2#ref-CR138 "Ugtakhbayar, N., Usukhbayar, B., Baigaltugs, S.: A Hybrid model for anomaly-based intrusion detection system. In: Pan, J.-S., Li, J., Tsai, P.-W., Jain, L.C. (eds.) Advances in Intelligent Information Hiding and Multimedia Signal Processing, pp. 419–431. Springer Singapore, Singapore (2020)")] | 2020 | Snort + Naïve Bayes                     |                                                    |                                                                     | An increased execution speed with decreased processing time                                 | Low detection accuracy rate, and huge resource consumed                                                                               |
| [[135](https://link.springer.com/article/10.1007/s10207-023-00682-2#ref-CR135 "Kaur, S., Singh, M.: Hybrid intrusion detection and signature generation using deep recurrent neural networks. Neural Comput. Appl. 32(12), 7859–7877 (2020). <br>https://doi.org/10.1007/s00521-019-04187-9")]                                                                                        | 2019 | rule-based approach and RNN using LSTM  | CICIDS 2017, NSL-KDD                               | TPR: 99.4<br><br>AC: 99.1<br><br>TNR: 99.2                          | High detection accuracy rate                                                                | Time expended by the model is relatively high, also imbalance nature of data leads to low detection of some specific kinds of attacks |
| [[137](https://link.springer.com/article/10.1007/s10207-023-00682-2#ref-CR137 "Kalavadekar, P.N., Sane, S.S.: Building an effective intrusion detection system using combined signature and anomaly detection techniques. Int. J. Innov. Technol. Explor. Eng. 8(10), 429 (2019)")]                                                                                                   | 2019 | DT, Association rule mining, GA         | DARPA,KDDCup99, NSL-KDD, UGR16<br><br>Kyoto 2006 + | AC:99.9<br><br>DR: 99.8<br><br>FAR:0.2                              | Enhanced detection performance                                                              | Different attack types were not explored                                                                                              |
| [[73](https://link.springer.com/article/10.1007/s10207-023-00682-2#ref-CR73 "Abbasi, J.S., Bashir, F., Qureshi, K.N., Najam ul Islam, M., Jeon, G.: Deep learning-based feature extraction and optimizing pattern matching for intrusion detection using finite state machine. Comput. Electr. Eng. 92, 107094 (2021). <br>https://doi.org/10.1016/j.compeleceng.2021.107094")]       | 2021 | AE, SVM<br><br>Snort AC Rules Algorithm | NA                                                 | PT:1.6us/100byte<br><br>TP:621,118/100byte<br><br>MU:682.7 Mb/5byte | An improved time complexity to process each packet                                          | Only detects few types of attacks                                                                                                     |
| [[85](https://link.springer.com/article/10.1007/s10207-023-00682-2#ref-CR85 "Kim, G., Lee, S., Kim, S.: A novel hybrid intrusion detection method integrating anomaly detection with misuse detection. Expert Syst. Appl. 41(4), 1690–1700 (2014). <br>https://doi.org/10.1016/j.eswa.2013.08.066")]                                                                                  | 2014 | C4.5 decision tree (DT), 1-class SVM    | NSL-KDD                                            | PT: 11.2 s                                                          | High detection performance for unknown attacks, low processing time, and less training time | Degraded profiling ability<br><br>Uneven data distribution leading to high training and testing time                                  |


