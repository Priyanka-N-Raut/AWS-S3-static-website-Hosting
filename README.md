# AWS-S3-static-website-Hosting

# 🌐 Static Resume Website using AWS S3

This project demonstrates how to host a static resume/portfolio website using AWS S3 without provisioning any servers.

The website is built using HTML and CSS and deployed using AWS S3 Static Website Hosting.

---

## 🚀 Project Overview

- Built a responsive resume website using HTML & CSS
- Hosted the website using AWS S3
- Configured bucket policy for public access
- Enabled Static Website Hosting
- Achieved serverless deployment with zero infrastructure management

---

## 🛠️ Technologies Used

- HTML5
- CSS3
- AWS S3
- AWS IAM

---

## 📁 Project Structure

resume-website/
│── index.html
│── style.css


---

## 🪜 Deployment Steps

### 1️⃣ Create S3 Bucket
- Go to AWS S3
- Create a new bucket (unique name)
- Disable "Block All Public Access"

### 2️⃣ Upload Files
- Upload `index.html`
- Upload `style.css`

### 3️⃣ Enable Static Website Hosting
- Go to Properties
- Enable Static Website Hosting
- Set index document as:
index.html


### 4️⃣ Add Bucket Policy

Replace `your-bucket-name` in the policy below:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}
🌍 Live Website
After enabling static hosting, access your website using:

http://your-bucket-name.s3-website-region.amazonaws.com
📌 Key Learnings
Hosting static websites without servers

Configuring S3 bucket policies

Understanding public access control in AWS

Cost-effective cloud deployment

💰 Cost
Free Tier eligible

No charges when idle

Pay only for storage and minimal requests

👩‍💻 Author
Priyanka Raut
DevOps Engineer | Cloud Enthusiast
