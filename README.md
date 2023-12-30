**Project Title**

Application of deep learning for the cybersecurity of In-Vehicle Networks of autonomous vehicles

**Project Overview**

This project focuses on applying deep learning techniques to analyze Controller Area Network (CAN) network traffic in automotive vehicles. The dataset contains both attack and normal messages, with features including class and subclass designations to differentiate between legitimate operational signals and potential attack messages. The primary objective is to develop robust models capable of distinguishing between normal and malicious CAN messages.

**Dataset Source**

https://www.mdpi.com/1424-8220/22/1/360

**Feature Engineering**

Feature engineering techniques were applied to enhance the dataset. The focus was on splitting the data column into its relevant format. This step aimed to improve the overall quality and informativeness of the dataset.

**Data Preprocessing**

After feature engineering, data preprocessing steps were implemented to prepare the dataset for model training. This involved handling missing values, normalizing numerical features, and encoding categorical variables. The objective was to create a clean and standardized input for the neural network models.

**Neural Network Architectures**

**Artificial Neural Network (ANN)**

An artificial neural network was also included in the study. This architecture was chosen for its versatility in handling structured data. The ANN model's performance was evaluated, and results were compared with those of the CNN and LSTM models.

**Long Short-Term Memory (LSTM)**

A long short-term memory network was employed as another neural network architecture. LSTMs are well-suited for capturing temporal dependencies, making them suitable for sequential data like CAN messages. The LSTM model's performance was assessed to determine its effectiveness in the context of automotive cybersecurity.

**Convolutional Neural Network (CNN)**

A convolutional neural network was implemented as one of the neural network architectures. Although typically used for image data, in this context, the CNN was tailored to capture patterns and relationships within the structured data of CAN messages. The results obtained from the CNN were analyzed to evaluate its performance on the given dataset.

**Multi-Task and Multi-Stage Approaches**

**Multi-Task Approach**

All three models were applied using a multi-task approach. This involved predicting both class and subclass simultaneously. The models were trained to recognize and differentiate between different types of CAN messages.

**Multi-Stage Approach**

In the multi-stage approach, the models were trained in two stages. In the first stage, the model was trained using the class feature. In the second stage, all normal instances were dropped, and the model was retrained specifically for the subclass feature. This approach aimed to enhance the model's ability to distinguish between subclasses after an initial classification based on the class feature.

**Model Evaluation**

The convolutional neural network using multi-stage approach demonstrated the best results among the three architectures. Evaluation metrics such as accuracy, precision, recall, and F1 score were used to assess the models' performance. The findings provide insights into the efficacy of deep learning for automotive cybersecurity in the context of CAN traffic analysis.

**Result Visualization**

Results, including predictions and performance metrics, were visualized to facilitate interpretation. Visualizations may include confusion matrices, ROC curves, and other relevant plots to showcase the models' effectiveness in distinguishing between normal and malicious CAN messages.
