# Real-Time Load Testing and Performance Analysis of JSONPlaceholder API Using Vegeta

---

## Student Information
- Name: [Your Name]
- Matric ID: [Your ID]
- Course: ITT440 / NBCS2555A

---

## Objective

This project evaluates the performance of a public REST API under different traffic conditions using a load testing tool.

Objectives:
- Measure API response time
- Evaluate system performance under load
- Analyze stress and spike behavior

---

## API Target

https://jsonplaceholder.typicode.com/posts

---

## Tools Used

- Vegeta (HTTP Load Testing Tool)
- Windows Command Prompt

---

## Test Scenarios

### Load Test
- 10 requests/second
- 30 seconds

### Stress Test
- 100 requests/second
- 30 seconds

### Spike Test
- 200 requests/second
- 10 seconds

---

## Methodology

### Step 1: Create targets.txt

GET https://jsonplaceholder.typicode.com/posts

---

### Step 2: Load Test

vegeta attack -rate=10 -duration=30s -targets=targets.txt > load.bin  
vegeta plot load.bin > load.html  

---

### Step 3: Stress Test

vegeta attack -rate=100 -duration=30s -targets=targets.txt > stress.bin  
vegeta plot stress.bin > stress.html  

---

### Step 4: Spike Test

vegeta attack -rate=200 -duration=10s -targets=targets.txt > spike.bin  
vegeta plot spike.bin > spike.html  

---

## Results

### Load Test
- Stable performance
- No failures

### Stress Test
- Higher latency
- Performance degradation

### Spike Test
- Sudden spikes
- Temporary instability

---

## Findings

- API works well under normal load
- Performance drops under stress
- Spike causes temporary delay

---

## Conclusion

API is stable for normal usage but not optimized for high traffic.

---

## Repository Structure

vegeta-api-performance-test/  
├── load/  
├── stress/  
├── spike/  
├── targets.txt  
└── README.md  

---

## How to Run

vegeta attack -rate=10 -duration=30s -targets=targets.txt > load.bin  
vegeta plot load.bin > load.html  

Change rate:
- Stress = 100
- Spike = 200
