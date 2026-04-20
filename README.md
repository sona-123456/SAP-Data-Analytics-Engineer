

# 🚀 SAP PP Simulation — Plan to Produce Cycle (Python)

A complete **end-to-end simulation of SAP Production Planning (PP)** business process using Python.
This project replicates the real-world **manufacturing lifecycle** from demand planning to order settlement.

📌 Based on SAP T-Codes and real enterprise workflow.

---

## 📖 Project Overview

This simulation models the **Plan-to-Produce Cycle** used in SAP ERP:

```
PIR → MRP → Production Order → Goods Issue → Confirmation → Goods Receipt → Settlement
```

It demonstrates how manufacturing companies plan, execute, and track production along with **costing and analytics**.

---

## 🏢 Business Context

* **Company:** KIIT Industries Ltd.
* **Plant:** 1000 — Manufacturing Unit (BBSR)
* **Material:** FG-001 (Finished Goods)
* **Raw Materials:**

  * RM-A (Aluminium Block)
  * RM-B (Steel Fasteners)

---

## ⚙️ Key Features

✔ Full SAP PP lifecycle simulation
✔ Realistic **T-Code mapping (MD61, MD01, CO01, MIGO, CO11N, KO88)**
✔ Cost calculation:

* Raw Material Cost
* Machine Cost
* Labour Cost
* Overhead (11%)

✔ Inventory tracking (Stock updates)
✔ Production order lifecycle tracking
✔ Variance analysis (Planned vs Actual cost)
✔ SAP-style reports & analytics

---

## 🔄 Process Flow

### 1️⃣ Demand Planning (MD61)

* Create Planned Independent Requirement (PIR)

### 2️⃣ MRP Run (MD01)

* Generate Planned Orders
* Check component availability

### 3️⃣ Production Order Creation (CO01)

* Convert planned order → production order
* Calculate planned cost

### 4️⃣ Goods Issue (MIGO 261)

* Consume raw materials from inventory
* Update actual cost

### 5️⃣ Production Confirmation (CO11N)

* Confirm production quantity
* Add machine & labour cost
* Apply overhead

### 6️⃣ Goods Receipt (MIGO 101)

* Add finished goods to inventory

### 7️⃣ Order Settlement (KO88)

* Calculate variance
* Close production order

---

## 💰 Costing Logic

* **Raw Material Cost:** Based on BOM
* **Machine Cost:** ₹500/hour
* **Labour Cost:** ₹300/hour
* **Overhead:** 11% of total direct cost

---

## 📊 Reports Generated

* 📈 Production Order Status (COOIS)
* 💸 Cost Distribution
* 📦 MRP Coverage (MD04)
* 🏭 Work Center Utilization
* 📅 Planned vs Actual Production
* ⚖️ Cost Variance Analysis
* 📊 Stock Summary (MB52)

---

## 🧠 Concepts Covered

* SAP PP (Production Planning)
* MRP (Material Requirement Planning)
* BOM (Bill of Materials)
* Routing & Work Centers
* Cost Accounting (CO)
* Inventory Management (MM)
* Data Simulation using Python

---

## 🛠️ Tech Stack

* Python 3
* Dataclasses
* OOP Design
* Enum for status management

---

## ▶️ How to Run

```bash
python sap_pp_simulation.py
```

---

## 📂 Output

The script prints:

* SAP-style transaction logs
* Cost calculations
* Inventory updates
* Final summary table

---

## 🎯 Learning Outcome

This project helps you understand:

* How SAP PP works internally
* How manufacturing cost flows
* How different SAP modules integrate (MM + PP + CO)
* Real-world business process simulation

---

## 📌 Ideal For

* Data Analysts
* SAP Learners
* Supply Chain Enthusiasts
* Students preparing for ERP roles

---

## 👩‍💻 Author

**Sonali**
B.Tech CSE (2023–2027)
KIIT University

---

## 📎 File Reference

Main implementation file: 

---

## ⭐ Final Note

This is not just a Python script — it’s a **mini SAP system simulation** designed for learning, showcasing, and interview discussions.


