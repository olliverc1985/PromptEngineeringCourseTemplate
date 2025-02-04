# Session 3: Advanced Prompt Techniques Examples

## Standard Format Guidelines
```
Each example in this course follows this structure:

1. Context
   - Background information
   - Prerequisites (Sessions 1-2 completion)
   - Target audience (Advanced business users)

2. Example Structure
   - Test data
   - Basic version
   - Enhanced version
   - Why it works better

3. Practice Format
   - Test scenarios
   - Basic approach
   - Enhanced approach
   - Solution guidelines

4. Validation Criteria
   - Success metrics
   - Common pitfalls
   - Testing approach
   - Quality checklist

5. Documentation Requirements
   - Implementation notes
   - Technical considerations
   - Error handling
   - Performance optimisation
```

## Review Checkpoints
At the end of each section, verify:
1. Understanding
   □ Complex query handling mastered
   □ Chain of thought implemented
   □ Self-reflection mechanisms used
   □ Error handling understood

2. Implementation
   □ Query decomposition tested
   □ Validation steps implemented
   □ Error handling robust
   □ Performance optimised

3. Documentation
   □ Process flows documented
   □ Error scenarios recorded
   □ Improvements tracked
   □ Updates logged

## Prerequisites
- Completion of Sessions 1-2
- Understanding of tone manipulation
- Experience with basic prompting
- Familiarity with business scenarios

## 1. Complex Query Handling

### Example 1: Market Analysis Report
```
Test Data:
market_analysis.json:
{
  "industry": "Electric Vehicles",
  "region": "United Kingdom",
  "market_data": {
    "current_market_size": "£15.2B",
    "growth_rate": "34.2% YoY",
    "key_players": [
      {
        "name": "Tesla",
        "market_share": "28%",
        "growth": "+5.2%"
      },
      {
        "name": "VW Group",
        "market_share": "15%",
        "growth": "+3.8%"
      },
      {
        "name": "BMW Group",
        "market_share": "12%",
        "growth": "+2.9%"
      }
    ],
    "consumer_trends": [
      {
        "trend": "Environmental Consciousness",
        "impact_score": 8.5,
        "growth_indicator": "Rising"
      },
      {
        "trend": "Government Incentives",
        "impact_score": 7.8,
        "growth_indicator": "Stable"
      },
      {
        "trend": "Charging Infrastructure",
        "impact_score": 6.9,
        "growth_indicator": "Improving"
      }
    ],
    "regulatory_environment": {
      "current_policies": [
        "2030 ICE Ban",
        "Clean Air Zones",
        "EV Grants"
      ],
      "upcoming_changes": [
        "Enhanced Tax Benefits",
        "Charging Network Expansion",
        "Manufacturing Incentives"
      ]
    }
  }
}

Basic Prompt:
"Analyse the UK electric vehicle market."

Enhanced Prompt:
"Conduct a comprehensive analysis of the UK electric vehicle market using the provided data:

1. Market Overview
   - Calculate total market value and growth trajectory
   - Analyse market share distribution
   - Identify key growth drivers

2. Competitive Analysis
   - Compare player performance metrics
   - Evaluate market share changes
   - Assess competitive advantages

3. Consumer Behaviour
   - Rank consumer trends by impact
   - Correlate trends with market growth
   - Project future behaviour patterns

4. Regulatory Impact
   - Assess policy effectiveness
   - Quantify incentive impacts
   - Forecast regulatory influence

Output Format:
1. Executive Summary (2-3 paragraphs)
2. Market Metrics Dashboard
3. Competitive Landscape Analysis
4. Consumer Trends Analysis
5. Regulatory Impact Assessment
6. Strategic Recommendations

Include:
- Data visualisation suggestions
- Confidence levels for projections
- Risk factors and mitigation strategies
- Market opportunity sizing"

Why it works better: Provides structured analysis framework with specific metrics and outputs.
```

### Example 2: Process Automation Analysis
```
Test Data:
customer_service_data.json:
{
  "department": "Customer Service",
  "current_metrics": {
    "daily_queries": 1200,
    "average_response_time": "4.5 hours",
    "resolution_rate": "85%",
    "customer_satisfaction": "3.8/5",
    "staff_count": 45,
    "cost_per_query": "£8.50"
  },
  "query_types": [
    {
      "category": "Order Status",
      "volume": "35%",
      "automation_potential": "High",
      "complexity": "Low",
      "current_handling": "Manual"
    },
    {
      "category": "Returns",
      "volume": "25%",
      "automation_potential": "Medium",
      "complexity": "Medium",
      "current_handling": "Semi-Automated"
    },
    {
      "category": "Technical Support",
      "volume": "20%",
      "automation_potential": "Low",
      "complexity": "High",
      "current_handling": "Manual"
    },
    {
      "category": "Account Issues",
      "volume": "15%",
      "automation_potential": "Medium",
      "complexity": "Medium",
      "current_handling": "Manual"
    },
    {
      "category": "Product Information",
      "volume": "5%",
      "automation_potential": "High",
      "complexity": "Low",
      "current_handling": "Manual"
    }
  ],
  "automation_tools": {
    "chatbot": {
      "setup_cost": "£50,000",
      "monthly_cost": "£2,500",
      "expected_coverage": "40%"
    },
    "email_automation": {
      "setup_cost": "£30,000",
      "monthly_cost": "£1,500",
      "expected_coverage": "25%"
    },
    "self_service_portal": {
      "setup_cost": "£75,000",
      "monthly_cost": "£3,000",
      "expected_coverage": "35%"
    }
  }
}

Basic Prompt:
"Suggest how to automate our customer service."

Enhanced Prompt:
"Develop a detailed customer service automation strategy using the provided data:

1. Current State Analysis
   - Calculate current operational costs
   - Identify efficiency bottlenecks
   - Map query types to resolution paths
   - Assess staff utilisation

2. Automation Opportunity Assessment
   - Rank processes by automation potential
   - Calculate ROI for each automation tool
   - Project impact on metrics
   - Identify risk factors

3. Implementation Strategy
   - Prioritise automation targets
   - Create phased rollout plan
   - Define success metrics
   - Design staff transition plan

Required Outputs:
1. Current State Assessment
   - Cost analysis
   - Efficiency metrics
   - Process bottlenecks
   - Staff impact

2. Automation Recommendations
   - Tool selection rationale
   - Coverage projections
   - Cost-benefit analysis
   - Risk assessment

3. Implementation Roadmap
   - Timeline
   - Resource requirements
   - Training needs
   - Success metrics

4. Financial Projections
   - Implementation costs
   - Expected savings
   - ROI timeline
   - Budget requirements"

Why it works better: Provides comprehensive analysis framework with clear financial and operational metrics.
```

### Example 3: Error Handling and Validation
```
Test Data:
order_data.json:
{
  "order": {
    "id": "ORD-2024-1234",
    "customer": {
      "name": "James Smith",
      "email": "j.smith@email",
      "address": {
        "line1": "42 High Street",
        "city": "Manchester",
        "county": "Greater Manchester"
      }
    },
    "items": [
      {
        "sku": "PROD-001",
        "quantity": 50,
        "price": 29.99,
        "stock_level": 30
      }
    ],
    "payment": {
      "method": "credit_card",
      "card_number": "XXXX-XXXX-XXXX-1234",
      "expiry": "01/24"
    },
    "delivery": {
      "method": "Standard",
      "instructions": ""
    }
  }
}

Basic Prompt:
"Check this order for errors."

Enhanced Prompt:
"Perform comprehensive order validation and generate appropriate responses:

1. Data Validation Checks
   - Required Fields Present
   - Format Validation
   - Business Rule Compliance
   - Stock Availability

2. Error Categorisation
   - Critical (Blocking)
   - Warning (Non-blocking)
   - Information (Advisory)
   - Suggestions

3. Response Generation
   - User-Friendly Messages
   - Correction Guidelines
   - Alternative Suggestions
   - Next Steps

Output Requirements:
1. Validation Summary
   - Overall status
   - Error count by category
   - Correction priority

2. Detailed Error Report
   - Field-level issues
   - Validation rule failed
   - Impact level
   - Resolution steps

3. User Communication
   - Clear error messages
   - Specific correction steps
   - Alternative options
   - Support contact details

4. System Actions
   - Hold/Release decisions
   - Notification triggers
   - Audit trail entries
   - Recovery procedures"

Why it works better: Provides structured error handling with clear user communication and system actions.
```

## Practice Exercises

### Exercise 1: Multi-Step Problem Solving
```
Test Data:
product_launch.json:
{
  "product": {
    "name": "EcoSmart Home Hub",
    "category": "Smart Home",
    "target_market": "UK Homeowners",
    "price_point": "£249.99",
    "features": [
      "Energy monitoring",
      "Smart device integration",
      "AI-powered automation",
      "Mobile app control"
    ],
    "competitors": [
      {
        "name": "SmartHome Pro",
        "price": "£299.99",
        "market_share": "35%"
      },
      {
        "name": "HomeControl+",
        "price": "£199.99",
        "market_share": "25%"
      }
    ],
    "market_research": {
      "total_market_size": "£1.2B",
      "growth_rate": "18%",
      "customer_pain_points": [
        "High energy bills",
        "Complex setup",
        "Limited integration"
      ]
    }
  }
}

Basic Prompt:
"Create a product launch strategy."

Enhanced Prompt:
"Develop a comprehensive product launch strategy using the provided data:

1. Market Analysis Phase
   - Market size calculation
   - Competitor positioning
   - Target audience definition
   - Value proposition development

2. Strategy Development Phase
   - Pricing strategy
   - Distribution channels
   - Marketing messages
   - Launch timeline

3. Implementation Planning Phase
   - Resource allocation
   - Marketing activities
   - Sales targets
   - Success metrics

Required Deliverables:
1. Market Analysis Report
2. Launch Strategy Document
3. Implementation Timeline
4. Budget Allocation
5. Risk Assessment
6. Success Metrics Dashboard"
```

## Tips for Advanced Prompting
- Use structured data inputs
- Implement validation checks
- Include error handling
- Provide clear metrics
- Document assumptions

## Common Advanced Mistakes to Avoid
- Overlooking data validation
- Insufficient error handling
- Unclear success metrics
- Missing documentation
- Incomplete test scenarios