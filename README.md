# Email Sceurity w/AI

**Project Purpose**

Phishing attacks pose a significant cybersecurity threat, leading to financial losses and data breaches. Traditional email filters struggle to detect sophisticated phishing attempts, leaving users vulnerable. This project aims to develop an AI-powered phishing email detection system that enhances email security by accurately identifying phishing emails using machine learning and natural language processing (NLP) techniques. Given the rising complexity of phishing schemes, improving automated detection is critical for individuals, businesses, and organizations. The objective is to minimize false negatives, ensuring that malicious emails are effectively flagged while legitimate messages are accurately classified, reducing the risk of user compromise.

**Method**

This project leverages machine learning models such as Support Vector Machines (SVM), XGBoost, and LightGBM to classify emails as phishing or legitimate. Using publicly available phishing and spam datasets, email text features are processed using TF-IDF vectorization. The goal is to deploy the model as an API that integrates with email providers to filter suspicious messages. 

**Outcome**

Preliminary results show high accuracy (~98%) and strong recall (~99%), effectively detecting phishing emails while minimizing false negatives. The goal is to integrate the system with existing email APIs to automatically filter phishing emails into spam folders. Future enhancements include advanced deep learning models (such as BERT), real-time phishing link analysis, and sender reputation filtering. 

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
