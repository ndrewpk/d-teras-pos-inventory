# D.TERAS POS & INVENTORY MANAGEMENT SYSTEM
## Senior Project Proposal Draft - IT483

---

## 1. Introduction

### 1.1 Document Structure
This proposal document outlines the development of an integrated Point-of-Sale (POS) and Inventory Management System for D.Teras restaurant in Jayapura, Sentani, Papua, Indonesia. The document is organized into the following sections:
- Introduction with project objectives
- Related works and similar solutions
- Preliminary investigation including company profile and problem analysis
- Project scope, constraints, and expected benefits
- System capabilities and development planning

### 1.2 Problem and Proposed Solution
D.Teras is a multi-division restaurant currently using Loyvers for POS transactions but lacks an integrated inventory management system. The restaurant operates three kitchen divisions (Bakery, Western Kitchen, Big Kitchen) and a Drink Bar with 17 staff members, handling approximately 10 million IDR in daily transactions. 

**Current Problems:**
- Stock levels drop unexpectedly without prior notification
- New supplies are purchased but not properly sorted or tracked
- Inventory is shared across all divisions but tracking is inconsistent
- Supply purchasing and checklists are entirely manual (paper-based)
- Multiple staff members make purchases without coordination
- No visibility into stock status before running out

**Proposed Solution:**
Develop an integrated POS and Inventory Management System that:
- Tracks inventory in real-time across all divisions
- Provides automated low-stock alerts
- Manages supplier information and purchase orders
- Records all supply purchases (bulk and small quantities)
- Generates inventory reports and analytics
- Integrates with the current POS system

### 1.3 Project Importance for Stakeholders
This system is critical for D.Teras because it will:
- **Reduce operational costs** by preventing stockouts and over-purchasing
- **Improve efficiency** by automating manual tracking processes
- **Enhance decision-making** through real-time inventory visibility
- **Prevent revenue loss** from unexpected supply shortages
- **Streamline purchasing** by coordinating multiple staff buyers
- **Enable scalability** as the restaurant grows

---

## 2. Related Works

### 2.1 Existing Solutions

**Loyvers (Current System)**
- Strengths: Already integrated with POS transactions, user-friendly interface
- Weaknesses: No inventory management module, no stock tracking, no purchase order management
- Advantages of Proposed System: Complete inventory ecosystem tailored to D.Teras operations

**Other POS Systems with Inventory:**
- **Toast POS** - Cloud-based, feature-rich but expensive and overkill for restaurant size
- **Square for Restaurants** - Good for small cafes but limited customization
- **MarginEdge** - Focuses on food cost management but requires separate POS
- **OpenPOS** - Open-source but requires technical expertise to customize

### 2.2 Why Our Proposed Solution is Better
Unlike existing solutions, our system will be:
- **Customized** to D.Teras's three-division structure
- **Cost-effective** with no licensing fees
- **Locally deployable** on D.Teras's own servers
- **Integrated** seamlessly with their current Loyvers POS
- **Scalable** for future growth and additional features

---

## 3. Preliminary Investigation

### 3.1 Company Profile

| Detail | Information |
|--------|-------------||
| **Company Name** | D.Teras (D.Teras Restaurant) |
| **Address** | Jayapura, Sentani, Papua, Indonesia |
| **Line of Business** | Food & Beverage - Multi-cuisine Restaurant |
| **Business Type** | Full-service restaurant with three kitchen divisions |
| **Contact Person** | Richard Kaihatu (Owner) |
| **Phone Number** | 0811484473 |
| **Email Address** | richardkaihatu2473@GMAIL.COM |
| **Number of Staff** | 17 employees |
| **Daily Revenue** | Approximately 10,000,000 IDR (Rp 10 juta) |
| **Operating Divisions** | Bakery, Western Kitchen, Big Kitchen, Drink Bar |

### 3.2 Organizational Chart

```
Owner (Richard Kaihatu)
│
├─ Kitchen Manager / Operations Lead
│  ├─ Bakery Division
│  ├─ Western Kitchen Division (Western Food)
│  ├─ Big Kitchen Division (Local Food)
│  └─ Drink Bar Division
│
├─ Finance/Purchase Manager
│  └─ Responsible for bulk purchasing and supplier coordination
│
└─ Staff (14 employees across divisions)
   ├─ Kitchen staff
   ├─ Cashiers/POS operators
   └─ Delivery/Purchasing staff (make local purchases by bike/car)
```

### 3.3 Statement of Mission/Goal of the Organization

**D.Teras Mission:** To provide high-quality, diverse food and beverage experiences across three culinary traditions (Bakery, Western, and Local Indonesian cuisine) in a welcoming atmosphere while maintaining operational excellence.

**Business Goals:**
- Increase operational efficiency and reduce food costs
- Maintain consistent quality and availability of menu items
- Improve customer satisfaction through reliable service
- Optimize purchasing and inventory management
- Enable data-driven business decisions

### 3.4 Project Request

**How the Project Was Initiated:**
The project emerged from direct operational challenges faced by D.Teras management:
- Owner Richard Kaihatu identified that while Loyvers handles POS well, the lack of inventory tracking creates significant operational problems
- The restaurant frequently experiences unexpected stockouts despite active purchasing
- Manual, paper-based inventory and purchasing processes are time-consuming and error-prone
- Multiple staff members purchasing supplies without centralized coordination leads to duplicated or missed purchases
- No mechanism to alert when stock levels become critical

**Request Details:**
- Develop an integrated inventory management system that works with existing Loyvers POS
- Provide real-time stock visibility across all three kitchen divisions
- Enable automated low-stock alerts
- Track all supply purchases (both bulk and small quantities)
- Generate reports for decision-making

### 3.5 Description of the Problem

**Core Problem:**
D.Teras operates with a **critical gap between POS transactions and inventory management**. While Loyvers records what is sold, there is no corresponding system to track what is in stock.

**Specific Issues:**

1. **Unexpected Stockouts:** Stock levels drop without prior notification, causing service disruptions and lost sales
   - Example: Running out of popular ingredients mid-service
   - Impact: Customer dissatisfaction, lost revenue

2. **Untracked Purchases:** New supplies bought by owner or staff are not immediately recorded or sorted
   - Multiple staff make independent purchases without coordination
   - Owner makes bulk purchases that aren't logged into any system
   - Staff make small purchases by bike that go untracked

3. **Manual Processes:** All inventory and purchasing is paper-based
   - Time-consuming daily counting
   - Prone to human error
   - No historical records or trends
   - Difficult to analyze spending patterns

4. **Lack of Coordination:** With 17 staff and multiple buyers, there's no visibility into who bought what and when
   - Risk of over-purchasing (waste)
   - Risk of under-purchasing (stockouts)
   - No supplier management

5. **No Analytics:** Owner cannot easily answer questions like:
   - Which items are used most frequently?
   - What is our average daily usage per item?
   - Which suppliers are most reliable/cost-effective?
   - What are our total inventory costs?

**Financial Impact:**
- Estimated monthly losses from stockouts: Unknown (but significant given 10M daily revenue)
- Wasted food from over-purchasing: Not quantified
- Staff time spent on manual tracking: Estimated 2-3 hours daily

### 3.6 Project Scopes and Constraints

#### **In Scope (What the System WILL Include):**

**Core Modules:**
1. **Inventory Module**
   - Real-time stock tracking for all items across 4 divisions
   - Low-stock threshold alerts
   - Stock adjustment and correction features
   - Inventory history and movement tracking

2. **Supplier Management**
   - Supplier database with contact information
   - Supplier pricing and terms
   - Purchase history per supplier

3. **Purchase Order Management**
   - Create and manage purchase orders
   - Track orders from placement to receipt
   - Record who made the purchase and when
   - Support for both bulk and small quantity purchases

4. **User Management**
   - Role-based access (Owner, Manager, Kitchen Staff, Cashier, Purchasing Staff)
   - User authentication and authorization
   - Activity logging

5. **Reporting**
   - Inventory status reports
   - Low-stock reports
   - Purchase history and spending reports
   - Inventory value reports
   - Daily/weekly/monthly summaries

6. **Integration**
   - API to sync with Loyvers POS for sales data (if possible)
   - Export capabilities (PDF, Excel reports)

#### **Out of Scope (What the System Will NOT Include):**

- Recipe management and food cost calculation (Phase 2)
- Employee payroll and human resources
- Complete POS replacement (will work alongside Loyvers)
- Mobile app (Phase 2)
- Multi-location support (Phase 2)
- Advanced AI/predictive ordering (Phase 2)
- Accounting/financial system integration (Phase 2)

#### **Constraints:**

**Technical Constraints:**
- Must work on local servers (no cloud requirement initially)
- Must be compatible with Loyvers data if possible
- Single database for all divisions
- Standard web browsers (Chrome, Firefox, Safari)

**Organizational Constraints:**
- Limited IT staff (owner will be primary user)
- Staff have limited technical training
- System must be user-friendly for non-technical users
- Minimal disruption to current operations during implementation

**Financial Constraints:**
- No licensing fees preferred (open-source or custom-built)
- Reasonable server hardware requirements
- Development timeline: 6 months total (IT483: 3 months, IT484: 3 months)

**Time Constraints:**
- Must be completed within IT483 (weeks 1-19) and IT484 (weeks 20-37) schedules
- Regular feedback cycles with owner required

### 3.7 Expected Business Benefits

| Benefit | Impact | Timeline |
|---------|--------|----------|
| **Reduced Stockouts** | Prevent lost sales and customer frustration | Immediate (Week 1 of deployment) |
| **Lower Inventory Costs** | Reduce over-purchasing and waste | 1-2 months post-launch |
| **Improved Efficiency** | Eliminate 2-3 hours daily manual tracking | Immediate |
| **Better Decision Making** | Data-driven purchasing based on usage trends | 1-2 months post-launch |
| **Supplier Coordination** | Centralized purchasing, better supplier relationships | 2-3 months post-launch |
| **Scalability** | Easy to add new items, divisions, or suppliers | Ongoing |
| **Staff Accountability** | Track who purchased what and when | Immediate |
| **Financial Visibility** | Know inventory value and costs at all times | Immediate |

**Estimated ROI:**
- Estimated savings from reduced waste: 500,000-1,000,000 IDR/month
- Estimated savings from reduced stockouts: 1,000,000-2,000,000 IDR/month
- **Total potential monthly savings: 1,500,000-3,000,000 IDR**
- System development cost: Estimated 3-5,000,000 IDR
- **ROI Payback Period: 2-3 months**

### 3.8 Expected System Capabilities

**Functional Capabilities:**

1. **Inventory Tracking**
   - Add, view, update, delete inventory items
   - Track quantity in stock, unit price, reorder point
   - Automatic low-stock alerts (configurable thresholds)
   - Inventory adjustments with reason tracking
   - Batch upload/import inventory data

2. **Supplier Management**
   - Add/manage supplier information
   - Track supplier pricing and lead times
   - Purchase history per supplier
   - Supplier performance metrics

3. **Purchase Orders**
   - Create POs with items, quantities, prices
   - Track PO status (Pending, Received, Partial)
   - Receive goods and update inventory automatically
   - Record purchasing staff and approval chain

4. **Reporting & Analytics**
   - Real-time inventory dashboard
   - Low-stock alerts and reports
   - Supplier performance reports
   - Spending trends and analysis
   - Inventory valuation reports
   - Export to PDF/Excel

5. **User Management**
   - Role-based dashboard (different views per role)
   - User authentication
   - Activity/audit logs
   - Permission management

6. **Data Security**
   - User authentication and authorization
   - Encrypted password storage
   - Encrypted data transmission (SSL/TLS)
   - Regular data backups
   - Access control by role

**Non-Functional Capabilities:**

- **Performance:** System must handle 50+ concurrent users with <2 second response time
- **Availability:** 99% uptime during business hours
- **Scalability:** Support up to 1,000+ inventory items
- **Usability:** Intuitive interface requiring minimal training
- **Reliability:** Automated backups, data integrity checks
- **Maintainability:** Clean, documented code for future updates

### 3.9 Planning

A detailed Gantt chart aligned with the IT483/IT484 schedule (Weeks 1-37) is provided below:

**IT483 Phase (Weeks 1-19):**
- **Week 1-4:** Proposal submission and approval
- **Week 5-6:** Requirements analysis and database design
- **Week 7-10:** System architecture and UI/UX design
- **Week 11-14:** Implementation of core inventory module
- **Week 15:** Submission of IT483 deliverables
- **Week 16-19:** IT483 defense preparation and presentation

**IT484 Phase (Weeks 20-37):**
- **Week 20-25:** Complete purchase order and supplier modules
- **Week 26-30:** Testing (unit, integration, system)
- **Week 31-32:** Acceptance testing with stakeholders
- **Week 33:** Submission of IT484 deliverables
- **Week 34-37:** IT484 defense preparation and presentation

---

## Document Information

**Document Prepared By:** Andrew Philips  
**Student ID:** 202300158  
**Date Prepared:** May 2026  
**Institution:** Asia-Pacific International University (AIU)  
**Course:** IT483 - Systems Development Project I  

**Client Contact:**
- **Name:** Richard Kaihatu
- **Organization:** D.Teras Restaurant
- **Phone:** 0811484473
- **Email:** richardkaihatu2473@GMAIL.COM
- **Location:** Jayapura, Sentani, Papua, Indonesia

---

*This proposal document follows the Senior Project Guidelines for BSc IT Programs at Asia-Pacific International University.*