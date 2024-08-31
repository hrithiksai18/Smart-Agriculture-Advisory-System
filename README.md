# Smart-Agriculture-Advisory-System
Practical Approach to Smart Agriculture Advisory System

#### Introduction
The Smart Agriculture Advisory System is supposed to be the digital assistant of a farmer advising on issues of crop management, pesticide usage, and irrigation regarding time and method of irrigation. In additions, using machine learning, the system surveys the prevailing environmental and soil conditions to recommend the most appropriate crops for a particular condition.

#### Dataset
In this project, the **Crop Recommendation Dataset** available on Kaggle is being used. This dataset is required to be fed to the model to train it for recommendations.

**Some Important Features in the Dataset:**

* **Nitrogen (N):** The amount of nitrogen in the soil.
* **Phosphorus (P):** The amount of phosphorus available.
* **Potassium (K):** The amount of potassium in the soil.
* **Temperature:** In degree Celsius.
* **Humidity:** In percentage.
* **pH:** Level of acidity or alkalinity.
- **Rainfall:** Amount of rainfall in millimeters.

**Target for Prediction:**
- **Crop Label:** The crop to be grown in such conditions.

#### Installation Guide
In order to get started, you need to set up the environment.

**Pre-Requisites:**
- **Anaconda:** A free and open source software package including Python and R for scientific computing.

**Steps to Install:**

1. **Install Anaconda:**
	- Go to Anaconda's website and click on the download option that matches your operating system.

2. **Clone the Repository:
```bash
git clone https://github.com/your-username/smart-agriculture-advisory-system.git
   cd smart-agriculture-advisory-system
   ```
3. **Create a Conda Environment:**
   ```
   conda create --name smart-agriculture python=3.8
   conda activate smart-agriculture
   ```
4. **Install Required Libraries:**
   ```
   pip install -r requirements.txt
   ```
5. **Install Jupyter Notebook:**
   ```bash
   conda install -c conda-forge notebook
Yu may start Jupyter Notebook by executing
```bash
jupyter notebook
```

2. **Play with the Notebook:**
	* Open `notebooks/Smart_Agriculture_Advisory_System.ipynb` to play with data preprocessing, model training and predictions of crops.

#### Project Structure

- **data/:** The folder contains the dataset for training and testing.
- **notebooks/:** Jupyter Notebooks to walk you through the process of data analysis and model development.
- **models/:** The folder saves machine learning models after training.
- **scripts/:** Python scripts to process data, fit the model and save it.
- **requirements.txt**: Concerning the used Python libraries.

#### Model Understandings

**Selection of the Best Model:
We tried many models of machine learning, but we went with **Random Forest**. This model was chosen with respect to its performance in terms of accuracy and reliability over the rest.

**Training of the Model:**

1. **Data Preprocessing:**

	* Clean the missing data.
	* Scale the features properly.
	* Encode categorical variables.

2. **Feature Selection:**

* Identify which features bear the most influence on the forecast of crops.

3. **Training Process:
Also, **GridSearchCV** did a pretty good job tuning the Random Forest model, which for its part did quite a good job in optimizing its performance.

#### Model Evaluation
The metrics we used to assess this model are as follows:

- **Accuracy:** It was quite impressive, 99%, which in itself says almost everything about how reliable the model is.
- **Precision, Recall, and F1-Score:** Complementary measures to further validate the reliability of the model in its correct predictions.
Cross-Validation: We wanted to make sure that the model was generalizable and not fitted to the training data, so we performed several cross-validation techniques.

#### Contributing to the Project
We welcome all kinds of contributions! If you have improvements or bug fixes please don't hesitate to:

* Fork the repository.
* Create your changes.
Pull request is open for review.

---
It's chattier in style, hence easier to understand; thus it summarizes some of the same information but it does so in a way that anyone could understand and, therefore, follow along in the project.
