# 🚀 Real-Time Load Testing and Performance Analysis of JSONPlaceholder API Using Vegeta

---

## 👤 Student Information
- Name: [Your Name]
- Matric ID: [Your ID]
- Course: ITT440 / NBCS2555A

---

## 🎯 Project Objective

This project aims to evaluate the performance and scalability of a public REST API under different traffic conditions using a lightweight HTTP load testing tool.

The objectives are:

- To measure API response time (latency)
- To evaluate throughput under different loads
- To analyze system behavior under stress and spike conditions
- To identify performance bottlenecks

---

## 🌐 Target API

- API Endpoint: https://jsonplaceholder.typicode.com/posts  
- Type: Public REST API (JSON format)

---

## 🛠 Tools Used

- :contentReference[oaicite:0]{index=0}  
- Windows Command Prompt (CLI)

---

## 🧪 Test Scenarios

### 1. Load Test (Normal Traffic)
Simulates normal user behavior.

- Rate: 10 requests/second  
- Duration: 30 seconds  

---

### 2. Stress Test (High Traffic)
Evaluates system performance under heavy load.

- Rate: 100 requests/second  
- Duration: 30 seconds  

---

### 3. Spike Test (Sudden Traffic Surge)
Simulates sudden traffic increase (e.g., viral event).

- Rate: 200 requests/second  
- Duration: 10 seconds  

---

## ⚙️ Methodology

### Step 1: Create Target File

Create `targets.txt`:

```text
GET https://jsonplaceholder.typicode.com/posts
