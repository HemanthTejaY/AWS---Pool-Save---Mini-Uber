# POOL AND SAVE (Mini Uber)
##### [Video Demo LinK](https://youtu.be/ggagQbUG2p4)
## ABOUT
This project is a part of the final-project component for the course- Cloud Computing and Applications (CS-GY 9223, New York University) 
###### Authors: Indraneel Ray, Hemanth Teja
# 🏎️ AWS Pool Save - Mini Uber: A Serverless Ride-Sharing Platform with AI-Powered Rekognition System  

## 📌 Introduction  

**AWS Pool Save - Mini Uber** is an innovative **serverless ride-sharing application** designed to optimize **carpooling and ride management**. Built on **Amazon Web Services (AWS)**, it ensures **scalability, cost-effectiveness, and security** by integrating **AI-powered face verification with Amazon Rekognition**.  

### **🚀 Key Features**  
- ✅ **Real-time ride request handling** using **AWS Lambda** and **DynamoDB**.  
- ✅ **Intelligent driver-passenger matching** with AWS-based route optimization.  
- ✅ **Automated notifications** and ride updates via **Amazon SNS**.  
- ✅ **AI-powered face verification** for security using **Amazon Rekognition**.  
- ✅ **Serverless backend infrastructure** (AWS Lambda, API Gateway, DynamoDB, and S3).  

---

## 📌 System Architecture  

The system follows a **serverless microservices architecture**, ensuring high availability and **cost-efficient scaling**.  
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/2.jpg)


### **🛠️ Core AWS Components**  

### **1️⃣ AWS Lambda (Business Logic)**
Handles key ride-sharing workflows:  
- **`RideRequestHandler`** → Validates ride requests, calculates optimal routes, and identifies ride matches.  
- **`DriverAssignmentHandler`** → Retrieves available drivers, assigns based on location, and notifies via **Amazon SNS**.  
- **`RideCompletionHandler`** → Updates ride status, processes payments, and collects feedback.  

### **2️⃣ Amazon API Gateway**  
- 🌐 **Securely routes HTTP requests to AWS Lambda.**  
- 🔐 **Manages authentication using Amazon Cognito.**  

### **3️⃣ Amazon DynamoDB (NoSQL Database)**  
- 📊 Stores **user profiles, ride requests, driver availability, and ride history**.  
- ⚡ Provides **low-latency, high-throughput storage** for seamless user experience.  

### **4️⃣ Amazon S3 (Storage for Images & Logs)**  
- 🖼️ **Stores driver and passenger profile images.**  
- 📂 **Maintains ride history logs for compliance & analytics.**  

### **5️⃣ Amazon Rekognition (AI-Powered Face Verification)**  
- 🛡️ **Enhances security by verifying driver and passenger identities.**  
- 🚫 **Prevents unauthorized ride access and fraud.**  

---

## 📌 AI-Powered Rekognition Feature  

The **AI-based identity verification system** ensures security and trust in ride-sharing.  

### **👤 Face Verification Workflow**  
**1️⃣ Driver Verification** → Matches **real-time selfie** with registered profile photo.  
**2️⃣ Passenger Verification (Optional)** → High-security rides require identity authentication before boarding.  

### **🔍 How Amazon Rekognition Works**  

#### **📌 Step 1: Image Capture**
- 📸 Driver takes a **real-time selfie** before starting a ride.  
- 🖼️ Image is **uploaded to Amazon S3**.  

#### **📌 Step 2: Face Matching Against Database**
- 🎯 **Amazon Rekognition CompareFaces API** validates identity.  
- ✅ **Success if similarity score > 90%**; else, triggers **manual review**.  

#### **📌 Step 3: Security & Approval**
- 🚦 **Approved rides continue; flagged cases require admin intervention.**  

### **🔹 AI Model Architecture**
- 🏗 **Deep Learning-based Convolutional Neural Networks (CNNs).**  
- 🔍 **Embeds facial features & compares using cosine similarity.**  

### **🔹 Security Benefits**
✅ **Eliminates fraudulent rides & identity theft.**  
✅ **Enhances trust & safety in carpooling services.**  
✅ **Seamless AI-powered authentication with AWS scalability.**  

---

## 📌 Benefits of the AI-Powered AWS Architecture  

### **⚡ Scalability & Performance**
- 🚀 **Serverless AWS Lambda auto-scales based on ride demand.**  
- 💰 **No infrastructure maintenance costs.**  

### **💰 Cost Optimization**
- **Pay-as-you-go pricing for Amazon Rekognition & AWS Lambda.**  
- **Optimized compute resources reduce unnecessary spending.**  

### **🔒 Security & Compliance**
- **AWS IAM & Cognito secure user authentication.**  
- **Face verification reduces identity fraud.**  

---

## 📌 Future Improvements 🚀  
✔ **Enhance AI-driven ride-matching algorithms.**  
✔ **Integrate LLM-based chatbots for automated ride assistance.**  
✔ **Optimize ride pricing using reinforcement learning.**  

---

## 📌 Key Technologies Used  

| Technology  | Purpose |
|-------------|---------|
| **AWS Lambda** | Serverless compute for ride request processing |
| **Amazon Rekognition** | AI-powered face verification for security |
| **Amazon API Gateway** | Secure API management for ride operations |
| **Amazon DynamoDB** | High-performance NoSQL database for ride data |
| **Amazon SNS** | Real-time notifications for ride updates |
| **Amazon Cognito** | User authentication & access management |
| **Amazon S3** | Secure storage for images & ride logs |

---

## 📌 Conclusion  
The **AWS Pool Save - Mini Uber project** integrates **AI-driven security, scalable cloud computing, and real-time optimization** to provide an **intelligent, secure, and cost-effective** ride-sharing experience.  

By leveraging **Amazon Rekognition for fraud detection**, **serverless AWS architecture for cost efficiency**, and **AI-based ride-matching for seamless coordination**, the system **sets new benchmarks in AI-powered transportation technology.**  

---

📌 **GitHub Repository:** [PoolSave Repo](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber)  

 
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/1.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/3.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/4.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/5.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/6.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/7.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/8.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/9.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/10.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/11.jpg)
![alt text](https://github.com/HemanthTejaY/AWS---Pool-Save---Mini-Uber/blob/master/project-images/12.jpg)




