
---

## ⚙️ Key Components

### 1️⃣ Catalog Item – *Network Request*
- Linked with **Requestor Information variable set**
- Captures: Name, Email, Department, Location, Device Type, Justification  

### 2️⃣ Variable Set – *Requestor Information*
- Reusable set across catalog items  
- Contains unique variables (avoids naming conflicts)  

### 3️⃣ Custom Table – *u_network_database_table*
- Stores all network request records  
- Fields:
  - Requestor Name
  - Email ID
  - Department
  - Device Type
  - Location
  - Status (Pending, Approved, Rejected)

### 4️⃣ Flow Designer Automation
- **Actions Implemented:**
  - **Get Catalog Variables** – fetch request inputs  
  - **Create Record** – insert into custom table  
  - **Send Email** – notify stakeholders (Requestor, Approver)  
  - **Ask for Approval** – manager/approver verification  
  - **If Condition (Flow Logic)** – evaluate approval state  
  - **Update Record** – finalize request status  

### 5️⃣ Notifications
- Automated email templates with dynamic values (name, request ID, status).  
- Configured **To, CC, BCC** with static/dynamic fields.  

### 6️⃣ Approvals
- Approval mode: *Anyone Approves*  
- Configurable for static (specific approvers) or dynamic (from request data).  

---

## 🧪 Testing & Validation
- ✅ **Record Creation** – verified correct data mapping.  
- ✅ **Email Notification** – tested after enabling instance email properties.  
- ✅ **Approval Flow** – validated both *Approve* and *Reject* branches.  
- ✅ **Update Record** – confirmed correct status updates post-approval.  
- ⚠️ **Resolved Issues:**
  - Duplicate variable naming → fixed by unique internal names.  
  - Journal field `approval_history` warning → ignored (field not in table).  
  - Email sending disabled → enabled via *System Properties > Email*.  

---

## 📸 Screenshots
- 📌 *Network Database Table Design*  
- 📌 *Variable Set Configuration*  
- 📌 *Relationship Mapping*  
- 📌 *Flow Designer Workflow*  

(All included in project files)  

---

## 🚀 Outcomes
- Fully automated **Network Request workflow**.  
- Eliminated manual effort in tracking requests.  
- Increased efficiency with real-time **notifications & approvals**.  
- Showcases **ServiceNow Flow Designer expertise**.  

---

## 🛠️ Setup & Deployment

### Import into ServiceNow
1. Navigate to **System Update Sets > Retrieved Update Sets**.  
2. Import the provided `Update_Set_Export.xml`.  
3. Preview & Commit the update set.  

### Enable Email Notifications
- Go to **System Properties > Email**  
- Enable: `glide.email.smtp.active` and `glide.email.read.active`.  

### Testing the Flow
1. Open Service Catalog → Submit **Network Request**.  
2. Validate record in **u_network_database_table**.  
3. Check requestor/approver inbox for email notifications.  
4. Approve/Reject request → Verify updated status.  

---

## 📚 Learnings
- Designing **reusable variable sets** to prevent naming conflicts.  
- Mapping catalog variables to custom tables effectively.  
- Handling **ServiceNow email configurations**.  
- Building **end-to-end flows** with approvals & logic.  

---

## 🌟 Why This Project Stands Out
- Mirrors **real-world ITSM automation** scenarios.  
- Demonstrates **ServiceNow development expertise** across Catalog, Flows, Approvals, Notifications.  
- Recruiter-ready: **scalable, reusable, production-oriented**.  
- Mentor-ready: Clear documentation, screenshots, update set for import.  

---

## 👨‍💻 Author
**Khadir Shaik**  
*Java MERN Stack Developer | ServiceNow Enthusiast | AI-Driven Solutions Builder*  
🔗 [LinkedIn](https://www.linkedin.com) | 🔗 [GitHub](https://github.com)  

---
