# Email Sceurity w/AI

**Project Purpose**

Phishing attacks pose a significant cybersecurity threat, leading to financial losses and data breaches. Traditional email filters struggle to detect sophisticated phishing attempts, leaving users vulnerable. This project aims to develop an AI-powered phishing email detection system that enhances email security by accurately identifying phishing emails using machine learning and natural language processing (NLP) techniques. Given the rising complexity of phishing schemes, improving automated detection is critical for individuals, businesses, and organizations. The objective is to minimize false negatives, ensuring that malicious emails are effectively flagged while legitimate messages are accurately classified, reducing the risk of user compromise.

**Method**

This project leverages machine learning models such as Support Vector Machines (SVM), XGBoost, and LightGBM to classify emails as phishing or legitimate. Using publicly available phishing and spam datasets, email text features are processed using TF-IDF vectorization. The goal is to deploy the model as an API that integrates with email providers to filter suspicious messages. 

**Outcome**

Preliminary results show high accuracy (~98%) and strong recall (~99%), effectively detecting phishing emails while minimizing false negatives. The system can be integrated with Gmail and Outlook APIs to automatically filter phishing emails into spam folders. Future enhancements include advanced deep learning models (such as BERT), real-time phishing link, and introduce sender reputation filtering. 


**Data source:**
	- *Al-Subaiey, A., Al-Thani, M., Alam, N. A., Antora, K. F., Khandakar, A., & Zaman, S. A. U. (2024, May 19). Novel Interpretable and Robust Web-based AI Platform for Phishing Email Detection. ArXiv.org. https://arxiv.org/abs/2405.11619*
 
	Kaggle link: https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset/data
