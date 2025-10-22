

## FitBuddy – AI-Powered Obesity Risk Prediction System

### Overview

FitBuddy is an **AI-driven health assistant** designed to predict a person’s **obesity risk** based on lifestyle, diet, and activity habits.
By using **Machine Learning algorithms**, FitBuddy analyzes user inputs such as age, height, fast-food consumption, and exercise frequency to classify individuals into categories like **Underweight**, **Normal**, **Overweight**, or **Obese**.

The system also includes a **speech-enabled chatbot**, allowing users to interact with the AI through voice input and receive personalized health advice through voice feedback.


### Purpose

Obesity is a growing global health challenge that increases the risk of chronic diseases such as diabetes, hypertension, and cardiovascular issues.
FitBuddy’s main goal is to:

* Provide **early obesity risk detection** using AI.
* Promote **health awareness and prevention**.
* Demonstrate how **AI can improve healthcare accessibility** through interactive tools.


### **Key Features**

Predicts obesity risk based on user’s lifestyle and physical data.
Provides personalized **health and lifestyle recommendations**.
Voice-enabled chatbot with **speech recognition (SpeechRecognition)** and **text-to-speech (pyttsx3)**.
Trained on real-world obesity dataset with over **1,600 records**.
Uses **Random Forest Classifier** for accurate obesity classification.
Displays ROC Curve and AUC evaluation metrics for model performance.


### Technologies Used

| Category             | Tools / Libraries                   |
| -------------------- | ----------------------------------- |
| Programming Language | Python                              |
| Machine Learning     | Scikit-learn, Joblib                |
| Data Handling        | Pandas, NumPy                       |
| Audio Interaction    | SpeechRecognition, Pyttsx3, PyAudio |
| Visualization        | Matplotlib                          |
| Dataset Format       | ARFF (Obesity_Dataset.arff)         |


### Installation & Setup

1. **Clone this repository**

   ```bash
   git clone https://github.com/OratilweBotlhale/PythonSoftbot.git
   cd PythonSoftbots
   ```

2. **Create a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   venv\Scripts\activate   # On Windows
   source venv/bin/activate  # On Mac/Linux
   ```

3. **Install required libraries**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the training script**

   ```bash
   python model.py
   ```

   This trains the model and saves:

   * `obesity_model.pkl`
   * `label_encoder.pkl`
   * `feature_order.json`

5. **Run the Softbot**

   ```bash
   python softbot.py
   ```

   Speak when prompted to answer FitBuddy’s questions.

---

## **Model Information**

* **Algorithm Used:** Random Forest Classifier
* **Accuracy:** 87.82%
* **Evaluation Metrics:** ROC Curve & AUC
* **AUC Score:** High (indicating excellent model performance)
* **Target Classes:** Underweight, Normal, Overweight, Obese


### Dataset Description

* **Dataset Name:** Obesity_Dataset.arff
* **Records:** 1,610 individuals
* **Attributes:**
  * Gender, Age, Height, Weight, Family History, Consumption of Fast Food, Vegetable Intake, Physical Activity, Technology Usage, etc.


### Chatbot Functionality

FitBuddy interacts with users through voice.
It:

1. **Asks questions** about age, diet, and exercise.
2. **Listens** to responses using SpeechRecognition.
3. **Processes** the answers through the trained AI model.
4. **Speaks** the obesity prediction and health advice back to the user.


### Evaluation Metrics

* **ROC Curve:** Shows the trade-off between True Positives and False Positives.
* **AUC (Area Under Curve):** Measures overall model quality (closer to 1.0 = better).
* The **Random Forest** model achieved the highest AUC among all tested algorithms.


### Future Improvements

* Integrate **time-series data** to track users’ progress over time.
* Develop a **mobile app version** for Android/iOS.
* Add **diet tracking and fitness goal recommendations**.
* Multi-language voice support for wider accessibility.
* Integration with **smartwatch and wearable sensors** for real-time data collection.


### Conclusion

FitBuddy demonstrates how **Artificial Intelligence can improve public health** through early detection and personalized advice.
By combining **machine learning** and **natural voice interaction**, this project bridges the gap between technology and healthcare — making health awareness both accessible and engaging.


Would you like me to generate the accompanying **`requirements.txt`** file for you too (so that everything installs smoothly on any computer)?
