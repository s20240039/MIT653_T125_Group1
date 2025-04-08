## Application of Machine Learning in detection of Cyber-attacks on critical infrastructure with focus on Smart Grids

### Abstract
<p>The security of smart grids, or next-generation power grids with digital communication and control, has become increasingly significant as cyberattacks pose the threat to the reliability of these vital infrastructures. This review of literature covers the use of machine learning (ML) techniques in the identification of cyberattacks on smart grids, such as False Data Injection Attacks (FDIAs), Denial-of-Service (DoS/DDoS) attacks, anomaly detection for SCADA systems, and comprehensive cybersecurity frameworks. We synthesize results from 20 recent papers (mostly 2015–2025), contrasting their methodologies, results, strengths, and weaknesses. Supervised learning techniques (such as tree-based classifiers, deep neural networks) have achieved high accuracy in FDIAs detection, whereas deep advanced learning (such as autoencoders, graph neural networks) promise potential for real-time detection of stealthy intrusions and DDoS attacks [1], [2]. Unsupervised and hybrid models address the detection of novel attack patterns with minimal retraining [2]. We categorize the literature by attack type and defence strategy, identifying emerging trends such as the integration of domain knowledge (power system models, digital twins, knowledge graphs) with ML for improved resilience. Key research needs are interpretable and robust ML models that can react to evolving threats without affecting performance. Ethical needs—basically the robustness, interpretability, and accountability of AI-informed decisions in core grid operations—are set as a condition for field deployment. The article concludes with suggestions for future work, including supporting hybrid approaches, better testbeds and datasets, and explainable AI adoption to render ML-based defences reliable and well-applied within smart grid defence frameworks.</p>

### Keywords
Machine Learning, Cybersecurity, Smart Grids, Cyber-attack, Artificial Intelligence, Intrusion Attacks, Anomaly Detection, Power Grids, Critical Infrastructure

### Table of Contents
[ABSTRACT](#abstract)<br/>
[KEYWORDS](#keywords)<br/>
[INTRODUCTION & BACKGROUND](#Introduction-&-Background)<br/>
[PURPOSE & AIMS OF THE LITERATURE REVIEW](#Purpose-&-Aims-of-the-Literature-Review)<br/>
[LITERATURE REVIEW PROCESS](#Literature-Review-Process)<br/>
[MAIN BODY OF THE LITERATURE REVIEW](#Main-Body-of-the-Literature-Review)<br/>
[MACHINE LEARNING IN SMART GRIDS]<br/>
[ANOMALY DETECTION IN SCADA SYSTEMS]<br/>
[CYBER-ATTACK DETECTION IN SMART GRIDS WITH MACHINE LEARNING]<br/>
[DENIAL-OF-SERVICE (DOS) ATTACKS IN SMART GRIDS NETWORKS]<br/>
[STRENGTH](#Strength)<br/>
[WEAKNESS](#Weakness)<br/>
[CONFLICTING FINDINGS](#Conflicting-Findings)<br/>
[CONCLUSION](#Conclusion)<br/>
[REFERENCES](#References)<br/>



### Introduction & Background
<p>Modern smart grids employ two-way digital communication, IoT sensors, and automation to improve power delivery efficiency and reliability. However, this higher connectivity exposes the power grid to cyber-attacks as well. Cyber-attacks on electrical power grids will cause operations to stop, generate blackouts, and provide economic damage, as exemplified with real incidents like the 2015 and 2016 attacks on the Ukrainian power grid. The attacker used contaminated information by means of malware (e.g., BlackEnergy 2007) in order to conceal the grid status and then create an outage in 2015's incident [3]. This, and other attacks (e.g., Stuxnet 2010, Industroyer 2016), indicate the susceptibility of critical power infrastructure to sophisticated attacks and highlight the need for sophisticated detection and mitigation strategies [4], [5]. </p>
<p>Machine learning provides an appealing prospect for enhancing smart grid cybersecurity since it can learn patterns and anomalies on vast amounts of data. Unlike rule-based intrusion detection systems based on pre-determined signatures, ML-based approaches can potentially identify zero-day attacks and subtle intrusion patterns by learning from experience. For smart grids, which include components like smart meters, SCADA systems, substations, and wide-area measurement systems, ML algorithms have been employed to detect various types of cyberattacks: </p>
<ul><li> FDIAs: where an attacker silently alters sensor or measurement data to mislead grid control systems. </li>
<li> DoS/DDoS attacks: which flood communication networks to shut down grid monitoring or control. </li>
<li> SCADA/ICS anomaly attacks: like remote tripping commands, replay attacks, and other intrusions that affect industrial control systems controlling the grid. </li></ul>
<p>Security of the smart grid is a national security issue, and using AI/ML for real-time detection is a research area. Recent studies have demonstrated high success rates in detection of certain attacks (usually well above 95% detection rate in lab experiments), but there are challenges in bringing these into operational live grid environments [6]. This Introduction has outlined the context of the topic and the threat environment. The following sections will outline the purpose of this review, the literature selection methodology, and an exhaustive overview of state-of-the-art ML application in smart grid attack detection.</p>

### Purpose & Aims of the Literature Review
<p>The objective of this review of literature is to abstract and critically evaluate recent research (published within the last 5–10 years) on machine learning techniques for detecting cyberattacks in smart/power grids. The study will aim to provide a comprehensive overview of different vulnerabilities and how recent analysis addressed the major issues involving these attacks.</p>
<p>Key Findings: Provide an overview of the major findings and outcomes of 20 shortlisted studies using ML for securing smart grids. We will identify what each contributes, such as methodologies and performance outcomes.</p>
<p>Thematic Synthesis: Organize the literature by thematic themes:
(1)	False Data Injection Attack detection
(2)	DoS/DDoS attack detection
(3)	SCADA/ICS anomaly detection
(4)	Broader cybersecurity models for smart grids.
The thematic categorization will reveal patterns and similarities across studies using different evidence and graphs that corresponds to the relationship of the data gathered. Providing various approaches will give the study a broad perspective on how these attacks can impact the Smart Grid systems.</p>
<p>Recent Trends: Recent trends in research and emerging methods (e.g., use of deep learning, graph-based approaches, hybrid techniques) in securing smart grids. The study will also look at how the field has evolved in the past decade, from early anomaly detectors to the present-day intelligent, real-time systems.</p>
<p>Critical Comparison: Critically compare the strengths and limitations of different approaches. For example, supervised vs. unsupervised learning approaches comparison, or analysis of what algorithm to use against stealthy vs. noisy attacks. Real-life considerations such as real-time performance, complexity of deployment, and false positives are analysed.</p>
<p>Identify Gaps: Highlight gaps in research in existing literature. While progress has been made, there are certain areas like attack adaptability, explainability, availability of representative datasets that are still lacking. The study will aim to highlight the areas where more research is needed.</p>
<p>Future Directions: Based on the gaps and trends that have been uncovered, together with the suggested future research directions. This study is about showing how existing limitations can be overcome and outlining how newer technologies like explainable AI, federated learning, or digital twins could be applied within future solutions.</p>
<p>Ethics Aspects: Have in mind the governance and ethical applications of Artificial Intelligence and Machine Learning considering the sector of critical infrastructure specifically the Smart Grid systems. Thus, our assessment not only includes technical competencies but employs these technologies also in an ethical manner including explainability, manipulation resistance by means of adversarial robustness and accountability for choices.</p>
<p>By obtaining these goals, the study hopes to inform researchers, practitioners, and stakeholders of the status of smart grid cybersecurity with machine learning and how to direct future research to secure power infrastructure against cyberattacks.</p>

### Literature Review Process
Scope Definition
We defined the scope to focus on machine learning applications for cyberattack detection in power systems, specifically smart grids and related industrial control systems. 
Research question
Application of machine learning in detection of cyberattacks on critical infrastructures with focus on power grids/smart grids.
Database search and search term use
We searched the following academic database for the peer reviewed articles and conferences.
•	IEEE Xplore
•	Google Scholar
Use of keywords and Boolean operator in search of related papers are:
•	Smart grids AND machine learning AND cyber security
•	False data injection AND power system and AI
•	Smart meters AND cyber threats
•	Anomaly Detection AND Smart meter AND Machine learning
•	SCADA AND deep learning
Initial filtration
The search gave us numerous papers that were filtered according to relevance and quality. In this case, our priorities were first on peer-reviewed journals and next high-quality conference papers. Subsequently, any duplicates or out-of-scope papers (focusing on non-ML techniques or unrelated IoT domains) were excluded.
Inclusion and exclusion criteria 
Inclusion criteria:
•	Journal articles, books or conferences
•	Published range, 2020 to 2025
•	Focused on Machine learning applications to detect cyberthreats on smart grids
•	Papers written in English
Exclusive criteria:
•	Papers not related to smart grids, machine learning
•	Published before 2020
•	Articles not reviewed by the peers such as blogs, opinion
•	Reports involving different attacks on the field

### Main Body of the Literature Review
Machine Learning in Smart Grids 
As the world's electricity demand rises due to urbanisation and population development, machine learning (ML) in smart grids has become increasingly important. By the year 2040, the demand for electricity will increase tremendously such that it will only mark an impending state of failure of existing power systems for smart, efficient, and reliable power systems. Smart grids are answers to making electrical networks more reliable and secure through the application of computational technologies and data analytics.
There has been an increasing infrastructure for Research in ML Applications in Smart Grids during the years 2017 through 2019. Neural Networks and Support Vector Machines are two out of many techniques applied widely within various domains such as safety, energy management, and forecasting. One study used 108 research papers-a total of the works from the IEEE Xplore database- to extract which ML methods become most popular and other emerging trends in the field.
Such findings demonstrate the necessity of smart grids for any prospective energy concerns, especially in terms of data security and system reliability. The research work aims to enlighten the professionals and the regulatory authorities about how machine learning applications' role in smart grid technologies is acted towards an expansion, and further research in this direction will be required to cater to such electric systems [7].
Anomaly Detection in SCADA Systems
According to findings on the use of deep learning methods for anomaly detection in SCADA systems, various models have shown strong detection rates for an array of cyber-attacks. The LSTM/Bloom Filter model, for example, produced a detection rate of 92% and had a strong reputation for recognizing Denial of Service (DoS) and Probe attacks, all while heavy training time and insufficient training data prevented its use for User-to-Root (U2R) and Remote-to-Local (R2L) attacks. Whereas the Smart Grid Autoencoder model registered an outstanding 96% detection rate due to offline training with real-time monitoring, hence facilitating better identification performance across a wider attack range. The CNN/LSTM went on to achieve a commendable detection rate of 89% while exhibiting improved training efficiency, particularly due to the CNN segment. The Deep Belief Network (DBN) model attained a 94% detection rate, which translated into a striking efficiency in the detection of unknown attacks, especially for the purpose of electricity theft. This just exemplifies the different strengths of deep learning models in combating cyber threats in SCADA systems, whereas some models fit better under some kinds of attack scenarios.
The studies followed methodologies involving the use of deep learning architectures such as CNN-autoencoders (AE), LSTM networks, and DBN. These models were characterized under the framework of intrusion detection systems (IDSs) as anomaly, signature, or hybrid. The evaluation of the efficiency of each model was conducted based on their capacity to identify and detect a certain category of cyber-attacks within the SCADA environment. The evaluation method involved extensive testing, comparing the performances of each model, and discussing issues that were faced by each approach mainly concerning training time and data limitations. 
To summarize, deep learning methods have stood the test for their efficacy in anomaly detection in SCADA systems, and the issue of extended training times and scant data should be considered in the subsequent research study. Distributed methods can be deployed to address all the above-mentioned challenges, making the system resilient and powerfully programmed to assess cyber-attacks on vital infrastructures [8].
Cyber-Attack Detection in Smart Grids with Machine Learning 
Machine Learning particularly via ANN methods has shown to be a good bet for infection detection in smart grid cyber-attacks. The ANN model proved better than the many widely used algorithms in achieving an F1 score above .95 in all datasets like Logistic Regression and Random Forest. It is most pronounced in the classification of faults into three categories: Attack, Natural, and No Event, showing that the ANN model is the best for finding a way through regular operations to cyber threats. The study further proved the model's greater precision and recall for different types of faults.
The methodology consists of a four-layered ANN used for recognizing faults, which was further enhanced by rigorous pre-processing methods to increase its efficiency. The dataset, extracted from a 3 bus 2-line system and including data from 15 machines, was split into 80% for training and 20% for testing purposes. It was performed Feature Extraction on the most relevant 24 out of the 29 measurements acquired from PMUs (Phasor Measurement Units) to achieve relevant features for classification. Thus, the training database would be a thorough one that conditions the model to fault classification.
Lastly, the study thus argued that the ANN model could be relied on for classifying disturbances in the power system, but it also pointed out that the larger datasets needed to be used in future studies to increase the reliability of the model and help reduce the high rate of false positives, stating that future work might possibly make the model more refined [9].
Denial-of-Service (DoS) attacks in smart grids Networks
It is very concerning how the smart grid control systems, especially Load Frequency Control (LFC), are very susceptible to Denial of Service (DoS) attacks. The research found a considerable alteration in the system performance owing to the timing of DoS attacks. If an attack is carried out during the transient phase of operation, prior to the system stabilization, a considerable disruption may occur; attacks after the system stabilizes have a lesser impact. Additionally, this paper points out the mathematical characterization of DoS attacks and signature identification that can be exploited for system destabilization.
The proposal consisted of representing the attacks under the switched system approach, where the absence of communication was expressed in binary signals while implementing the theory of switched systems to study stability and performance degraded by cyber-attacks. The whole system dynamics were captured in state space, and important performance indicators such as convergence time and steady-state error were assessed through simulations.
In conclusion, it was reiterated by the study that the LFC systems are significantly vulnerable to DoS attacks, especially in their transient recovery phase. Therefore, smart grids should have cyber-resilience mechanisms such as real-time monitoring, redundant communication channels, and resilient control algorithms to contain the consequences of these attacks. Furthermore, this research feeds into the continued integration of cyber-physical security solutions for smart grid systems [10].

### Strength
Effective problem solving: Machine learning has been proved to be the most effective answer to common problems of smart grids in terms of security, reliability, and perhaps management of energy [7].
Utilization of diverse Algorithm: The use of a wide range of machine learning techniques, such as support vector machines and neural networks, has been effectively used in smart grid research, demonstrating a strong methodological framework [7].
Integration with cybersecurity: There is a growing trend in the application of machine learning techniques to enhance cybersecurity mechanisms in smart grids against discriminating between normal operations and possible cyber-attacks events [9].
Vulnerabilities identification: The research finds out major vulnerabilities in all aspects of spaces in smart grid infrastructure, physical security threats and complexity introduced by integration process of the IoT components [11].

### Weakness
Data Limitations: Insufficient datasets can constrain machine learning models and negatively impact their forecast accuracy, resulting in more missed detections of some cyber-attacks in smart grids [11].
Performance Gaps: While some models detect different attacks, others are better at identifying some specific attacks, suggesting room for improvement in this area [11].
Implication complexity: The challenges in integrating machine learning with existing systems relate to scalability and the ability to apply them in realistic settings [7].

Conflicting findings
Vulnerabilities and their mitigations: while there is a need for a robust cybersecurity for smart grids is recognized; however, there is a lack of specificity in addressing existent mitigation strategies, which may suggest that the vulnerabilities are acknowledged but not managed [11].
Impact of cyberattack: Cyber-attacks cause considerable financial and operational disruptions, there is a focus on the necessity of improved security and collaboration among the various stakeholders, suggesting that solutions might not be enough [7].

Conclusion
Recent studies have analysed the increasing number of papers and articles published relating to the application of ML around smart grids [7]. This is a clear indication of the high demand of a possible outcome evaluation in this important field. But is also a sign that there is still a lot of unanswered questions to the issues and concerns regarding the safety and protection of the Smart Grid system to different vulnerabilities and attacks.  As we all know, Energy is the most important resources in urbanization and the introduction of the Internet of Energy (IoE) that can collect, monitor and manage power grid would provide challenge than solution if not properly integrated and implemented [12]. Having said that the advancements of AI and ML in power/smart grids would require a lot of responsibility especially in safeguarding its operation, distribution and network. This study aims to uncover these threats and different vulnerabilities that is present to the Smart Grid system. Through detection and prevention of cyberattacks by identifying anomalies in the data and network traffic to training AI in identifying and mitigating false data that can be injected to the system which can affect certain areas of the operation, like power distribution, load forecasting, smart metering and data collection. 




### References
[1]	A. Ashok, M. Govindarasu, and V. Ajjarapu, “Online Detection of Stealthy False Data Injection Attacks in Power System State Estimation,” IEEE Trans. Smart Grid, pp. 1–1, 2016, doi: 10.1109/TSG.2016.2596298.
[2]	S. S. A. Naqvi, Y. Li, and M. Uzair, “DDoS attack detection in smart grid network using reconstructive machine learning models,” PeerJ Comput. Sci., vol. 10, p. e1784, Jan. 2024, doi: 10.7717/peerj-cs.1784.
[3]	“Cyber-Attack Against Ukrainian Critical Infrastructure | CISA.” Accessed: Apr. 08, 2025. [Online]. Available: https://www.cisa.gov/news-events/ics-alerts/ir-alert-h-16-056-01
[4]	© Stanford University, Stanford, and California 94305, “Stuxnet: The world’s first cyber weapon.” Accessed: Apr. 08, 2025. [Online]. Available: http://cisac.fsi.stanford.edu/news/stuxnet
[5]	N. Sahani, R. Zhu, J.-H. Cho, and C.-C. Liu, “Machine Learning-based Intrusion Detection for Smart Grid Computing: A Survey,” ACM Trans. Cyber-Phys. Syst., vol. 7, no. 2, pp. 1–31, Apr. 2023, doi: 10.1145/3578366.
[6]	T.-H. Chua and I. Salam, “Evaluation of Machine Learning Algorithms in Network-Based Intrusion Detection Using Progressive Dataset,” Symmetry, vol. 15, no. 6, p. 1251, Jun. 2023, doi: 10.3390/sym15061251.
[7]	T. S. Bomfim, “Evolution of Machine Learning in Smart Grids,” in 2020 IEEE 8th International Conference on Smart Energy Grid Engineering (SEGE), Oshawa, ON, Canada: IEEE, Aug. 2020, pp. 82–87. doi: 10.1109/SEGE49949.2020.9182023.
[8]	H. C. Altunay, Z. Albayrak, A. N. Ozalp, and M. Cakmak, “Analysis of Anomaly Detection Approaches Performed Through Deep Learning Methods in SCADA Systems,” in 2021 3rd International Congress on Human-Computer Interaction, Optimization and Robotic Applications (HORA), Ankara, Turkey: IEEE, Jun. 2021, pp. 1–6. doi: 10.1109/HORA52670.2021.9461273.
[9]	A. Talati, V. Garg, N. Mishra, P. Tiwari, and P. Jena, “Cyber-Attack Detection in Smart Grids Using Machine Learning Approach,” in 2023 7th International Conference on Computer Applications in Electrical Engineering-Recent Advances (CERA), Roorkee, India: IEEE, Oct. 2023, pp. 1–6. doi: 10.1109/CERA59325.2023.10455586.
[10]	S. Liu, X. P. Liu, and A. El Saddik, “Denial-of-Service (dos) attacks on load frequency control in smart grids,” in 2013 IEEE PES Innovative Smart Grid Technologies Conference (ISGT), Washington, DC, USA: IEEE, Feb. 2013, pp. 1–6. doi: 10.1109/ISGT.2013.6497846.
[11]	B. Paul et al., “Potential smart grid vulnerabilities to cyber attacks: Current threats and existing mitigation strategies,” Heliyon, vol. 10, no. 19, p. e37980, Oct. 2024, doi: 10.1016/j.heliyon.2024.e37980.
[12]	I. Demir, O. Ileri, and O. F. Ertuurul, “The Core of a Smart Grid: Internet of Energy and Machine Learning,” in 2022 Global Energy Conference (GEC), Batman, Turkey: IEEE, Oct. 2022, pp. 357–360. doi: 10.1109/GEC55014.2022.9987139.




