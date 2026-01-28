🧠 IT Ticket Prioritizer using Transformer Models
📌 Project Overview

This project implements an IT Ticket Prioritization System that automatically classifies support tickets as Angry/Urgent or Neutral. The goal is to help IT teams quickly identify critical issues and respond faster without manual intervention.

🎯 Objective

To analyze IT support tickets

To detect anger or urgency in user messages

To assign appropriate ticket priority automatically

🛠️ Technologies Used

Python

Google Colab

Hugging Face Transformers

RoBERTa (Sentiment Analysis Model)

🧠 Approach

A pre-trained RoBERTa transformer model is used to detect the sentiment of each ticket.

The model outputs sentiment labels (LABEL_0, LABEL_1, LABEL_2).

Urgency is identified using keyword-based checks (e.g., down, urgent, unacceptable).

If a ticket shows negative sentiment OR urgency, it is marked as P1 – Immediate Attention.

Otherwise, it is marked as P3 – Normal Priority.

No custom model training is required (zero-shot approach).

🚦 Priority Rules
Condition	Priority
Angry or Urgent	P1 – Immediate Attention
Normal Request	P3 – Normal Priority
🧪 Sample Input
My server is down and this is unacceptable!

✅ Sample Output
Category: Angry/Urgent
Priority: P1 – Immediate Attention

📂 Project Structure
IT-Ticket-Prioritizer/
│
├── ticket_prioritizer.ipynb
├── README.md

▶️ How to Run

Open the notebook in Google Colab

Install required libraries

Run all cells

Modify ticket text to test different cases

📌 Conclusion

The project demonstrates how transformer-based language models can be effectively used to automate IT ticket prioritization. By combining sentiment analysis with urgency detection, the system improves response efficiency and reduces manual workload.

👨‍🎓 Author

Christananda B
