# Day 2 Progress – ServiceNow Project

## Module Completed: Table & Field Creation

### Tasks Completed:
- Created a **custom table** named **Network Database Table**  
  - Table Label: Network Database Table  
  - Table Name: u_network_database_table  
  - Application: Global  

- Added multiple **fields (columns)** to the table, including:
  - Customer Address (String)  
  - Request Number (String)  
  - Requested For (String)  
  - Assignment Group (Reference → Group table)  
  - Work Status (String)  
  - Device Details (String)  
  - Updates (Integer)  
  - Assigned To (Reference → User table)  
  - Date Of Enquiry (Date)  
  - Customer Document (String)  
  - Other system-generated fields (Created, Updated, Sys ID, Created by, Updated by, etc.)  

- Defined **field properties**:
  - Max length for string fields (default: 40 / 255 as required).  
  - Reference type fields for linking with other tables.  
  - Default values left empty for flexibility.  
  - Ensured proper naming conventions followed (auto-generated column names).  

- Verified the table and fields by opening the **Columns tab** under **System Definition > Tables**.  

---

### Evidence:
Screenshots have been uploaded to `/screenshots/module2/`:
- `Network Database Table.png` – showing the table creation.  
- `Creation Of Fields.png` – showing fields added to the table.  

---

### Deliverables:
- Update Set exported: `update-sets/NetworkDatabaseTable_Module2.xml`  
- Screenshots: `/screenshots/module2/`  
- Documentation: Updated `Day2.md`  

---

✅ **Module 2 (Table & Field Creation) completed successfully.**
