DATA FLOW

┌─────────┐   ┌──────────── BRONZE ────────────┐   ┌──────────── SILVER ────────────┐   ┌───────── GOLD ─────────┐
│ Sources │   │ crm_sales                      │   │ crm_sales                      │   │ fact_sales             │
│ CRM     │──>│ crm_cust                       │──>│ crm_cust                       │──┐│                        │
│ ERP     │──>│ crm_prod                       │──>│ crm_prod                       │──┼│ dim_customers          │
│         │──>│ erp_cust                       │──>│ erp_cust                       │──┤│                        │
│         │──>│ erp_loc                        │──>│ erp_loc                        │──┼│ dim_products           │
│         │──>│ erp_cat                        │──>│ erp_cat                        │──┘│                        │
└─────────┘   └────────────────────────────────┘   └────────────────────────────────┘   └────────────────────────┘
