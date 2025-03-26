# Deploying an Static website on AWS S3 Bucket:
# 🚀 Static Website Hosted on AWS S3

This repository documents the steps taken to deploy a **static website** on **AWS S3** and provides access to the hosted website.

## 📌 Project Overview
This project showcases how to:
- Upload and host a static website on AWS S3
- Enable public access to the website
- Configure bucket policies and permissions

## 🛠 Deployment Steps
### 1️⃣ Create an S3 Bucket
1. Navigate to **AWS S3 Console**
2. Click **Create Bucket** and provide a unique name
3. Disable "Block all public access" and acknowledge
4. Click **Create bucket**

### 2️⃣ Upload Website Files
1. Open your S3 bucket
2. Click **Upload** and select your `index.html`, `style.css`, and other assets

### 3️⃣ Configure Static Website Hosting
1. Go to the **Properties** tab
2. Scroll to **Static Website Hosting** and enable it
3. Set `index.html` as the default root document
4. Save the changes

### 4️⃣ Set Bucket Policy for Public Access
1. Go to the **Permissions** tab
2. Edit the **Bucket Policy** and paste:
   ```json
   {
     "Version": "2012-10-17",
     "Statement": [
       {
         "Effect": "Allow",
         "Principal": "*",
         "Action": "s3:GetObject",
         "Resource": "arn:aws:s3:::your-s3-bucket-name/*"
       }
     ]
   }
   ```
3. Save changes

### 5️⃣ Access Your Website
- The URL for your website will be available in the **Static Website Hosting** section.

## 📂 Repository Structure
```
📦 your-repo-name
 ┣ 📂 assets
 ┣ 📜 index.html
 ┣ 📜 style.css
 ┣ 📜 README.md
```
## ⭐ Contribute
Feel free to fork this repo, make improvements, and submit a **Pull Request**. 🚀

## 📧 Contact
For any queries, reach out at: **[your-email@example.com](mailto:anandgaurav69@gmail.com)**
<img width="1424" alt="Screenshot 2025-03-26 at 20 09 50" src="https://github.com/user-attachments/assets/4ab9b214-7294-43ae-8d48-0c93a39ad5cf" />
<img width="1424" alt="Screenshot 2025-03-26 at 20 09 36" src="https://github.com/user-attachments/assets/679dc81d-0497-4285-992d-969c3715e258" />
<img width="1433" alt="Screenshot 2025-03-26 at 20 09 14" src="https://github.com/user-attachments/assets/68a4f4fb-511d-40ce-b34e-e522e2d6e5a7" />
<img width="719" alt="Screenshot 2025-03-26 at 20 08 55" src="https://github.com/user-attachments/assets/4340fd21-a4e4-4744-9cf3-91825932b92c" />
