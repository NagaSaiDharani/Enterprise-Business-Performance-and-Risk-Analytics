## Data Model Design

The project follows a star-schema-inspired model where possible.

### Fact Tables
- fact_sales
- fact_operations
- fact_complaints
- fact_targets

### Dimension Tables
- dim_customer
- dim_product
- dim_date (created in Power BI)
- dim_region (created in Power BI)

### Modeling Decisions
- Sales acts as the central analytical fact table
- Operations and complaints are analyzed via DAX using TREATAS where direct relationships were not feasible
- Ambiguous many-to-many relationships were intentionally avoided
- The model prioritizes correctness and performance over forced joins

This design reflects real-world BI constraints and trade-offs.
