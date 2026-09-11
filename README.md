# Customer Issue & Support Ticket Analyzer

## 📌 Project Overview

**Customer Issue & Support Ticket Analyzer** is a Python-based project designed to store, clean, and analyze customer support ticket data.

The project simulates a simple customer support ticket analysis system where ticket information such as customer name, issue description, and priority is collected and analyzed to identify common issues, support quality, ticket priorities, and frequently used words.

---

## 🎯 Objectives

Customer support teams handle numerous service tickets every day. These tickets contain valuable information about customer problems, service quality, and support experiences.

Manually reviewing these tickets can be time-consuming and makes it difficult to identify common issues and trends.

This project provides a simple Python-based solution to organize, clean, and analyze customer support tickets. It extracts useful insights from issue descriptions and ticket priorities, helping understand customer concerns and areas that may require improvement.

---

## ❓ Problem Statement

* Store customer support ticket information using Python data structures.  
* Add new tickets with automatically generated ticket numbers.  
* Validate ticket priorities as **High, Medium, or Low**.  
* Clean and standardize customer issue descriptions.  
* Perform keyword-based analysis of customer issues.  
* Analyze the distribution of ticket priorities.  
* Identify the ticket with the longest issue description.  
* Extract unique words used across all issue descriptions.  

---

## 🛠️ Technologies & Concepts Used

* **Python**  
* Lists  
* Dictionaries  
* Sets  
* Loops  
* Conditional Statements  
* Functions  
* String Manipulation  
* User Input  
* Data Cleaning  

---

## 🔄 Project Workflow

### Step 1: Preloaded Tickets

The project starts with **10 preloaded customer support tickets** containing:

* Ticket Number  
* Customer Name  
* Issue Description  
* Priority  

The initial ticket data is displayed in a readable format.

### Step 2: Add New Tickets

Users can enter the number of new tickets they want to add.

For each new ticket, the system collects:

* Customer Name  
* Issue Description  
* Priority  

Ticket numbers are automatically generated starting from **11**.

Priority validation ensures that only:

* High  
* Medium  
* Low  

are accepted.

In this project, **2 additional tickets** were added, bringing the total number of tickets to **12**.

### Step 3: Text Cleaning

The issue descriptions are cleaned and standardized by:

* Removing punctuation such as `. , ! ? -`  
* Removing extra spaces  
* Removing leading and trailing spaces  
* Converting text to lowercase  
* Replacing shorthand such as `ok` with `okay`  

For example:

```text
"Ok."
```

is converted to:

```text
"okay"
```

Another example:

```text
"Good service...quick response."
```

is converted to:

```text
"good service quick response"
```

### Step 4: Keyword-Based Analysis

A function named:

```python
count_tickets_with_word(word)
```

is used to identify how many tickets contain a specific keyword.

The project analyzes the following keywords:

* `poor`  
* `good`  
* `slow`  
* `excellent`  

The search is **case-insensitive** and counts tickets containing the exact word.

### Step 5: Final Analysis

The project performs the following analysis:

* Displays the final cleaned ticket data.  
* Counts High, Medium, and Low priority tickets.  
* Identifies the ticket(s) with the longest issue description.  
* Extracts unique words from all issue descriptions.  
* Displays the sorted list of unique words.  

---

## 📊 Key Insights

Based on the final output containing **12 tickets**:

### Priority Analysis

| Priority | Number of Tickets |
| -------- | ----------------: |
| High     |                 5 |
| Medium   |                 4 |
| Low      |                 3 |

**Insight:** High-priority tickets are the largest category, indicating that several customer issues require immediate attention.

### Keyword Analysis

| Keyword   | Tickets Containing the Word |
| --------- | --------------------------: |
| Poor      |                           2 |
| Good      |                           3 |
| Slow      |                           2 |
| Excellent |                           1 |

**Insights:**

* **"Good"** is the most frequently occurring keyword among the selected keywords.  
* **"Poor"** appears in 2 tickets, indicating some negative customer experiences.  
* **"Slow"** appears in 2 tickets, suggesting response time may be an area for improvement.  
* **"Excellent"** appears in 1 ticket, indicating positive feedback about the support experience.  

### Longest Issue Descriptions

Three tickets have the highest issue-description word count:

| Ticket No. | Customer | Word Count |
| ---------: | -------- | ---------: |
|          2 | Meera    |          5 |
|          7 | Arjun    |          5 |
|          8 | Kiran    |          5 |

The cleaned descriptions are:

```text
Ticket 2: slow response very poor service  
Ticket 7: good support and good behaviour  
Ticket 8: poor handling of technical issue  
```

### Unique Words

The project identified:

**33 unique words**

across all cleaned issue descriptions.

This helps understand the variety of terms customers use when describing their support experiences.

---

## 📈 Overall Findings

* The majority of tickets are categorized as **High or Medium priority**.  
* Positive feedback is present through words such as **good, excellent, great, satisfied, and helpful**.  
* Negative feedback mainly relates to **poor service, slow response, and technical issues**.  
* Response speed and technical issue handling appear to be important areas for improving customer satisfaction.  
* Text cleaning makes the issue descriptions more consistent and suitable for analysis.  
* Keyword and unique-word analysis provide a simple way to identify patterns in customer feedback.  

---

## 💡 Recommendations

Based on the analysis, customer support teams could:

* Improve response time for customers reporting slow service.  
* Give priority to high-priority technical issues.  
* Monitor recurring complaints related to poor service.  
* Continue maintaining good support practices that result in positive customer feedback.  
* Use automated ticket analysis to identify common issues more efficiently.  

---

## 🧠 Python Concepts Demonstrated

This project demonstrates practical use of:

```text
Lists
Dictionaries
Sets
For Loops
While Loops
If-Else Statements
Functions
String Methods
User Input
Data Validation
Data Cleaning
Keyword Searching
```

---

## 📂 Project Structure

```text
Customer-Issue-Support-Ticket-Analyzer/
│
├── Customer_Support_Ticket_Analyzer.ipynb
└── README.md
```

---

## ✅ Conclusion

The **Customer Issue & Support Ticket Analyzer** demonstrates how Python can be applied to a real-world customer support data analysis problem.

The project successfully manages customer tickets, validates new ticket information, cleans issue descriptions, analyzes keywords and priorities, identifies the longest issue descriptions, and extracts unique words.

Overall, this project provides practical experience in using fundamental Python concepts for **data cleaning, text analysis, and extracting meaningful insights from customer support data**.

