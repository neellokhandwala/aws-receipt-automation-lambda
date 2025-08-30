# AWS Receipt Automation using Lambda, Textract, DynamoDB & SES  

## Project Overview  
This project is a **serverless automation workflow** built on AWS that extracts text data from uploaded receipts, stores it in a database, and notifies the user via email.  
It demonstrates **Cloud Computing + Automation** skills using AWS services and Python (boto3).  

**Use Case Example:**  
- Upload a receipt (or invoice) → System automatically extracts key information → Stores it in DynamoDB → Sends email notification with extracted details.  

---

**Workflow:**  
1. User uploads a file (PDF/JPG) to **Amazon S3**.  
2. **AWS Lambda** (triggered by S3) runs a script to:  
   - Use **Amazon Textract** to extract text.  
   - Store extracted data in **Amazon DynamoDB**.  
   - Send an email with the extracted data using **Amazon SES**.  
3. User receives an email confirmation with structured data.  

---

## Tech Stack  

- **AWS S3** → File storage (receipts/invoices)  
- **AWS Lambda** → Serverless automation (Python boto3 code)  
- **AWS Textract** → OCR for extracting text from receipts  
- **AWS DynamoDB** → NoSQL database for storing structured data  
- **AWS SES (Simple Email Service)** → Automated email notifications  
- **Python (boto3)** → AWS SDK for automation  

---

## 📂 Project Structure  

