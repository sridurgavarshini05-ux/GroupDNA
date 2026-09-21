# GroupDNA
WhatsApp Group Chat Analysis using Python and NumPy

# 🧬 GroupDNA – Your WhatsApp Group, Decoded

## 📌 Project Description

GroupDNA is a Python-based data analysis project that analyzes a
WhatsApp group chat and converts the raw chat data into meaningful
activity and communication insights.

The project is inspired by the idea of "Spotify Wrapped, but for
your friend group."

It analyzes messages, participants, activity patterns, frequently
used words, response time, silent streaks, and personality archetypes.

---

## 🎯 Objective

The main objective of this project is to understand how a WhatsApp
group communicates by analyzing its exported chat data using Python
fundamentals and NumPy.

---

## 📂 Dataset

Dataset used:

`hostel_bois.txt`

The dataset is a synthetic WhatsApp Android chat export containing:

- 60 days of chat data
- 6 participants
- 3,174 real messages
- Date range: 01/04/2024 to 30/05/2024

The chat follows the format:

DD/MM/YY, HH:MM - Sender Name: Message

---

## 🛠️ Technologies and Libraries Used

### Programming Language
- Python

### Libraries
- NumPy
- datetime

### Python Concepts Used
- Strings
- Lists
- Tuples
- Dictionaries
- Sets
- Loops
- Conditional statements
- Functions
- List comprehensions
- File handling
- String processing
- Sorting

---

## 🔍 Project Features

### 1. Chat Parser

The raw WhatsApp chat is read line by line and converted into
structured data containing:

- Timestamp
- Sender
- Message

Special cases such as system messages and other non-standard
messages are considered during parsing.

---

### 2. Group Overview

This section answers questions such as:

- How many total messages are there?
- How many participants are in the group?
- What is the date range?
- How many active days are there?
- Who sent the most messages?
- How many messages did each participant send?

---

### 3. Most Active Day and Hour

This feature identifies:

- The day with the highest number of messages
- The hour with the highest number of messages

It helps identify when the group is most active.

---

### 4. Activity Heatmap

A NumPy-based activity matrix is created.

- Rows represent participants
- Columns represent hours from 00 to 23
- Each cell represents the number of messages sent by a participant
  during that hour

This helps visualize the activity pattern of each participant.

---

### 5. Top 10 Frequently Used Words

The messages are processed by:

- Converting text to lowercase
- Removing punctuation
- Removing common stop words
- Counting word frequency
- Finding the top 10 most frequently used words

---

### 6. Response Speed and Silent Streaks

This feature analyzes communication behavior by calculating:

- Average response time
- Response gaps between different participants
- Longest period of inactivity for each participant
- Silent streaks in days

---

### 7. Personality Archetype Detection

Each participant is assigned one personality archetype based on
quantitative characteristics of their messages.

The archetypes include:

- Spammer
- Group Mom
- Night Owl
- Storyteller
- Drama Queen
- Ghost
- Comedian
- Question Master

The classification is based on measurable chat behavior such as
message bursts, caring keywords, night-time activity, message
length, capital letters, silence, humour-related words, and
question frequency.

---

## 📊 Example Archetypes

| Participant | Archetype |
|------------|-----------|
| Rahul | Spammer |
| Priya | Group Mom |
| Aman | Night Owl |
| Karan | Storyteller |
| Neha | Drama Queen |
| Vikas | Ghost |

---

## 📋 Main Questions Answered by the Project

The project attempts to answer questions such as:

1. Who is the most active member of the group?
2. What day has the highest activity?
3. What hour is the group most active?
4. What are the most frequently used words?
5. How quickly do members respond to each other?
6. Who has the longest silent streak?
7. What are the activity patterns of each participant?
8. Which personality archetype best describes each participant?
9. When is each participant most active?
10. What communication patterns can be observed from the group?

---

## 📈 Final Output

The project generates a formatted GroupDNA report containing:

- Group overview
- Messages by participant
- Most active day
- Most active hour
- Top 10 words
- Average response time
- Longest silent streaks
- Personality archetypes

---

## 📸 Project Output

Add a screenshot of your final GroupDNA report here.

Example:

![GroupDNA Final Report](final_report.png)

Add your activity heatmap screenshot here if available.

![Activity Heatmap](activity_heatmap.png)

---

## ▶️ How to Run the Project

### Using Google Colab

1. Open the notebook in Google Colab.
2. Upload `hostel_bois.txt`.
3. Run the notebook cells from top to bottom.
4. The final GroupDNA report will be generated at the end.

The dataset should be available at:

`/content/hostel_bois.txt`

---

## 📁 Project Files

```text
GroupDNA/
│
├── GroupDNA_SRIDURGA.ipynb
├── hostel_bois.txt
└── README.md
