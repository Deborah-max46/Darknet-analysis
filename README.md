# Name: Uwase Ketsia Deborah
# ID: 26244

---

## PROBLEM DEFINITION & PLANNING

### I. Sector Selection
Cybersecurity

### II. Problem Statement
How can we use flow-based network data to accurately detect and differentiate between Tor and Non-Tor traffic in darknet environments?

### III. Dataset Identification
- Dataset Title: Darknet
- Source Link: https://www.unb.ca/cic/datasets/darknet2020.html
- Number of Rows and Columns: 158616, 85
- Data Structure: csv file
- Data Status: needs preprocessing.


## PYTHON ANALYTICS TASKS
1. Clean the Dataset
   ![Data Cleaning](used%20screenshots/Data%20cleaning.png)
   The code loads the **Darknet dataset (158,616 rows × 85 columns)**, checks for **missing values** *(none found)*, removes an irrelevant **"Flow Bytes/s"** column, drops any **NaN rows**, encodes the **"Label"** column into numbers, and deletes identifier columns like **IP addresses** and **timestamps** to keep only useful features for **analysis or modeling**.
2. Conduct Exploratory Data Analysis (EDA)
   ![EDA](used%20screenshots/EDA.png)
   The code shows that after cleaning, the dataset has 79 usable columns and 158,616 records.
The numeric summary (df.describe()) gives ranges, averages, and variation for each feature, showing wide value differences between network traffic attributes.
The label distribution plot reveals how balanced Tor vs Non-Tor classes are.
   ![labels](used%20screenshots/labels.png)
3. Machine learning model
   ![evaluationn](used%20screenshots/evaluationn.png)
   The code trains a Random Forest Classifier on the darknet dataset to classify network traffic and evaluates its performance using a classification report, confusion matrix, and weighted metrics. The model achieved about 98.5% accuracy, with high precision, recall, and F1-scores across all classes, showing it reliably distinguishes normal and potentially malicious traffic. The confusion matrix indicates very few misclassifications, confirming the model is highly effective for darknet traffic detection.
   
   4. Power BI Dashboard.
      
      ![dashboard](used%20screenshots/dashboard.png)
      
      This is the screenshot of the dashboard, you may also find its file to download



