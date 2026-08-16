# Leave Request Management System (Salesforce)

A complete Leave Management automation built on Salesforce using **Flows**, **Approval Processes**, **Email Alerts**, **Custom Objects**, and **Security Controls**.

---

## 🚀 Features

### 1️⃣ Custom Objects
- **Employee__c**
- **Leave_Request__c**

### 2️⃣ Leave Request Automation
- Record-Triggered Flow (Leave_Request_Automation)
- Auto email notifications:
  - Leave submitted → Manager notified
  - Manager approval → HR notified
  - HR approval → Employee notified
  - Manager rejection → HR notified
  - HR rejection → Employee notified

### 3️⃣ Approval Process
- **Step 1:** Manager Approval  
- **Step 2:** HR Approval  
- Status auto-updates:
  - Submitted → Manager Approved → HR Approved
  - Rejected (both levels)

### 4️⃣ Email Alerts
- Manager Submission Notification  
- HR Submission Notification  
- Manager Approval  
- HR Approval  
- Manager Rejection  
- HR Rejection  

### 5️⃣ Custom Fields
- Start Date  
- End Date  
- Status  
- Manager (Lookup: User)  
- HR (Lookup:User)  
- Employee (Lookup: Employee)  

---

## 📂 Project Structure (Salesforce DX)

```
force-app/
  main/
    default/
      objects/
      workflows/
      flows/
      email/
      approvalProcesses/
sfdx-project.json
```

---

## 💡 How It Works – End-to-End

1. Employee submits Leave Request  
2. Flow triggers automatically  
3. Manager receives an email  
4. Manager approves → HR receives an email  
5. HR approves → Employee notified  
6. Approval process updates final status  
7. If either Manager/HR rejects → Rejection emails sent automatically  

---

## 🛠️ Salesforce Technologies Used
- Record-Triggered Flow
- Approval Process
- Email Alerts & Templates
- Custom Objects & Fields
- Profiles & Users
- Validation Rules

---

## 📦 Installation (If someone wants to deploy)
Clone this repository and run:

```
sfdx force:source:deploy -p force-app
```

---

## ✨ Author
**Anjali Tarachandani**  


