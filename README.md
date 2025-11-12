# 🚀 Certificate Eligibility Automation using n8n

This project automates the **certificate eligibility evaluation process** for students at **Innomatics Research Labs** using **n8n**.  
It reads student data from **Google Sheets**, evaluates performance based on predefined logic, and sends personalized emails indicating each student’s **certificate type** — 🥇 Gold, 🥈 Silver, 🥉 Bronze, or ❌ Not Eligible.

---

## 💡 Project Overview

The workflow eliminates manual effort in student performance evaluation by integrating **Google Sheets**, **n8n**, and **automated email notifications**.  
Once the student marks are updated in the sheet, the workflow automatically determines eligibility and sends a personalized email with the result.

---

## ⚙️ Tools & Technologies Used

- 🧩 **n8n** – Workflow Automation Platform  
- 📊 **Google Sheets** – Data Collection & Storage  
- ✉️ **Email Node** – Automated Communication  
- 🧠 **Conditional Logic Nodes** – Eligibility Evaluation  
- 💻 **Python Code Node** – Custom Logic (Average Calculation, Edge Cases)

---

## 🧠 Workflow Logic

| Criteria | Certificate Type | Condition |
|-----------|------------------|------------|
| 🥇 Gold | Eligible | Average ≥ 85 |
| 🥈 Silver | Eligible | 70 ≤ Average < 85 |
| 🥉 Bronze | Eligible | 50 ≤ Average < 70 |
| ❌ Not Eligible | Not Eligible | Average < 50 |

*(You can customize these thresholds as per institutional requirements.)*

---

## 🔄 Workflow Steps

1. **Fetch Data from Google Sheets**  
   - Retrieve student names, emails, and marks for all modules.

2. **Calculate Average Marks**  
   - Use n8n **Function Node** or **Python Code Node** for average calculation.

3. **Evaluate Eligibility**  
   - Use **IF** / **Switch** nodes to categorize based on average marks.

4. **Send Automated Email**  
   - Each student receives a personalized email with their certificate type and improvement suggestions.

5. **Real-Time Execution**  
   - Workflow triggers automatically whenever new data is added or updated.

---

## 📈 Key Features

✅ End-to-end **no-code automation**  
✅ Real-time **data synchronization** with Google Sheets  
✅ **Personalized** email notifications  
✅ Fully **customizable logic**  
✅ Reduces **manual evaluation time**  

---

## 🖼️ Workflow Preview (Example)

```text
Google Sheets → n8n Trigger → Function Node → Switch Node → Email Node
![n8n Workflow](./ebcebf0f-fe77-4191-96c1-0205793c4f33.png)


