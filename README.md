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

## 📊 Results and Observations

### Load Test Results
- Stable response time observed
- No request failures detected
- API handled normal traffic efficiently

---

### Stress Test Results
- Increased latency observed under high load
- Performance degradation occurred
- System remained functional

---

### Spike Test Results
- Sudden latency spikes detected
- Temporary performance instability occurred
- System recovered after load reduced

---

## 📈 Graph Explanation

The following graphs were generated using :contentReference[oaicite:0]{index=0}:

- load.html → Baseline performance under normal traffic
- stress.html → Performance under high load conditions
- spike.html → System behavior during sudden traffic surge

Each graph visualizes latency variation over time during testing.

---

## 🔍 Findings

- The API performs well under normal conditions
- Performance degrades under stress load conditions
- Spike traffic causes temporary latency increase
- No critical system failures were observed

---

## 📌 Conclusion

The JSONPlaceholder API demonstrates strong stability under normal traffic conditions. However, performance degradation is observed under high concurrency scenarios, indicating limited scalability for heavy load environments.

Overall, the API is suitable for testing and development purposes.

---

---

## 🚀 How to Run

```bash
vegeta attack -rate=10 -duration=30s -targets=targets.txt > load.bin
vegeta plot load.bin > load.html
