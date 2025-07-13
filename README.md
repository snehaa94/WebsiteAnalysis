# 🌐 Website Performance Analysis

This project explores and visualizes user behavior and engagement across various website traffic channels using Python. It helps in understanding which traffic sources drive the most users, how users engage with the site, and what patterns exist across different hours and channels.

---

## 📁 Project Structure

```
websiteAnalysis/
├── website_performance_Analysis.ipynb
├── data-export.csv
├── .ipynb_checkpoints/
└── README.md
```

---

## 📊 Features of the Analysis

- Data cleaning and preprocessing using **Pandas**
- Time parsing and extraction of hourly patterns
- Conversion of metrics to numeric values
- Analysis of:
  - Total Users by Channel Group
  - Average Engagement Time
  - Engagement Rate Distribution
- Visualizations with **Seaborn** and **Matplotlib**

---

## 🛠️ Libraries Used

- pandas
- numpy
- matplotlib
- seaborn

---

## 🔍 Key Insights

- **User Volume**: Compared total users from each channel group.
- **Engagement Time**: Analyzed which sources retained users for longer.
- **Engagement Rate**: Used box plots to detect variations across sources.

---

## 📈 Sample Visualizations

### 👥 Total Users by Channel Group

```python
sns.barplot(data=df, x="channel group", y="Users", estimator=np.sum, palette="viridis")
```

### ⏱️ Average Engagement Time

```python
sns.barplot(data=df, x="channel group", y="Avg Engagement Time", estimator=np.mean, palette="magma")
```

### 📦 Engagement Rate Distribution

```python
sns.boxplot(data=df, x="channel group", y="Engagement rate", palette="coolwarm")
```

---

## 📂 Dataset Columns

- `channel group`
- `DateHour`
- `Users`
- `Sessions`
- `Engaged Sessions`
- `Average engagement time per session`
- `Engaged sessions per user`
- `Events per session`
- `Engagement rate`
- `Event count`

---

## 🧪 How to Run the Project

1. Clone the repo:
   ```bash
   git clone https://github.com/snehaa94/WebsiteAnalysis.git
   cd WebsiteAnalysis
   ```

2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Open `website_performance_Analysis.ipynb` and run the cells.

---

## 📊 Sample Visualizations

### 👥 Sessions and Users Over Time

<img width="1299" height="912" alt="Screenshot (57)" src="https://github.com/user-attachments/assets/4a26d372-d78f-43aa-8aa9-ae6b748f2235" />

### ⏱️ Total Users by Channels

<img width="1271" height="902" alt="Screenshot (58)" src="https://github.com/user-attachments/assets/83872897-5956-4704-b4a0-666dc1d2b8b5" />

### 📦 Average Engagement Time by Channel

<img width="1288" height="930" alt="Screenshot (59)" src="https://github.com/user-attachments/assets/bd4657d6-836a-436f-815d-6d25de0b49cb" />

### 📈 Engagement Rate Distribution by Channel

<img width="1281" height="909" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/72b7a737-015b-4210-8eeb-b5667dfee580" />

---

## 📃 License

This project is for educational and analytical purposes only. Feel free to use and modify.
