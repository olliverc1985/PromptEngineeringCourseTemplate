# Session 5: Multi-step Reasoning and Self-Correction Examples

## Standard Format Guidelines
```
Each example in this course follows this structure:

1. Context
   - Background information
   - Prerequisites (Sessions 1-4 completion)
   - Target audience (Advanced problem solvers)

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
   - Reasoning methodology
   - Validation steps
   - Improvement cycles
```

## Review Checkpoints
At the end of each section, verify:
1. Understanding
   □ Multi-step reasoning mastered
   □ Self-correction implemented
   □ Strategic thinking demonstrated
   □ Complex problems decomposed

2. Implementation
   □ Reasoning steps documented
   □ Validation methods applied
   □ Solutions optimised
   □ Improvements tracked

3. Documentation
   □ Methodology documented
   □ Decision points recorded
   □ Improvements logged
   □ Updates tracked

## Prerequisites
- Completion of Sessions 1-4
- Advanced problem-solving skills
- Experience with complex scenarios
- Understanding of validation methods

## 1. Strategic Reasoning Examples

### Example 1: Market Expansion Analysis
```
Test Data:
market_expansion.json:
{
  "company": {
    "name": "TechRetail Plus",
    "sector": "E-commerce",
    "current_markets": {
      "primary": {
        "region": "London & South East",
        "revenue": "£45M",
        "market_share": "12%",
        "growth_rate": "15%",
        "customer_base": 125000
      },
      "secondary": {
        "region": "Manchester & North West",
        "revenue": "£15M",
        "market_share": "5%",
        "growth_rate": "25%",
        "customer_base": 42000
      }
    },
    "financials": {
      "annual_revenue": "£60M",
      "profit_margin": "18%",
      "cash_reserves": "£8M",
      "investment_budget": "£5M"
    },
    "capabilities": {
      "logistics_centres": 2,
      "delivery_fleet": 45,
      "tech_platform": "Custom E-commerce",
      "staff": 180
    }
  },
  "target_markets": [
    {
      "region": "Birmingham & Midlands",
      "market_size": "£850M",
      "growth_rate": "12%",
      "competition": {
        "major_players": 3,
        "market_leader_share": "28%",
        "barriers_to_entry": "Medium"
      },
      "demographics": {
        "population": 5200000,
        "average_income": "£32,000",
        "e_commerce_adoption": "72%"
      },
      "infrastructure": {
        "logistics_cost": "£2.5M",
        "setup_time": "6 months",
        "regulatory_requirements": "Standard UK"
      }
    },
    {
      "region": "Scotland",
      "market_size": "£720M",
      "growth_rate": "14%",
      "competition": {
        "major_players": 2,
        "market_leader_share": "35%",
        "barriers_to_entry": "High"
      },
      "demographics": {
        "population": 4500000,
        "average_income": "£31,000",
        "e_commerce_adoption": "68%"
      },
      "infrastructure": {
        "logistics_cost": "£3.2M",
        "setup_time": "8 months",
        "regulatory_requirements": "Scotland-specific"
      }
    }
  ]
}

Basic Prompt:
"Analyse which market we should expand into."

Enhanced Prompt:
"Develop a comprehensive market expansion analysis using the provided data:

1. Current Position Assessment
   - Market share analysis
   - Financial capability review
   - Operational capacity evaluation
   - Core competencies identification

2. Target Market Analysis
   - Market size comparison
   - Growth potential assessment
   - Competition analysis
   - Entry barrier evaluation

3. Resource Requirements
   - Infrastructure needs
   - Financial investment
   - Timeline estimation
   - Staffing requirements

4. Risk Assessment
   - Market risks
   - Operational risks
   - Financial risks
   - Regulatory risks

5. ROI Projection
   - Revenue potential
   - Cost structure
   - Break-even analysis
   - Growth trajectory

Required Outputs:
1. Market Comparison Matrix
2. Resource Requirement Plan
3. Risk Assessment Dashboard
4. Financial Projections
5. Implementation Timeline
6. Go/No-Go Recommendation

Decision Criteria:
- Market potential vs. Investment required
- Operational feasibility
- Risk level
- Expected ROI
- Strategic fit"

Why it works better: Provides structured analysis framework with clear decision criteria and measurable outcomes.
```

### Example 2: Technical Problem Resolution
```
Test Data:
system_issue.json:
{
  "incident": {
    "id": "INC-2024-1234",
    "type": "Performance Degradation",
    "status": "Critical",
    "duration": "72 hours",
    "impact": {
      "users_affected": 15000,
      "revenue_loss": "£25,000/hour",
      "services_impacted": [
        "Checkout Process",
        "Order Management",
        "Inventory Updates"
      ]
    }
  },
  "system_metrics": {
    "response_times": {
      "checkout": {
        "normal": "0.8s",
        "current": "4.5s",
        "threshold": "2.0s"
      },
      "order_processing": {
        "normal": "1.2s",
        "current": "6.8s",
        "threshold": "3.0s"
      }
    },
    "error_rates": {
      "api_failures": "12%",
      "database_timeouts": "8%",
      "payment_declines": "15%"
    },
    "resource_utilization": {
      "cpu": "92%",
      "memory": "87%",
      "disk_io": "95%",
      "network": "65%"
    }
  },
  "recent_changes": [
    {
      "type": "Deployment",
      "component": "Payment Gateway",
      "date": "2024-01-15",
      "details": "Version 2.5.0 upgrade"
    },
    {
      "type": "Database",
      "component": "Order Management",
      "date": "2024-01-14",
      "details": "Schema optimization"
    },
    {
      "type": "Infrastructure",
      "component": "Load Balancer",
      "date": "2024-01-13",
      "details": "Configuration update"
    }
  ],
  "monitoring_data": {
    "logs": [
      {
        "timestamp": "2024-01-15T10:00:00Z",
        "component": "Payment Gateway",
        "message": "Connection pool exhausted"
      },
      {
        "timestamp": "2024-01-15T10:01:00Z",
        "component": "Database",
        "message": "Deadlock detected"
      }
    ],
    "alerts": [
      {
        "type": "High CPU Usage",
        "frequency": "Every 5 minutes",
        "duration": "48 hours"
      },
      {
        "type": "Database Connections",
        "frequency": "Every 2 minutes",
        "duration": "72 hours"
      }
    ]
  }
}

Basic Prompt:
"Fix the system performance issue."

Enhanced Prompt:
"Analyse and resolve the critical system performance degradation using the provided data:

1. Impact Assessment
   - Calculate business impact
   - Identify affected systems
   - Quantify user impact
   - Determine priority level

2. Root Cause Analysis
   - Analyse system metrics
   - Review recent changes
   - Examine error patterns
   - Correlate events

3. Solution Development
   - Identify potential fixes
   - Evaluate solution impact
   - Consider dependencies
   - Assess implementation risks

4. Implementation Plan
   - Define resolution steps
   - Create timeline
   - Identify resources needed
   - Plan verification tests

5. Prevention Strategy
   - Identify systemic issues
   - Recommend improvements
   - Define monitoring needs
   - Update procedures

Required Deliverables:
1. Incident Analysis Report
2. Root Cause Findings
3. Solution Recommendation
4. Implementation Plan
5. Verification Steps
6. Future Prevention Measures

Success Criteria:
- Response times within thresholds
- Error rates below 1%
- Resource utilization under 70%
- No recurring incidents"

Why it works better: Provides structured problem-solving approach with clear metrics and success criteria.
```

### Example 3: Decision Analysis
```
Test Data:
product_decision.json:
{
  "product": {
    "name": "Smart Home Hub Pro",
    "status": "Development Complete",
    "investment": "£2.5M",
    "target_launch": "Q2 2024",
    "features": [
      {
        "name": "Energy Management",
        "development_cost": "£800,000",
        "market_demand": "High",
        "competitor_parity": true
      },
      {
        "name": "AI Assistant",
        "development_cost": "£1,200,000",
        "market_demand": "Medium",
        "competitor_parity": false
      },
      {
        "name": "Security Suite",
        "development_cost": "£500,000",
        "market_demand": "High",
        "competitor_parity": true
      }
    ]
  },
  "market_research": {
    "total_addressable_market": "£1.2B",
    "growth_rate": "18%",
    "customer_survey": {
      "sample_size": 1500,
      "price_sensitivity": {
        "optimal_price": "£299",
        "price_ceiling": "£399",
        "price_floor": "£199"
      },
      "feature_importance": {
        "energy_management": "85%",
        "ai_assistant": "65%",
        "security": "90%"
      }
    },
    "competitor_analysis": [
      {
        "name": "SmartLife Hub",
        "market_share": "35%",
        "price": "£349",
        "rating": "4.2/5"
      },
      {
        "name": "HomeIQ",
        "market_share": "25%",
        "price": "£299",
        "rating": "3.8/5"
      }
    ]
  },
  "launch_scenarios": [
    {
      "type": "Full Launch",
      "cost": "£1.5M",
      "timeline": "3 months",
      "risk_level": "High"
    },
    {
      "type": "Phased Launch",
      "cost": "£900,000",
      "timeline": "6 months",
      "risk_level": "Medium"
    },
    {
      "type": "Soft Launch",
      "cost": "£500,000",
      "timeline": "2 months",
      "risk_level": "Low"
    }
  ]
}

Basic Prompt:
"Decide how to launch the product."

Enhanced Prompt:
"Develop a comprehensive product launch decision analysis using the provided data:

1. Market Opportunity Assessment
   - Market size analysis
   - Growth potential
   - Competition mapping
   - Customer demand validation

2. Product Readiness Evaluation
   - Feature completeness
   - Competitive advantage
   - Technical stability
   - Support readiness

3. Launch Strategy Analysis
   - Scenario comparison
   - Resource requirements
   - Timeline feasibility
   - Risk assessment

4. Financial Modelling
   - Cost-benefit analysis
   - ROI projections
   - Break-even analysis
   - Cash flow impact

5. Risk Mitigation Planning
   - Technical risks
   - Market risks
   - Operational risks
   - Competitive risks

Required Outputs:
1. Strategy Recommendation
2. Implementation Plan
3. Risk Management Plan
4. Success Metrics
5. Contingency Plans

Decision Framework:
- Market timing
- Resource availability
- Risk tolerance
- Revenue potential
- Strategic alignment"

Why it works better: Provides structured decision-making framework with clear evaluation criteria and risk assessment.
```

## Practice Exercises

### Exercise 1: Business Process Optimization
```
Test Data:
process_analysis.json:
{
  "process": {
    "name": "Customer Support Workflow",
    "current_metrics": {
      "average_resolution_time": "4.5 hours",
      "first_response_time": "45 minutes",
      "customer_satisfaction": "3.8/5",
      "resolution_rate": "85%",
      "escalation_rate": "15%"
    },
    "bottlenecks": [
      {
        "stage": "Initial Triage",
        "delay": "25 minutes",
        "cause": "Manual Classification"
      },
      {
        "stage": "Specialist Assignment",
        "delay": "35 minutes",
        "cause": "Resource Availability"
      }
    ],
    "resources": {
      "staff": 45,
      "tools": [
        "Ticketing System",
        "Knowledge Base",
        "Chat Support"
      ],
      "cost_per_ticket": "£12.50"
    }
  }
}

Basic Prompt:
"Improve the customer support process."

Enhanced Prompt:
"Analyse and optimize the customer support workflow:

1. Process Analysis
   - Performance metrics review
   - Bottleneck identification
   - Resource utilization
   - Cost analysis

2. Improvement Opportunities
   - Automation potential
   - Resource optimization
   - Workflow streamlining
   - Technology enhancement

3. Solution Design
   - Process modifications
   - Technology solutions
   - Resource allocation
   - Implementation approach

Required Deliverables:
1. Current State Analysis
2. Improvement Recommendations
3. Implementation Plan
4. ROI Projection
5. Success Metrics"
```

## Tips for Reasoning
- Use structured analysis
- Document assumptions
- Consider alternatives
- Validate conclusions
- Plan for contingencies

## Common Reasoning Mistakes
- Incomplete analysis
- Biased assumptions
- Missing data points
- Poor validation
- Unclear criteria 