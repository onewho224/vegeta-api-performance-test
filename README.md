# 🚀 Real-Time Load Testing and Performance Analysis of JSONPlaceholder API Using Vegeta

---

## 👤 Student Information
- Name: [Your Name]
- Matric ID: [Your ID]
- Course: ITT440 / NBCS2555A
- Title: Performance Testing Assignment

---

## 🎯 Project Objective

This project aims to evaluate the performance and scalability of a public REST API under different traffic conditions using a lightweight HTTP load testing tool.

The main objectives are:

- To measure API response time (latency)
- To evaluate system throughput under different loads
- To analyze system behavior under stress and spike conditions
- To identify potential performance bottlenecks

---

## 🌐 Target API

- API Endpoint: https://jsonplaceholder.typicode.com/posts
- Type: Public REST API (JSON-based)

---

## 🛠 Tools Used

- Vegeta HTTP Load Testing Tool
- Windows Command Prompt (CLI environment)

---

## 🧪 Test Scenarios

### 1. Load Test (Normal Traffic)
Simulates normal user behavior under expected system usage.

- Rate: 10 requests/second
- Duration: 30 seconds

---

### 2. Stress Test (High Traffic)
Evaluates system behavior under high concurrency.

- Rate: 100 requests/second
- Duration: 30 seconds

---

### 3. Spike Test (Sudden Traffic Surge)
Simulates sudden increase in user traffic (e.g., viral event).

- Rate: 200 requests/second
- Duration: 10 seconds

---

## ⚙️ Testing Methodology

All tests were executed using Vegeta CLI commands.

### Step 1: Prepare Target File
