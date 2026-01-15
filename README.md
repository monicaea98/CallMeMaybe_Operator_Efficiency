# 📞 CallMeMaybe Operator Efficiency Analysis

This project analyzes operator performance for the **CallMeMaybe virtual telephone service** with the goal of identifying the **least effective operators** based on objective, data-driven metrics. By detecting patterns of inefficiency, the analysis helps supervisors improve service quality, reduce missed calls, and optimize operational performance.

The project includes both an **analytical notebook** and a **final presentation** summarizing results and recommendations.

---

## 🎯 Project Objectives

### Overall Objective

Identify the least effective operators using key telephone service metrics in order to support **data-driven decision-making** by supervisors.

### Specific Objectives

* Analyze incoming and outgoing call behavior
* Evaluate waiting time, call duration, and missed calls per operator
* Define quantitative criteria for operator inefficiency
* Classify operators as **efficient** or **inefficient**
* Validate findings using statistical hypothesis testing

---

## 🗂️ Data Sources

The analysis was conducted using datasets containing information on:

* Call duration
* Number of incoming and outgoing calls
* Percentage of missed calls
* Average waiting time
* Internal and external calls
* User and operator identifiers

---

## 📊 Exploratory Analysis Highlights

### Call Duration Distribution

* Most calls are **very short**, with a right-skewed distribution
* A small number of extremely long calls increases variability
* This pattern is typical in customer service environments

### Call Duration Without Outliers

* Removing extreme values reveals typical behavior more clearly
* Most calls last between **0 and 100 seconds**
* This improves the stability of statistical analysis and threshold definition

### Outgoing Calls by Operator

* Most operators make between **0 and 20 outgoing calls**
* Several operators show **very low or no outgoing activity**
* This helps identify low-engagement operators

---

## 🚨 Inefficiency Definition

An operator is classified as **inefficient** if they meet **two or more** of the following conditions:

* Fewer than **5 outgoing calls**
* **Missed call rate greater than 12.13%**
* **Average waiting time greater than 155.54 seconds**

These thresholds were selected based on data distributions and represent values significantly worse than the overall average.

---

## 📈 Efficient vs. Inefficient Operators

Operators were segmented into two groups based on the defined criteria:

* **Efficient operators** — meet performance expectations
* **Inefficient operators** — require attention and intervention

This classification enables supervisors to **prioritize actions** and allocate resources more effectively.

---

## 🧪 Hypothesis Testing

A **t-test** was conducted to compare the average waiting time between efficient and inefficient operators.

* **H₀:** There is no significant difference in average waiting time
* **H₁:** Inefficient operators have a longer average waiting time

### Result

The test provided sufficient evidence to **reject H₀** (p-value < 0.05), confirming that inefficient operators have **significantly longer waiting times**.

---

## 🧠 Key Findings

* Inefficient operators consistently show **longer waiting times**
* Missed calls are more frequent among inefficient operators
* Many operators exhibit **low outgoing call activity**
* The selected metrics allow for **reliable and objective classification**
* Statistical testing validates waiting time as a strong inefficiency indicator

---

## 📊 Project Presentation (Results Summary)

The final presentation includes:

* Overview of objectives and data sources
* Key exploratory visualizations
* Definition of inefficiency criteria
* Comparison of efficient vs. inefficient operators
* Hypothesis testing results
* Conclusions and actionable recommendations

---

## 📌 Recommendations

* Provide **targeted training** for inefficient operators
* Implement **continuous monitoring** of key performance metrics
* Use **early warning indicators** based on inefficiency factors
* Review operator rankings and performance **monthly**
* Introduce real-time dashboards to detect performance drops early

---

## 🛠️ Tools & Technologies

* 🐍 **Python**
* 📊 **Pandas & NumPy** — data processing and aggregation
* 📈 **Matplotlib & Seaborn** — exploratory analysis and visualizations
* 🧮 **Statistical Testing (t-test)** — hypothesis validation
* 📘 **Jupyter Notebook** — interactive analysis

---

## 📝 Conclusion

This project demonstrates how operational data and statistical analysis can be used to **objectively measure operator performance**. By identifying inefficiency patterns and validating them statistically, CallMeMaybe gains a practical framework to improve service quality, optimize resources, and enhance customer experience.
