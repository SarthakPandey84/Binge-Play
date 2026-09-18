<div align="center">
  <h1>🍿 BingePlay Streaming Analytics</h1>
  <p><i>Uncovering actionable business insights from streaming data through complex SQL analysis.</i></p>

  [![SQL](https://img.shields.io/badge/SQL-Core_Analysis-003B57?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
  [![Python](https://img.shields.io/badge/Python-Data_Extraction-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
  [![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Presentation-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
</div>

<br />

## 📖 Overview

**BingePlay** is a comprehensive data analytics project focused on a fictional streaming platform. This repository contains data analysis, metrics extraction, and business intelligence queries designed to answer 12 critical business questions about user engagement, revenue generation, content performance, and customer churn.

**Dataset:** You can download the SQL dataset used for this analysis [here](https://drive.google.com/file/d/1xifptnaD3xbYdNc0i7otqDsl03SL5nPs/view?usp=sharing).

By leveraging advanced SQL techniques—including Common Table Expressions (CTEs), Window Functions, and complex JOINs—this project transforms raw database records into strategic business insights.

---

## 🛠️ Technologies & Tools

- **SQL / MySQL:** Core analytical logic, advanced aggregations, and data transformation.
- **Python (Pandas, SQLAlchemy):** Data extraction, script execution, and seamless notebook integration.
- **Jupyter Notebook (Google Colab):** Interactive presentation of code, queries, and business findings.

---

## 📊 Key Analytics & Business Questions

The main notebook (`bingeplay_Sarthak.ipynb`) executes complex SQL queries to uncover actionable business insights across several domains:

### 💰 Revenue & Growth
1. **Active Revenue:** Calculation of Monthly Recurring Revenue (MRR) for active subscriptions.
2. **Signup Momentum:** Monthly cohort tracking of new users to measure platform growth.
3. **Upgrade Success:** Tracking the cohort of Basic users who upgraded to Premium/Family and calculating average conversion time.

### 📱 User Engagement & Behavior
4. **Device Analytics:** Session counts and completion rates across Mobile and TV.
5. **Binge Day Detection:** Identification of highly engaged users consuming 5+ sessions of the same show in a single day.
6. **Consecutive-Week Streaks:** Complex gaps-and-islands logic to identify users with 4+ uninterrupted calendar weeks of viewing.
7. **Cliffhanger Comebacks:** Re-engagement analysis tracking users who leave a show incomplete but return within 7 days.

### 🎬 Content Performance
8. **Rating Distribution:** Sentiment analysis based on user star ratings.
9. **Originals vs. Acquired:** Quality comparison between in-house and acquired shows.

### ⚠️ Risk & Churn Mitigation
10. **Activation Failures:** Identifying Q1 signups who have never watched a single show.
11. **Overpaying Users:** Highlighting Premium/Family users who exclusively watch Basic-tier content (or nothing at all), making them prime targets for downgrade offers rather than churn.
12. **Churn Signals:** Flagging users whose watch time dropped by over 50% month-over-month.

---

## 📂 Repository Structure

```text
📦 BingePlay
 ┣ 📜 README.md               # Project documentation (You are here!)
 ┣ 📓 bingeplay_Sarthak.ipynb # Primary executable notebook with SQL queries & insights
 ┗ 📝 .gitignore              # Ignored files and directories
```

*(Note: Additional python testing scripts might be present in the original dataset for validating SQL queries against the local database schema.)*

---

## 🚀 Getting Started

Follow these steps to run the analytics notebook locally:

### 1. Prerequisites
- **MySQL Server:** Ensure you have a local instance running.
- **Python 3.x:** With `pandas`, `sqlalchemy`, and `jupyter` installed.
- **Database Schema (Dataset):** Download the [SQL Setup File](https://drive.google.com/file/d/1xifptnaD3xbYdNc0i7otqDsl03SL5nPs/view?usp=sharing) and load it into your local MySQL server to create the `bingeplay` database.

### 2. Installation
Clone the repository to your local machine:
```bash
git clone https://github.com/yourusername/BingePlay.git
cd BingePlay
```

### 3. Execution
Launch Jupyter Notebook:
```bash
jupyter notebook
```
Open `bingeplay_Sarthak.ipynb`. The notebook will securely prompt you for your MySQL root password to establish the SQLAlchemy connection. Once connected, run the cells sequentially to view the analysis and insights.

---

## 💡 Key Takeaways

Through this analysis, the BingePlay project demonstrates the power of SQL in extracting real-world business value. From identifying at-risk users before they churn, to pinpointing highly engaged "binge" viewers, the queries provide a foundation for data-driven decision making in a subscription-based digital media environment.

<br />

<div align="center">
  <i>If you find this project interesting, feel free to ⭐ the repository!</i>
</div>
