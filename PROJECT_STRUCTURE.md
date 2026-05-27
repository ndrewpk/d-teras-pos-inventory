# D.Teras POS & Inventory System - Project Structure

## Directory Layout

```
d-teras-pos-inventory/
│
├── docs/                          # Documentation and reports
│   ├── Senior_Project_Proposal_Draft.md    # Initial proposal (Weeks 1-4)
│   ├── IT483_Report.md                     # Full IT483 report (Weeks 5-15)
│   ├── IT484_Report.md                     # Full IT484 report (Weeks 20-33)
│   ├── requirements/
│   │   ├── functional_requirements.md
│   │   ├── non_functional_requirements.md
│   │   └── use_cases.md
│   ├── design/
│   │   ├── database_design.md
│   │   ├── system_architecture.md
│   │   ├── ui_mockups.md
│   │   └── api_endpoints.md
│   ├── testing/
│   │   ├── test_plan.md
│   │   ├── unit_test_results.md
│   │   ├── integration_test_results.md
│   │   └── acceptance_test_results.md
│   └── presentations/
│       ├── IT483_Defense_Presentation.pptx
│       └── IT484_Defense_Presentation.pptx
│
├── src/                           # Source code
│   ├── frontend/                  # React.js web application
│   │   ├── public/
│   │   │   ├── index.html
│   │   │   └── favicon.ico
│   │   ├── src/
│   │   │   ├── components/        # Reusable React components
│   │   │   │   ├── Dashboard.js
│   │   │   │   ├── InventoryTable.js
│   │   │   │   ├── SupplierForm.js
│   │   │   │   ├── PurchaseOrderForm.js
│   │   │   │   ├── ReportGenerator.js
│   │   │   │   └── Navigation.js
│   │   │   ├── pages/             # Page components
│   │   │   │   ├── HomePage.js
│   │   │   │   ├── InventoryPage.js
│   │   │   │   ├── SupplierPage.js
│   │   │   │   ├── PurchaseOrderPage.js
│   │   │   │   ├── ReportsPage.js
│   │   │   │   └── UserManagementPage.js
│   │   │   ├── services/          # API client services
│   │   │   │   ├── api.js
│   │   │   │   ├── inventoryService.js
│   │   │   │   ├── supplierService.js
│   │   │   │   └── authService.js
│   │   │   ├── styles/            # CSS files
│   │   │   │   ├── App.css
│   │   │   │   ├── components.css
│   │   │   │   └── responsive.css
│   │   │   ├── App.js             # Main React app
│   │   │   ├── index.js           # Entry point
│   │   │   └── config.js          # Configuration
│   │   ├── package.json
│   │   └── .env.example
│   │
│   ├── backend/                   # Node.js/Express API server
│   │   ├── routes/                # API route handlers
│   │   │   ├── auth.js            # Authentication routes
│   │   │   ├── inventory.js       # Inventory CRUD routes
│   │   │   ├── suppliers.js       # Supplier CRUD routes
│   │   │   ├── purchase_orders.js # Purchase order routes
│   │   │   ├── users.js           # User management routes
│   │   │   └── reports.js         # Report generation routes
│   │   ├── controllers/           # Business logic
│   │   │   ├── authController.js
│   │   │   ├── inventoryController.js
│   │   │   ├── supplierController.js
│   │   │   ├── purchaseOrderController.js
│   │   │   ├── userController.js
│   │   │   └── reportController.js
│   │   ├── models/                # Database models
│   │   │   ├── InventoryItem.js
│   │   │   ├── Supplier.js
│   │   │   ├── PurchaseOrder.js
│   │   │   ├── User.js
│   │   │   ├── Division.js
│   │   │   └── ActivityLog.js
│   │   ├── middleware/            # Express middleware
│   │   │   ├── auth.js            # Authentication middleware
│   │   │   ├── errorHandler.js
│   │   │   └── validation.js
│   │   ├── config/                # Configuration files
│   │   │   ├── database.js        # Database connection
│   │   │   ├── environment.js     # Environment variables
│   │   │   └── constants.js       # Application constants
│   │   ├── utils/                 # Utility functions
│   │   │   ├── logger.js
│   │   │   ├── validators.js
│   │   │   └── helpers.js
│   │   ├── server.js              # Main server entry point
│   │   ├── package.json
│   │   └── .env.example
│   │
│   └── database/                  # Database setup and migrations
│       ├── schema.sql             # Complete database schema
│       ├── migrations/
│       │   ├──001_initial_schema.sql
│       │   ├── 002_add_audit_logging.sql
│       │   └── 003_add_indexes.sql
│       ├── seeders/               # Sample data for testing
│       │   ├── divisions.sql
│       │   ├── suppliers.sql
│       │   ├── inventory_items.sql
│       │   └── users.sql
│       └── backup/                # Database backups
│           └── .gitkeep
│
├── tests/                         # Test suites
│   ├── unit/                      # Unit tests
│   │   ├── inventory.test.js
│   │   ├── supplier.test.js
│   │   ├── purchaseOrder.test.js
│   │   └── auth.test.js
│   ├── integration/               # Integration tests
│   │   ├── api.test.js
│   │   ├── database.test.js
│   │   └── workflows.test.js
│   ├── system/                    # System/E2E tests
│   │   ├── inventory_workflow.test.js
│   │   ├── purchase_workflow.test.js
│   │   └── reporting.test.js
│   └── acceptance/                # Acceptance tests
│       ├── user_scenarios.md
│       └── test_results.md
│
├── deployment/                    # Deployment and operations
│   ├── docker/
│   │   ├── Dockerfile
│   │   ├── docker-compose.yml
│   │   └── .dockerignore
│   ├── nginx/                     # Web server configuration
│   │   └── nginx.conf
│   ├── backup/
│   │   ├── backup_script.sh
│   │   └── restore_script.sh
│   ├── installation/
│   │   ├── INSTALL.md             # Installation instructions
│   │   ├── setup_database.md
│   │   └── initial_configuration.md
│   └── operations/
│       ├── OPERATIONS_MANUAL.md   # How to operate the system
│       ├── troubleshooting.md
│       └── maintenance.md
│
├── documentation/                 # User and technical documentation
│   ├── USER_MANUAL.md             # End-user documentation
│   ├── ADMIN_GUIDE.md             # Administrator guide
│   ├── API_DOCUMENTATION.md       # API reference
│   ├── DEVELOPER_GUIDE.md         # For future developers
│   └── FAQ.md                     # Frequently asked questions
│
├── .gitignore
├── .env.example
├── README.md
├── PROJECT_STRUCTURE.md            # This file
└── CHANGELOG.md                    # Version history

```

## File Descriptions

### Documentation (docs/)
- **Proposals & Reports:** All required university documents
- **Requirements:** Detailed functional and non-functional requirements
- **Design:** Architecture, database design, UI mockups, API specs
- **Testing:** Test plans and results for each phase
- **Presentations:** PowerPoint presentations for IT483 and IT484 defenses

### Source Code (src/)

#### Frontend (React.js)
- **components/**: Reusable UI components (tables, forms, alerts)
- **pages/**: Full page components for each feature area
- **services/**: API client services for backend communication
- **styles/**: CSS and responsive design files

#### Backend (Node.js/Express)
- **routes/**: HTTP route definitions and request handlers
- **controllers/**: Business logic separated from routes
- **models/**: Database interaction layer (using ORM)
- **middleware/**: Authentication, validation, error handling
- **config/**: Environment-specific and global configuration
- **utils/**: Reusable helper functions and utilities

#### Database (MySQL)
- **schema.sql**: Complete database design with all tables
- **migrations/**: Version-controlled schema changes
- **seeders/**: Sample data for testing and development
- **backup/**: Automated and manual database backups

### Tests (tests/)
- **unit/**: Individual component tests
- **integration/**: Tests across multiple components
- **system/**: End-to-end workflow tests
- **acceptance/**: Tests validated by stakeholders

### Deployment & Operations (deployment/)
- **docker/**: Containerization for easy deployment
- **nginx/**: Web server reverse proxy configuration
- **backup/**: Database backup and recovery scripts
- **installation/**: Step-by-step installation guide
- **operations/**: How to run and maintain the system

### Documentation (documentation/)
- **USER_MANUAL.md**: Instructions for end-users
- **ADMIN_GUIDE.md**: Administrator operations guide
- **API_DOCUMENTATION.md**: Complete API reference
- **DEVELOPER_GUIDE.md**: For future development and maintenance

## Development Phases

### Phase 1: IT483 (Weeks 5-15)
- Requirements analysis and finalization
- Database design and schema creation
- System architecture and API design
- Frontend UI/UX design and prototyping
- Core inventory module implementation
- Initial testing setup

### Phase 2: IT484 (Weeks 20-32)
- Complete purchase order and supplier modules
- Advanced reporting and analytics
- Comprehensive testing (unit, integration, system)
- Acceptance testing with client
- Documentation completion
- Deployment preparation

## Key Features by Directory

| Feature | Location |
|---------|----------|
| Inventory tracking | src/backend/controllers/inventoryController.js |
| Low-stock alerts | src/backend/models/InventoryItem.js |
| Purchase orders | src/backend/controllers/purchaseOrderController.js |
| Supplier management | src/backend/controllers/supplierController.js |
| User authentication | src/backend/middleware/auth.js |
| Reports generation | src/backend/controllers/reportController.js |
| Dashboard UI | src/frontend/pages/HomePage.js |
| Inventory UI | src/frontend/pages/InventoryPage.js |
| Database schema | src/database/schema.sql |

## Getting Started

1. **Review proposal:** `docs/Senior_Project_Proposal_Draft.md`
2. **Set up development environment:** See `deployment/installation/INSTALL.md`
3. **Review requirements:** `docs/requirements/functional_requirements.md`
4. **Study database design:** `src/database/schema.sql`
5. **Run tests:** `npm test` in respective frontend/backend directories

---

*Last Updated: May 2026*  
*Project Status: Proposal Phase (Week 1-4)*