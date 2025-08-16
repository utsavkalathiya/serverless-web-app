#STATIC WEBSITE HOSTING ON S3
FIRST OF ALL, WE NEED TO CREATE A DIAGRAM ARCHITECTURE WHICH SHOWS what THE RESOURCES WILL BE REQUIRED TO COMPLETE THE PROJECT.

Let's get started

1. Frontend

index.html → Main HTML page.

styles.css → Styling.

app.js → JavaScript to call your backend APIs. Example:



4. README.md (Documentation)

Example outline:

# Serverless Web App on AWS

## Overview
This is a serverless web app built with AWS services:
- Frontend: S3 + CloudFront
- Backend: Lambda + API Gateway
- Database: DynamoDB
- IaC: AWS SAM

## Architecture
![Architecture Diagram](docs/architecture.png)

## How to Deploy
1. Clone this repo
2. Deploy backend:
   ```bash
   cd infrastructure
   sam build
   sam deploy --guided


Upload frontend to S3 bucket:

aws s3 sync frontend/ s3://<your-bucket-name>

Features

Create items

View items

Scales automatically with serverless


---

## ✅ Workflow for GitHub

1. Create a new repo on GitHub (`repo-nam`).  
2. Clone it locally:  
   ```bash
   git clone https://github.com/<your-username>/serverless-web-app.git
   cd serverless-web-app


Add your files (frontend, backend, infra).

Commit and push:

git add .
git commit -m "Initial commit - serverless web app"
git push origin main
