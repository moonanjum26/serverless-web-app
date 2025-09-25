# serverless-web-app

A **serverless web application** built on **AWS** that allows students' information management.  
The project demonstrates how to combine **DynamoDB, Lambda, API Gateway, S3, and CloudFront** into a secure, scalable, and globally available application.  

---


**Workflow:**
1. **Frontend**: Hosted on **Amazon S3** (static website with `index.html` + `script.js`).
2. **Content Delivery**: Distributed securely with **Amazon CloudFront** (using OAC, S3 remains private).
3. **API Gateway**: Exposes REST API endpoints for student operations.
4. **AWS Lambda**: Executes backend logic on demand:
   - `insertStudent` → Add a new student record  
   - `getStudent` → Retrieve student by ID  
5. **Amazon DynamoDB**: Stores student data (NoSQL table).

---

## 🛠️ Services Used

- **Amazon DynamoDB** → NoSQL table `student` with primary key `studentId`.
- **AWS Lambda** → Event-driven compute for CRUD operations.
- **Amazon API Gateway** → REST API with GET & POST methods + CORS enabled.
- **Amazon S3** → Static website hosting for frontend files.
- **Amazon CloudFront** → Secure CDN distribution, ensures private bucket access with OAC.

---


