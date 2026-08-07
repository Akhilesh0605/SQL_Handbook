# 📘 SQL Handbook for Interviews
### By: Senior SQL Engineer & Database Architect
### Chapter 1 — What is Data?

---

## 1. What is Data?

---

### 📌 Definition

**Data** is any raw, unprocessed fact, figure, symbol, or value that on its own may or may not carry meaning.

- Data can be **numbers**, **text**, **images**, **audio**, **video**, **dates**, or **boolean values**.
- Data becomes **information** when it is **processed, organized, and given context**.

> Example: `23` is data. `"Employee age is 23"` is information.

---

### ❓ Why Do We Use It?

| Reason | Explanation |
|---|---|
| **Decision Making** | Businesses use data to make strategic decisions |
| **Automation** | Systems use data to trigger automated actions |
| **Machine Learning** | ML models train on large amounts of structured data |
| **Analytics** | Data helps find patterns, trends, and insights |
| **Storage & Retrieval** | Applications store and fetch data constantly |

---

### ⏰ When Should We Think About Data?

- When building any application that needs to **store state**
- When performing **analytics or reporting**
- When training **ML/AI models**
- When designing **APIs that serve or receive information**
- Whenever a business process needs to be **tracked or audited**

---

### 🗂️ Types of Data

#### 1. Based on Structure

| Type | Description | Example |
|---|---|---|
| **Structured** | Organized in rows & columns | SQL Tables, Excel |
| **Semi-Structured** | Partially organized | JSON, XML, CSV |
| **Unstructured** | No fixed format | Images, Videos, PDFs, Emails |

---

#### 2. Based on Nature

| Type | Description | Example |
|---|---|---|
| **Quantitative** | Numeric, measurable | Salary, Age, Price |
| **Qualitative** | Descriptive, categorical | Name, Gender, City |

---

#### 3. Based on Time

| Type | Description | Example |
|---|---|---|
| **Static** | Rarely changes | Date of Birth, Country Code |
| **Dynamic** | Frequently changes | Stock Price, Order Status |

---

#### 4. Based on Source

| Type | Description | Example |
|---|---|---|
| **Primary** | Collected directly | Survey responses |
| **Secondary** | Collected from existing sources | Public datasets |
| **Real-time** | Streamed continuously | Sensor data, Clicks |
| **Historical** | Stored over time | Transaction logs |

---

### 💡 Example

Imagine an **E-commerce application** like Amazon:

| Data Point | Type |
|---|---|
| Customer Name | Qualitative, Structured |
| Order Amount | Quantitative, Structured |
| Product Image | Unstructured |
| Delivery Status | Dynamic, Structured |
| Customer Review | Semi-structured / Unstructured |
| Date of Purchase | Static (per transaction), Structured |

---

### 🌍 Real-World Example

**Banking System**

| Column | Data | Type |
|---|---|---|
| `account_id` | 10023 | Quantitative |
| `account_holder` | "Jane Doe" | Qualitative |
| `balance` | 52000.75 | Quantitative |
| `account_type` | "Savings" | Qualitative |
| `is_active` | TRUE | Boolean |
| `created_at` | 2021-06-15 | Date |

All these individual values are **data**.  
Together in context, they become **information** about a customer's bank account.

---

### 🎯 Data in SQL Context

In SQL (Structured Query Language), we primarily deal with **structured data** stored in **tables** inside a **relational database**.

```sql
-- Example: A simple employees table storing structured data
SELECT employee_id, name, salary, department
FROM employees;
```

Every row = one **record** (a set of related data points)  
Every column = one **attribute** (a specific type of data)

---

### 📐 Data vs Information vs Knowledge

| Term | Definition | Example |
|---|---|---|
| **Data** | Raw facts | `45000` |
| **Information** | Processed data with context | `Salary is ₹45,000` |
| **Knowledge** | Understanding derived from information | `This salary is above average for this role` |

---

### ⚠️ Common Interview Questions

1. **What is data? How is it different from information?**
2. **What are the different types of data?**
3. **What is structured vs unstructured data? Give examples.**
4. **What type of data does SQL handle?**
5. **What is the difference between quantitative and qualitative data?**
6. **Can SQL store unstructured data? How?**
7. **What is semi-structured data? Where is it used?**
8. **Why is data important for machine learning?**
9. **What is real-time data? How is it different from batch data?**
10. **What is a data point vs a dataset?**

---

### ❌ Common Mistakes

- Confusing **data** with **information** — they are NOT the same.
- Assuming SQL only stores **text and numbers** — it can also store JSON, XML, BLOBs (Binary Large Objects), etc.
- Forgetting that **NULL** is also a valid data value in SQL, representing missing/unknown data.
- Treating all data as **static** — in real systems, most data is **dynamic**.
- Ignoring **data quality** — bad data leads to wrong decisions (Garbage In, Garbage Out).

---

### ✅ Best Practices

- Always **validate data** before storing it (use constraints).
- Use the **right data type** for each column to save space and improve performance.
- Handle **NULL values** explicitly — never assume a field will always have a value.
- Keep **raw data** separate from **processed/aggregated data** in data pipelines.
- Document what each data field means (**data dictionary / data catalog**).

---

### ⚡ Performance Tips

- **Structured data** in relational databases (SQL) is faster to query than unstructured data.
- Choosing the **correct data type** (e.g., `INT` vs `VARCHAR`) directly impacts **storage size and query speed**.
- **Indexing** columns that are frequently searched improves retrieval performance.

---

### 📝 Important Notes

- In **SQL interviews**, when asked about data, always relate it back to **tables, rows, columns, and schema**.
- For **AI/ML interviews**, emphasize **structured vs unstructured**, **missing data handling**, and **feature data**.
- For **Data Engineering interviews**, emphasize **batch vs streaming**, **ETL pipelines**, and **data quality**.

---

### 📋 Summary

| Point | Key Takeaway |
|---|---|
| Data Definition | Raw, unprocessed facts |
| Types | Structured, Semi-structured, Unstructured |
| SQL Focus | Primarily **Structured Data** |
| Data vs Information | Data + Context = Information |
| NULL | Valid data value meaning "unknown" |
| Importance | Foundation of every application, ML model, and business decision |

---

### 🏋️ Practice Questions

1. Define data in your own words with an example.
2. List 5 examples of structured data from an e-commerce app.
3. How does SQL handle semi-structured data like JSON?
4. What is the difference between static and dynamic data? Give real-world examples.
5. A hospital stores patient names, X-ray images, and doctor notes. Classify each.
6. Why is data quality important? What happens with bad data?
7. What does NULL represent in SQL?
8. How is data used in a machine learning pipeline?
9. Give 3 examples of real-time data from a ride-sharing app like Uber.
10. What is a data dictionary? Why do teams use it?

---

> ✅ **Chapter 1 Complete.**
> ➡️ **Next: Chapter 2 — What is a Database?**
