Try Link - https://rajmulik511.github.io/GitaverseAi/

# GitaverseAi 🤖

**A serverless, scalable, and cost-effective Generative AI chatbot built on AWS.**

GitaverseAi leverages Amazon Bedrock's **Titan Large Language Model (LLM)** to deliver intelligent, context-aware responses to user queries — all through a fully serverless architecture designed for scalability and low operational cost.

---

## 🚀 Overview

GitaverseAi demonstrates an end-to-end serverless GenAI application on AWS — from a secure REST API backend to a globally-delivered static frontend, with CI/CD baked in from day one.

---

## 🏗️ Architecture

```
User → AWS Amplify (Frontend) → Amazon API Gateway → AWS Lambda → Amazon Bedrock (Titan LLM)
                                                              ↓
                                                     AWS IAM (Least-Privilege Access)
```

---

## ✨ Key Features

- **Backend & API**
  Serverless backend built on AWS Lambda to process business logic and orchestrate API calls, exposed through a secure RESTful API via Amazon API Gateway (request routing, validation, and authorization).

- **AI Integration**
  Integrated with Amazon Bedrock to invoke the Titan Foundation Model, enabling advanced natural language understanding and generative AI capabilities for the chatbot's core functionality.

- **Security & Permissions**
  Implemented a least-privilege security model using AWS IAM roles and policies, ensuring the Lambda function only has the exact permissions needed to invoke Amazon Bedrock.

- **Frontend & Deployment**
  User-facing static web app deployed on Amazon S3 with global delivery via AWS Amplify Hosting, with a CI/CD workflow integrated with GitHub for seamless deployment and version control.

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| Cloud Provider | Amazon Web Services (AWS) |
| Generative AI | Amazon Bedrock (Titan LLM) |
| Compute | AWS Lambda |
| API Layer | Amazon API Gateway |
| Security/IAM | AWS IAM |
| Storage/Hosting | Amazon S3, AWS Amplify Hosting |
| CI/CD & VCS | GitHub, AWS Amplify CI/CD |
| Language | Python |
| Architecture Style | Serverless, REST API |

---

## 📦 Project Structure

```
GitaverseAi/
├── backend/          # AWS Lambda functions (business logic, Bedrock invocation)
├── frontend/          # Static web application
├── api/               # API Gateway configuration/specs
├── iam/                # IAM role and policy definitions
└── README.md
```
*(Adjust to match your actual repo structure.)*

---

## ⚙️ How It Works

1. The user interacts with the chatbot through the frontend hosted on **AWS Amplify**.
2. Requests are routed through **Amazon API Gateway**, which validates and authorizes each call.
3. **AWS Lambda** processes the request and invokes **Amazon Bedrock's Titan LLM** to generate a context-aware response.
4. **IAM roles and policies** enforce least-privilege access between Lambda and Bedrock at every step.
5. Responses are returned to the frontend in real time.

---

## 🔒 Security

- Least-privilege IAM roles scoped specifically to Bedrock invocation
- No hardcoded credentials — all access managed via IAM policies
- API Gateway handles request validation and authorization before requests reach the backend

---

## 📈 Why Serverless?

- **Cost-effective:** Pay only for actual compute/API usage — no idle server costs
- **Scalable:** Automatically scales with traffic, no manual provisioning
- **Low maintenance:** No servers to patch or manage

---

## 🙋 Author

**Raj Jaywant Mulik**
[GitHub](https://github.com/Rajmulik511) • [LinkedIn](https://www.linkedin.com/in/raj-mulik-4675a6158)

---

## 📄 License

This project is available under the MIT License.
