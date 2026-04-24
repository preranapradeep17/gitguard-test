 🧪 GitGuard Test Repository

This repository is used to test GitGuard AI, an automated pull request analysis system.

It is intentionally designed to create Pull Requests (PRs) that trigger webhook events and simulate real-world development scenarios.

---

## 🎯 Purpose

- Generate Pull Requests  
- Trigger GitHub Webhooks  
- Test GitGuard AI backend  
- Simulate buggy and real-world code changes  

---

## 🔗 Connected System

This repository is connected to:

👉 GitGuard AI Backend

When a Pull Request is opened here:
1. GitHub sends a webhook event  
2. GitGuard AI receives it  
3. Verifies the request  
4. Processes PR data  
5. Logs or analyzes the changes  

---

## ⚙️ How to Use This Repo

### 1. Create a new branch

bash git checkout -b feature-test 

---

### 2. Add or modify code

Example (intentional bug):

js let total = items.length - 1; // off-by-one error 

---

### 3. Commit and push

bash git add . git commit -m "Test PR with bug" git push origin feature-test 

---

### 4. Open Pull Request

Go to GitHub and click:

👉 Compare & Pull Request

---

## 🧪 Expected Behavior

Once PR is created:

- Webhook is triggered  
- GitGuard AI backend receives event  
- PR details are logged in backend terminal  

---

## 🧾 Example Output (Backend)

bash Received event: pull_request New PR Detected Title  : Test PR with bug Author : username Repo   : username/gitguard-test 

---

## ⚠️ Important Notes

- This repo is for testing only  
- Code may intentionally contain bugs  
- Do not use this repo for production code  

---

## 🔐 Webhook Setup

Ensure this repository has a webhook configured:

- Payload URL:
https://your-ngrok-url/webhook

- Content type:
application/json

- Secret:
(same as backend .env WEBHOOK_SECRET)

- Events:
Pull Requests

---

## 🧠 Testing Ideas

Try creating PRs with:

- Logic bugs  
- Syntax errors  
- Security issues  
- Performance problems  

This helps validate GitGuard AI functionality.

---

## 📌 Status

Active testing repository for GitGuard AI  

---

## 👩‍💻 Author

Prerana Pradeep
