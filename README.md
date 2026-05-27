# D.Teras POS & Inventory Management System

## Project Overview

This is a Senior Project for Asia-Pacific International University (AIU) - IT483/IT484 Systems Development Project.

**Project:** Integrated Point-of-Sale (POS) and Inventory Management System for D.Teras Restaurant  
**Student:** Andrew Philips (202300158)  
**Client:** Richard Kaihatu, D.Teras Restaurant, Jayapura, Sentani, Papua, Indonesia  
**Timeline:** 6 months (IT483: Weeks 1-19, IT484: Weeks 20-37)

## Problem Statement

D.Teras is a multi-division restaurant (Bakery, Western Kitchen, Big Kitchen, Drink Bar) with 17 staff members handling approximately 10 million IDR in daily transactions. While using Loyvers for POS, the restaurant lacks an integrated inventory management system, resulting in:

- Unexpected stockouts without prior notification
- Untracked supply purchases (both bulk and small quantities)
- Manual, paper-based inventory and purchasing processes
- No coordination among multiple staff buyers
- No visibility into inventory trends or supplier performance

## Proposed Solution

Develop a comprehensive, web-based Inventory Management System featuring:

- **Real-time Inventory Tracking** across all divisions
- **Automated Low-Stock Alerts** with configurable thresholds
- **Purchase Order Management** for centralized purchasing coordination
- **Supplier Management** with performance tracking
- **Advanced Reporting & Analytics** for data-driven decisions
- **Role-Based Access Control** for staff management
- **Integration with Loyvers POS** for seamless operation

## Expected Business Benefits

- Reduce stockouts and prevent lost sales
- Lower inventory costs through optimized purchasing
- Eliminate 2-3 hours of daily manual tracking
- Enable data-driven business decisions
- **Estimated ROI: 2-3 months**

## Technology Stack

- **Frontend:** React.js with modern UI/UX design
- **Backend:** Node.js + Express.js
- **Database:** MySQL with automated backup policies
- **Deployment:** Local server (on-premises)
- **Security:** User authentication, encrypted communication (SSL/TLS), role-based access control

## Project Structure

```
d-teras-pos-inventory/
├── docs/                          # Documentation and reports
│   ├── Senior_Project_Proposal_Draft.md
│   ├── IT483_Report.md
│   └── IT484_Report.md
├── src/
│   ├── frontend/                  # React.js application
│   ├── backend/                   # Node.js/Express API
│   └── database/                  # MySQL schema and migrations
├── tests/                         # Unit, integration, system tests
├── deployment/                    # Installation & operations docs
├── documentation/                 # User and admin manuals
└── README.md                      # This file
```

## Key Milestones

### IT483 Phase (Weeks 1-19)
- ✅ Week 1-4: Proposal submission and approval
- ⏳ Week 5-6: Requirements analysis and database design
- ⏳ Week 7-10: System architecture and UI/UX design
- ⏳ Week 11-14: Implementation of core inventory module
- ⏳ Week 15: Submission of IT483 deliverables
- ⏳ Week 16-19: IT483 defense

### IT484 Phase (Weeks 20-37)
- ⏳ Week 20-25: Complete purchase order and supplier modules
- ⏳ Week 26-30: Testing (unit, integration, system)
- ⏳ Week 31-32: Acceptance testing with stakeholders
- ⏳ Week 33: Submission of IT484 deliverables
- ⏳ Week 34-37: IT484 defense

## Stakeholders

- **Primary User:** Richard Kaihatu (Owner/Decision Maker)
- **Secondary Users:** Kitchen staff, Purchase managers, Cashiers
- **Evaluation Committee:** AIU Faculty members (TBD)
- **Adviser:** (To be assigned upon proposal approval)

## System Requirements

### Functional Requirements
- CRUD operations for inventory items, suppliers, and purchase orders
- Automatic low-stock alerts (configurable per item)
- Real-time inventory tracking across divisions
- Purchase order workflow management
- Comprehensive reporting and analytics
- User authentication and role-based authorization
- Activity/audit logging

### Non-Functional Requirements
- Support 50+ concurrent users
- <2 second response time for typical operations
- 99% uptime during business hours
- Support 1,000+ inventory items
- Intuitive interface with minimal training required
- Data encryption and regular automated backups

## Minimum Complexity Standards

Per AIU guidelines, this Management Information System meets minimum requirements:

- **Security:** User authentication, encrypted communication, role-based access
- **Remote Database:** MySQL server with backup policies
- **Web Framework:** React.js (frontend) + Node.js/Express (backend)
- **Data Objects:** 7+ entities (Items, Suppliers, PurchaseOrders, Users, Divisions, Categories, etc.)
- **Use Cases:** 30+ windows/screens for full functionality

## Contact Information

**Student:**  
Andrew Philips (202300158)  
Asia-Pacific International University  

**Client:**  
Richard Kaihatu (Owner)  
D.Teras Restaurant  
Jayapura, Sentani, Papua, Indonesia  
Phone: 0811484473  
Email: richardkaihatu2473@GMAIL.COM  

## License

© Asia-Pacific International University 2026. All rights reserved.

This senior project's deliverables (software and reports) are copyright of Asia-Pacific International University. The student author has full authority to distribute or commercially exploit the software and technical documentation of the project.

---

**Last Updated:** May 2026  
**Status:** Proposal Phase (Week 1-4)  
**Next Step:** Proposal approval and adviser assignment