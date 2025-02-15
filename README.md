
# 🚀 TDS_Project LLM-Based Automation Agent  

Welcome to the **LLM-Based Automation Agent**! This intelligent automation system leverages **Natural Language Processing (NLP)** and **Large Language Models (LLMs)** to efficiently execute a variety of tasks.

---

## 🌟 Features  

✅ **Intelligent Task Parsing** – Powered by **GPT-4o-Mini** for accurate task interpretation.  
✅ **Secure File Handling** – Ensures safe and secure processing of sensitive files.  
✅ **Multi-Task Support** – Efficiently handles multiple task types simultaneously.  
✅ **API-Driven Execution** – Integrates with powerful APIs for seamless task execution.  

---

## 📋 Prerequisites  

Before running the project, ensure you have the following installed:  

- 🐳 **Docker** – For containerization and deployment.  
- 🔑 **AI Proxy Token** – Required for accessing LLM functionalities.  

---

## ⚙️ Installation & Run  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/shailja-gramener2025/tds_project_my_llm_agent.git
cd tds_project_my_llm_agent
```

### 2️⃣ Install Dependencies (For Local Execution)  
```bash
pip install -r requirements.txt
```

### 3️⃣ Setup Environment Variables  
Create a `.env` file in the project root and add your AI proxy token:  
```bash
echo "AIPROXY_TOKEN=your_token_here" > .env
```

### 4️⃣ Run Locally (Without Docker)  
```bash
python run.py
```

---

## 🐳 Using Docker  

### 1️⃣ Build the Docker Image  
```bash
docker build -t tdsimage .
```

### 2️⃣ Run the Container  
```bash
docker run -d --env-file .env -p 8000:8000 tdsimage
```

---

## 🚢 Deploying to Docker Hub  

### 1️⃣ Log in to Docker Hub  
```bash
docker login
```

### 2️⃣ Check Your Docker Images  
```bash
docker images
```
🔹 **Find the IMAGE ID** for `tdsimage` from the list.

### 3️⃣ Tag the Image  
```bash
docker tag <image_id> shailja197/tdsimage:latest
```

### 4️⃣ Push the Image to Docker Hub  
```bash
docker push shailja197/tdsimage:latest
```

---

