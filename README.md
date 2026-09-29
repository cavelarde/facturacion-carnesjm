# facturacion-carnesjm
# 🥩 Carnes JM - Point of Sale (POS) & Cash Reconciliation System

A high-efficiency, lightweight Point of Sale (POS) terminal and cash reconciliation system custom-built for retail operations and meat distribution centers. This application optimizes real-time transaction processing, dynamic expense tracking, and end-of-day financial balance calculations.

🚀 **Live Demo:** [View Application in Action](https://github.io)

---

## 🛠️ Tech Stack & Architecture

- **Frontend Core:** Semantic HTML5, Modular Dashboard Layout.
- **Styling Architecture:** Modern CSS3 featuring dynamic UI state components and specialized `@media print` hardware stylesheets.
- **Icons & Typography:** Plus Jakarta Sans & Lucide Icons integration.
- **Logic Engine:** Vanilla JavaScript (ES6+) utilizing synchronous state arrays for inventory tracking and financial data stream processing.

---

## ✨ Core Features & Technical Engineering

### 1. Dual-Input Transaction Engine (Barcode & Manual Parsing)
The checkout module supports dual-input processing for modern retail workflows:
- **Hardware Scanner Ready:** Asynchronous listeners optimized for rapid barcode inputs.
- **Manual Overrides:** Structural forms enabling cashiers to instantly parse product quantities, weights, and unit values directly into the active sales ledger.

### 2. Dual-Panel POS Dashboard Design
Architected with a split-screen design system that mirrors corporate touch-screen checkout terminals:
- **Left Control Panel:** Drives administrative operations, cash drawer auditing, expense logs, and inventory state toggles.
- **Right Ticket Panel:** Acts as a real-time virtual receipt, re-rendering active line items, itemized sub-totals, and final checkout calculations dynamically.

### 3. Automated End-of-Day Cash Reconciliation (Cuadre de Caja)
Features an automated financial accounting engine that computes the store's daily performance:
- **Multi-Channel Revenue Segregation:** Segregates incoming cash flows into Cash (Efectivo), Bank Transfer (Transferencia), and Store Credit (Crédito).
- **Expense Sinking Fund:** Tracks immediate daily payouts across multiple categories (Suppliers, Employees, Operational Expenses).
- **Net Balance Calculation:** Executes algorithmic computations (`Total Revenue - Total Expenses = Net Balance`), triggering reactive UI color warnings (Green/Red) to alert management of financial deficits or surpluses in real-time.

### 4. Hardware Thermal Print Formatter
Embedded with a production-ready hardware printing utility. The active stylesheet includes a specialized print media query that automatically strips away the administrative dashboard, transaction buttons, and entry logs during browser print execution. This forces the DOM to compile a clean, perfectly aligned 80mm standard thermal POS ticket.

---

## 🗂️ Project Structure

```text
├── index.html          # POS Core Terminal layout & UI structure
├── css/
│   └── styles.css      # Design tokens, grid structures, and thermal print queries
├── js/
│   └── script.js       # Financial calculations, inventory states, and DOM mutations
└── README.md           # Technical architecture documentation
```

---

## ⚙️ Local Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   ```
2. **Launch locally:**
   Open the `index.html` file in any modern web browser or run it through a development server (e.g., Live Server in VS Code).

3. **Data Persistency Note:**
   This terminal is architected using localized application states, making it highly portable and ready to be integrated into centralized cloud APIs or local relational databases (SQLite/IndexedDB).
