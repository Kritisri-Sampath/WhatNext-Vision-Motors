# WhatNext-Vision-Motors
Salesforce project
# 🚗 WhatNext Vision Motors

### Salesforce CRM for Automotive Business Management

**WhatNext Vision Motors** is a Salesforce CRM application designed to manage the day-to-day operations of an automotive business. The system brings **vehicles, customers, dealers, orders, test drives, and service requests** into a single Salesforce environment.

The project combines **Salesforce declarative automation and programmatic development using Apex** to reduce manual work, improve data accuracy, and simplify automotive business operations.

---

## 📌 Project Overview

The system provides a centralized platform for managing automotive sales and customer-related activities.

Key processes include:

* 🚘 Vehicle management
* 👤 Customer management
* 🏢 Dealer management
* 🛒 Vehicle order management
* 🚗 Test-drive scheduling
* 🔧 Vehicle service requests
* ⚡ Automated dealer assignment
* 📦 Vehicle stock validation
* 📧 Test-drive reminder emails
* 📊 Reports and dashboards
* 🔐 Role-based access and security

The project was developed using a **Salesforce Developer Edition Org**.

---

## 🎯 Objectives

* Centralize automotive business information
* Improve vehicle order processing
* Reduce repetitive manual activities
* Maintain accurate and consistent data
* Provide a simple Lightning-based user experience
* Automate rule-based business processes
* Improve visibility through reports and dashboards

---

## 🏗️ Salesforce Architecture

### Custom Objects

The application uses six main custom objects:

| Object                         | Purpose                                             |
| ------------------------------ | --------------------------------------------------- |
| 🚘 **Vehicle**                 | Stores vehicle model, price, stock and availability |
| 🏢 **Dealer**                  | Stores dealer details and contact information       |
| 👤 **Customer**                | Stores customer information                         |
| 🛒 **Vehicle Order**           | Manages vehicle purchase orders                     |
| 🚗 **Vehicle Test Drive**      | Manages test-drive bookings                         |
| 🔧 **Vehicle Service Request** | Tracks customer service requirements                |

These objects are connected through relationships to avoid duplicate data and keep related records easily accessible.

---

## ⚡ Automation

### Salesforce Flow

Salesforce Flow is used to automate repetitive business processes.

#### 1. Auto Assign Dealer

Automatically assigns a suitable dealer when a new vehicle order is created.

#### 2. Test Drive Reminder

Automatically sends reminder emails before scheduled test drives.

---

## 💻 Apex Development

Apex is used for business logic and transaction processing.

### Apex Classes

* Vehicle Order Processing
* Stock Validation
* Order Management
* Reusable business logic

The business logic is separated into handler/classes instead of placing everything directly inside triggers, making the implementation easier to maintain and test.

### Apex Trigger

The **Vehicle Order Trigger** handles important order-related events.

Main responsibilities:

* Check vehicle stock availability
* Prevent invalid orders
* Update vehicle stock after confirmation
* Support order-status changes
* Delegate processing to the trigger handler

---

## 🛡️ Validation

A vehicle stock validation rule prevents an order from being confirmed when the selected vehicle does not have enough stock.

For example:

```text
Vehicle Stock = 0
        ↓
User confirms order
        ↓
Validation Check
        ↓
❌ Order blocked
```

This prevents invalid transactions from entering the system.

---

## 🎨 User Interface

The project uses **Salesforce Lightning Experience** to provide a structured user interface.

### Lightning Features

* Lightning App
* App Manager
* Page Layouts
* Dynamic Forms
* Lightning Record Pages
* Related Lists
* Highlights Panels
* Reports
* Dashboards

A single **WhatNext Vision Motors Lightning App** provides access to Vehicles, Dealers, Customers, Orders, Test Drives, and Service Requests.

---

## 🔐 Security

The project implements Salesforce security features including:

* Profiles
* Roles
* Role Hierarchy
* Permission Sets
* Object-Level Permissions
* Sharing Rules

These controls help ensure users receive access according to their responsibilities.

---

## 🧪 Testing

Major functionality was tested using different test cases.

### Test Cases

**1. Vehicle Creation**

* Create a valid vehicle
* Verify that the record saves successfully

**2. Out-of-Stock Order**

* Select a vehicle with no stock
* Attempt to confirm the order
* Verify that the system blocks the transaction

**3. Test Drive Reminder**

* Create a scheduled test drive
* Verify that the reminder email is triggered

**4. Pending Order Processing**

* Create a pending order
* Make vehicle stock available
* Verify that the pending order is processed correctly.

---

## 🛠️ Technology Stack

| Technology                          | Usage                        |
| ----------------------------------- | ---------------------------- |
| **Salesforce CRM**                  | Main development platform    |
| **Salesforce Lightning Experience** | User interface               |
| **Apex**                            | Backend/business logic       |
| **Apex Triggers**                   | Transaction-based automation |
| **Salesforce Flow**                 | Declarative automation       |
| **SOQL**                            | Salesforce data querying     |
| **Custom Objects & Fields**         | Data modelling               |
| **Reports & Dashboards**            | Business analytics           |
| **Permission Sets & Roles**         | Security                     |

---

## 🔄 Project Workflow

```text
Customer
   ↓
Vehicle Selection
   ↓
Vehicle Availability Check
   ↓
Create Vehicle Order
   ↓
Auto Dealer Assignment
   ↓
Order Processing
   ↓
Update Vehicle Stock
   ↓
Order Confirmation
```

Additional workflows:

```text
Customer
   ↓
Book Test Drive
   ↓
Scheduled Date
   ↓
Automated Reminder Email
```

---

## 📊 Key Features

### 🚘 Vehicle Management

Manage vehicle information, availability, pricing and stock.

### 👤 Customer Management

Maintain customer records for purchases, test drives and service.

### 🏢 Dealer Management

Store and manage dealership information.

### 🛒 Order Management

Create and process vehicle orders with automatic stock validation.

### 🚗 Test Drive Management

Schedule and manage customer test drives with automated reminders.

### 🔧 Service Management

Record customer vehicle service requirements.

### ⚡ Business Automation

Use Salesforce Flow and Apex to automate repetitive operations.

### 📈 Reports & Dashboards

Provide management with visual summaries of business activity.

### 🔐 Security

Control access using Salesforce profiles, roles, permission sets and sharing rules.

---

## 📈 Key Outcomes

The project successfully demonstrates:

* Centralized automotive CRM management
* Automated vehicle stock validation
* Automatic dealer assignment
* Automated test-drive reminders
* Vehicle order processing
* Customer and dealer management
* Service request tracking
* Salesforce Lightning UI customization
* Role-based security
* Reports and dashboards
* Apex and Flow integration

---

## 👩‍💻 Developer

**Kritisri Sampath Kumar**

🎓 R.M.K. Engineering College
💻 Computer Science and Design

---

## ⭐ Project Highlights

> **WhatNext Vision Motors demonstrates how Salesforce CRM, Flow, Apex, Lightning Experience, and security features can be combined to build a complete automotive business management solution.**

---

## 📌 Future Enhancements

Possible future improvements include:

* Customer self-service portal
* Online vehicle booking
* Payment integration
* Advanced sales analytics
* AI-based vehicle recommendations
* Mobile application integration
* Automated service appointment scheduling

---

### 🔗 Salesforce

Built and configured using a **Salesforce Developer Edition Org**.

