# PRODIGY_DS_02

## Task 2: Data Cleaning and Exploratory Data Analysis

In this task, I performed **data cleaning** and **exploratory data analysis (EDA)** on the Titanic dataset provided by **Prodigy Infotech**.

### 📌 Steps I Followed
1. **Data Loading**  
   - Imported the dataset (`train.csv`) into Google Colab using Pandas.

2. **Data Inspection**  
   - Checked dataset shape, data types, missing values, and basic statistics using `.info()`, `.describe()`, and `.isnull().sum()`.

3. **Data Cleaning**  
   - Filled missing values in `Age` with median.  
   - Filled missing values in `Embarked` with mode.  
   - Dropped the `Cabin` column due to high percentage of missing values.  
   - Removed duplicate rows.

4. **Exploratory Data Analysis (EDA)**  
   - Visualized **Survival distribution**.  
   - Analyzed survival rates by **gender** and **passenger class**.  
   - Plotted **Age** and **Fare** distributions.  
   - Created a **correlation heatmap** for numeric features.

### 📊 Key Findings
- **Females** had a much higher survival rate than males.  
- **1st class** passengers had the highest survival rates.  
- Younger passengers (children) had better chances of survival compared to seniors.  
- Fare also showed a positive correlation with survival.

### 🛠 Tools Used
- Python  
- Pandas  
- Matplotlib  
- Seaborn  

### 📸 Example Visualizations
*(Add screenshots of your main plots here)*

---

**GitHub Repository:** [Add your Task 2 folder link here]

