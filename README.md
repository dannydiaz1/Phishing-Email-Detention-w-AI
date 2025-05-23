# Email Sceurity w/AI

##**Project Purpose**

Phishing attacks pose a significant cybersecurity threat, leading to financial losses and data breaches. Traditional email filters struggle to detect sophisticated phishing attempts, leaving users vulnerable. This project aims to develop an AI-powered phishing email detection system that enhances email security by accurately identifying phishing emails using machine learning and natural language processing (NLP) techniques. Given the rising complexity of phishing schemes, improving automated detection is critical for individuals, businesses, and organizations. The objective is to minimize false negatives, ensuring that malicious emails are effectively flagged while legitimate messages are accurately classified, reducing the risk of user compromise.

##**Method**

This project leverages machine learning models such as Support Vector Machines (SVM), XGBoost, and LightGBM to classify emails as phishing or legitimate. Using publicly available phishing and spam datasets, email text features are processed using TF-IDF vectorization. The goal is to deploy the model as an API that integrates with email providers to filter suspicious messages.

Models were trained with ~80K emails sourced from the kaggle link below. The AI systems then determined patterns in the emails’
subject, bodies, and whether a url was present in the text. 

##**Model Performance**
The models were then compared based on their ability to classify emails as phishing. This was done using accuracy, precision,
recall, and F1-score, with recall being the most critical metric to minimize false negatives (missed phishing emails).

##**Results**

The Support Vector Machine (SVM) was the most effective model, achieving the highest recall (0.99) and F1-score (0.99).

Random Forest had the highest precision (0.99), reducing false positives, but its recall was slightly lower (0.98).

AdaBoost performed the worst, with an accuracy of 77.7% and low precision (0.71), making it unreliable for real-world deployment.

Though the SVM had the best recall and F1-score, it is a computationally expensive model that would require extensive resources to deploy in a production environment. Therefore, the best option is the Random Forest. It scored highest in precision, its recall was only 0.01 behind the front-runner, and it is a light-weight model requiring significantly less resources than the SVM.

##**Considerations**

###Challenges & Limitations
**Computational Costs:** Advanced models (SVM, XGBoost, BERT) require significant processing power, which can impact real-time detection speed.

**Evolving Phishing Techniques:** Attackers constantly adapt, making it necessary to update models regularly. 

**False Positives & False Negatives:** While high recall minimizes false negatives, some legitimate emails may be wrongly classified as phishing.

###Future Improvements
Incorporate Deep Learning (BERT, NNs) for contextual understanding.

Real-Time URL Analysis & Sender Reputation Filtering to improve detection accuracy.

Adaptive Learning Systems that can retrain models automatically based on new phishing patterns.


	Model				Accuracy	Precision 	Recall      F1-Score
	Support Vector Machine		  0.9851	     0.98	  0.99	        0.99
	Logistic Regression		  0.9839	     0.98	  0.99	        0.98
	LightGBM			  0.9741	     0.96	  0.99	        0.98
	XGBoost				  0.9697	     0.95	  0.99	        0.97
	Random Forest			  0.9818	     0.99	  0.98	        0.98
	AdaBoost			  0.7771	     0.71	  0.97	        0.82
	Multinomial Naïve Bayes		  0.9657	     0.97	  0.96	        0.97



**Data source:**

Al-Subaiey, A., Al-Thani, M., Alam, N. A., Antora, K. F., Khandakar, A., & Zaman, S. A. U. (2024, May 19). Novel Interpretable and Robust Web-based AI Platform for Phishing Email Detection. ArXiv.org. https://arxiv.org/abs/2405.11619
 
	Kaggle link: https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset/data
