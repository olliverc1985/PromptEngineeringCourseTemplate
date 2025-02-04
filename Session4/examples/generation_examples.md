# Session 4: Data and Document Generation Examples

## Standard Format Guidelines
```
Each example in this course follows this structure:

1. Context
   - Background information
   - Prerequisites (Sessions 1-3 completion)
   - Target audience (Technical professionals)

2. Example Structure
   - Basic version
   - Enhanced version
   - Why it works better
   - Implementation notes

3. Practice Format
   - Beginner level task
   - Intermediate level task
   - Advanced level task
   - Solution guidelines

4. Validation Criteria
   - Success metrics
   - Common pitfalls
   - Testing approach
   - Quality checklist

5. Documentation Requirements
   - Implementation notes
   - Technical specifications
   - Security considerations
   - Performance requirements
```

## Review Checkpoints
At the end of each section, verify:
1. Understanding
   □ Document generation principles mastered
   □ Data structure concepts applied
   □ Code generation patterns understood
   □ Quality control implemented

2. Implementation
   □ Generated content validated
   □ Data structures tested
   □ Code quality verified
   □ Performance optimised

3. Documentation
   □ Technical specifications complete
   □ Security measures documented
   □ Performance metrics recorded
   □ Updates tracked

## Prerequisites
- Completion of Sessions 1-3
- Understanding of data structures
- Basic coding knowledge
- Familiarity with documentation standards

## 1. Document Generation

### Example: Technical Documentation Template
```
Context: Software feature documentation
Prerequisites: Understanding of technical writing
Target Audience: Development team and stakeholders

Basic Version:
"Write documentation for a new feature."

Enhanced Version:
Task: Generate a comprehensive technical documentation template
Required Sections:
1. Overview
2. Technical Specifications
3. Implementation Details
4. API Documentation
5. Usage Examples
6. Troubleshooting Guide

Why it works better:
- Structured approach
- Complete coverage
- Clear hierarchy
- Practical examples

Implementation Notes:
- Use consistent formatting
- Include code examples
- Add cross-references
- Maintain version control
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

## 5. Quality Control and Evaluation

### Document Quality Control
```
Task: Implement quality control for generated documents

Checklist:
1. Structure Validation
   □ All required sections present
   □ Correct heading hierarchy
   □ Consistent formatting
   □ Valid cross-references

2. Content Quality
   □ Grammar and spelling
   □ Technical accuracy
   □ Completeness of information
   □ Consistency of terminology

3. Format Compliance
   □ Style guide adherence
   □ Branding requirements
   □ Accessibility standards
   □ Document metadata
```

### XML Generation Example
```
Task: Create a product catalogue in XML

<?xml version="1.0" encoding="UTF-8"?>
<catalogue>
    <category name="Electronics">
        <product id="E001">
            <name>Smart Watch Pro</name>
            <description>Advanced fitness tracking smartwatch</description>
            <specifications>
                <battery>5 days</battery>
                <waterproof>Yes</waterproof>
                <connectivity>Bluetooth 5.0</connectivity>
            </specifications>
            <pricing>
                <retail>199.99</retail>
                <discount>179.99</discount>
            </pricing>
        </product>
    </category>
</catalogue>

Validation Rules:
- Required attributes: id, name
- Valid price format: 2 decimal places
- Non-empty description
- Valid category assignment
```

### XML Schema Validation Example
```
Task: Create XML schema for product catalogue

XML Schema:
<?xml version="1.0" encoding="UTF-8"?>
<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
    <xs:element name="catalogue">
        <xs:complexType>
            <xs:sequence>
                <xs:element name="category" maxOccurs="unbounded">
                    <xs:complexType>
                        <xs:sequence>
                            <xs:element name="product" maxOccurs="unbounded">
                                <xs:complexType>
                                    <xs:sequence>
                                        <xs:element name="name" type="xs:string"/>
                                        <xs:element name="description" type="xs:string"/>
                                        <xs:element name="specifications">
                                            <xs:complexType>
                                                <xs:sequence>
                                                    <xs:element name="battery" type="xs:string"/>
                                                    <xs:element name="waterproof" type="xs:string"/>
                                                    <xs:element name="connectivity" type="xs:string"/>
                                                </xs:sequence>
                                            </xs:complexType>
                                        </xs:element>
                                        <xs:element name="pricing">
                                            <xs:complexType>
                                                <xs:sequence>
                                                    <xs:element name="retail" type="xs:decimal"/>
                                                    <xs:element name="discount" type="xs:decimal"/>
                                                </xs:sequence>
                                            </xs:complexType>
                                        </xs:element>
                                    </xs:sequence>
                                    <xs:attribute name="id" type="xs:string" use="required"/>
                                </xs:complexType>
                            </xs:element>
                        </xs:sequence>
                        <xs:attribute name="name" type="xs:string" use="required"/>
                    </xs:complexType>
                </xs:element>
            </xs:sequence>
        </xs:complexType>
    </xs:element>
</xs:schema>

Validation Rules:
1. Required Elements:
   - Product must have name and description
   - Pricing must include retail and discount
   - All products must have specifications

2. Data Types:
   - Product ID: String (required)
   - Prices: Decimal (positive numbers)
   - Names: String (non-empty)

3. Cardinality:
   - Multiple products per category
   - Multiple categories in catalogue
   - One set of specifications per product
```

### Enhanced HTML/CSS Responsive Design
```
Task: Create a responsive product grid with modern features

HTML Structure:
```html
<div class="product-grid">
    <article class="product-card">
        <div class="product-image">
            <img src="[product-image]" alt="[product-name]" loading="lazy">
            <div class="product-badges">
                <span class="badge badge-sale">Sale</span>
                <span class="badge badge-new">New</span>
            </div>
        </div>
        <div class="product-content">
            <h3 class="product-title">[Product Name]</h3>
            <p class="product-description">[Short description]</p>
            <div class="product-meta">
                <div class="price-container">
                    <span class="original-price">£99.99</span>
                    <span class="sale-price">£79.99</span>
                </div>
                <div class="rating">
                    <span class="stars">★★★★☆</span>
                    <span class="count">(42)</span>
                </div>
            </div>
            <div class="product-actions">
                <button class="btn-primary">Add to Basket</button>
                <button class="btn-secondary">Save for Later</button>
            </div>
        </div>
    </article>
</div>
```

Advanced CSS Styling:
```css
.product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
    padding: 2rem;
}

.product-card {
    background: #ffffff;
    border-radius: 12px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    overflow: hidden;
}

.product-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
}

.product-image {
    position: relative;
    aspect-ratio: 16/9;
    overflow: hidden;
}

.product-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
}

.product-card:hover .product-image img {
    transform: scale(1.05);
}

.product-badges {
    position: absolute;
    top: 1rem;
    left: 1rem;
    display: flex;
    gap: 0.5rem;
}

.badge {
    padding: 0.25rem 0.75rem;
    border-radius: 4px;
    font-size: 0.875rem;
    font-weight: 600;
}

.badge-sale {
    background: #ff4444;
    color: white;
}

.badge-new {
    background: #00c853;
    color: white;
}

/* Responsive Design */
@media (max-width: 768px) {
    .product-grid {
        grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
        gap: 1rem;
        padding: 1rem;
    }
}

@media (max-width: 480px) {
    .product-actions {
        flex-direction: column;
        gap: 0.5rem;
    }
}

/* Dark Mode Support */
@media (prefers-color-scheme: dark) {
    .product-card {
        background: #2a2a2a;
        color: #ffffff;
    }
}

/* Accessibility */
.btn-primary:focus,
.btn-secondary:focus {
    outline: 2px solid #007bff;
    outline-offset: 2px;
}

/* Reduced Motion */
@media (prefers-reduced-motion: reduce) {
    .product-card,
    .product-image img {
        transition: none;
    }
}
```

Features:
1. Responsive Grid Layout
2. Lazy Loading Images
3. Smooth Animations
4. Dark Mode Support
5. Accessibility Features
6. Reduced Motion Support
7. Modern CSS Grid
8. Flexible Component Design

### Solution Evaluation Framework
```
Task: Create evaluation criteria for generated solutions

1. Technical Assessment
   - Code quality metrics
   - Performance benchmarks
   - Security considerations
   - Scalability factors

2. User Experience Evaluation
   - Accessibility compliance
   - Responsive design
   - Load time optimization
   - Interface usability

3. Implementation Feasibility
   - Resource requirements
   - Technical dependencies
   - Maintenance complexity
   - Integration challenges

4. Optimization Opportunities
   - Performance improvements
   - Code efficiency
   - Resource utilization
   - Caching strategies

Example Scoring Matrix:
| Criterion          | Weight | Score (1-5) | Weighted Score |
|-------------------|--------|-------------|----------------|
| Code Quality      | 0.25   | 4           | 1.00          |
| Performance       | 0.20   | 3           | 0.60          |
| Maintainability   | 0.15   | 4           | 0.60          |
| Scalability       | 0.20   | 5           | 1.00          |
| Security          | 0.20   | 4           | 0.80          |
| Total             | 1.00   |             | 4.00          |
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