# Session 4: Data and Document Generation Examples

## 1. Document Generation

### Example: Technical Documentation Template
```
Task: Generate a technical documentation template for a new software feature.

Required Sections:
1. Overview
2. Technical Specifications
3. Implementation Details
4. API Documentation
5. Usage Examples
6. Troubleshooting Guide

Format Requirements:
- Clear heading hierarchy
- Code block formatting
- Table formatting
- Links to related documentation
- Version control information
```

### Example: Business Report Structure
```
Task: Create a quarterly business report template.

Structure:
1. Executive Summary
2. Financial Highlights
3. Key Performance Indicators
4. Market Analysis
5. Strategic Initiatives
6. Recommendations

Include:
- Data visualisation placeholders
- Table formats for financial data
- Standard chart templates
- Appendix structure
```

## 2. Structured Data Generation

### Example: Excel/CSV Data
```
Task: Generate a sales data structure for Q1 2024

Required Fields:
- Date (DD/MM/YYYY)
- Product ID (PRDXXX)
- Product Name
- Category
- Quantity Sold
- Unit Price
- Total Revenue
- Region
- Sales Representative

Format:
Date,Product_ID,Product_Name,Category,Quantity,Unit_Price,Total_Revenue,Region,Sales_Rep
01/01/2024,PRD001,Widget A,Electronics,10,29.99,299.90,London,John Smith
```

### Example: JSON Structure
```
Task: Create a customer data structure in JSON

{
  "customers": [
    {
      "id": "CUS001",
      "personal_info": {
        "name": "Jane Smith",
        "email": "jane.smith@email.com",
        "phone": "+44 20 1234 5678"
      },
      "address": {
        "street": "123 High Street",
        "city": "Manchester",
        "postcode": "M1 1AA"
      },
      "preferences": {
        "communication": "email",
        "marketing_opt_in": true
      }
    }
  ]
}
```

## 3. Code Generation Examples

### Example: Python Script
```
Task: Generate a data processing script

# Template for data processing script
def process_sales_data(input_file: str, output_file: str) -> dict:
    """
    Process sales data from CSV and generate summary statistics.
    
    Args:
        input_file (str): Path to input CSV file
        output_file (str): Path to output CSV file
    
    Returns:
        dict: Summary statistics
    """
    # Implementation details here
    pass

def generate_report(data: dict) -> None:
    """
    Generate PDF report from processed data.
    
    Args:
        data (dict): Processed data dictionary
    """
    # Implementation details here
    pass

if __name__ == "__main__":
    # Main execution logic
    pass
```

### Example: SQL Query Generation
```
Task: Generate SQL queries for sales analysis

-- Template for sales analysis queries
-- 1. Monthly Sales Summary
SELECT 
    DATE_FORMAT(sale_date, '%Y-%m') as month,
    COUNT(*) as total_transactions,
    SUM(amount) as total_revenue,
    AVG(amount) as average_sale
FROM sales
GROUP BY DATE_FORMAT(sale_date, '%Y-%m')
ORDER BY month DESC;

-- 2. Top Products by Revenue
SELECT 
    p.product_name,
    COUNT(*) as units_sold,
    SUM(s.amount) as total_revenue
FROM sales s
JOIN products p ON s.product_id = p.id
GROUP BY p.product_name
ORDER BY total_revenue DESC
LIMIT 10;
```

## 4. Practice Exercises

### Exercise 1: Document Generation
```
Task: Create a project proposal template

Requirements:
1. Executive Summary section
2. Project Scope section
3. Timeline section
4. Budget section
5. Risk Assessment section
6. Team Structure section

Include prompts for:
- Formatting guidelines
- Section content requirements
- Standard phrases and terminology
- Required data tables
```

### Exercise 2: Data Structure Creation
```
Task: Design a product inventory system

Create structures for:
1. Product catalogue
2. Inventory levels
3. Supplier information
4. Order tracking
5. Price history

Include:
- Field definitions
- Data validation rules
- Relationship mappings
- Sample data entries
```

## Tips for Generation Tasks
- Always specify format requirements
- Include validation criteria
- Define clear structure
- Provide example outputs
- Specify error handling
- Include documentation requirements

## Common Generation Mistakes to Avoid
- Inconsistent formatting
- Missing validation rules
- Incomplete structure definitions
- Ambiguous requirements
- Lack of error handling
- Poor documentation
- Inconsistent naming conventions 