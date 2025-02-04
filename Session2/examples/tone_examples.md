# Session 2: Tone and Content Manipulation Examples

## Standard Format Guidelines
```
Each example in this course follows this structure:

1. Context
   - Background information
   - Prerequisites (Session 1 completion)
   - Target audience (Business professionals)

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
   - Communication guidelines
   - Tone considerations
   - Cultural sensitivity
```

## Review Checkpoints
At the end of each section, verify:
1. Understanding
   □ Tone variations mastered
   □ Examples contextually appropriate
   □ Practice exercises completed
   □ Cultural considerations understood

2. Implementation
   □ Tone consistency checked
   □ Cultural sensitivity verified
   □ Department adaptations tested
   □ Communication effective

3. Documentation
   □ Style guides referenced
   □ Tone guidelines documented
   □ Adaptations recorded
   □ Updates tracked

## Prerequisites
- Completion of Session 1
- Understanding of basic prompt structures
- Familiarity with business communication
- Basic knowledge of professional writing

## 1. Tone Variation Examples

### Example 1: Company Policy Change
```
Test Data:
company_policy.json:
{
  "policy_type": "Hybrid Work",
  "effective_date": "2024-03-01",
  "impact": {
    "departments": ["Sales", "Marketing", "IT", "HR"],
    "employees_affected": 250,
    "locations": ["London", "Manchester", "Birmingham"],
    "current_setup": "Full office-based",
    "key_changes": [
      "3 days office / 2 days remote",
      "Core hours 10am-3pm",
      "Team collaboration days",
      "Equipment provision"
    ],
    "business_metrics": {
      "expected_cost_savings": "£500,000/year",
      "productivity_forecast": "+15%",
      "employee_satisfaction_target": "85%"
    }
  }
}

Basic Prompt:
"Write an announcement about changing to hybrid work."

Enhanced Prompt:
"Create three versions of the hybrid work policy announcement using the provided data:

1. Executive Version (Board and C-level):
   - Focus on business impact and ROI
   - Include financial projections
   - Reference industry trends
   - Outline success metrics

2. Management Version (Team Leaders):
   - Implementation timeline
   - Team coordination guidelines
   - Resource allocation
   - Performance monitoring

3. Employee Version (General Staff):
   - Practical day-to-day changes
   - Clear expectations
   - Support resources
   - Next steps

For each version, include:
- Clear policy overview
- Specific dates and deadlines
- Contact points for questions
- Required actions"

Why it works better: Provides tailored messaging for each audience while maintaining consistency in core information.
```

### Example 2: Customer Service Response
```
Test Data:
customer_complaint.json:
{
  "customer": {
    "name": "Sarah Thompson",
    "type": "Premium Member",
    "loyalty_years": 3,
    "purchase_history": {
      "total_orders": 47,
      "average_value": "£125",
      "last_order": "2024-01-15"
    }
  },
  "complaint": {
    "category": "Delivery Delay",
    "product": "Limited Edition Tea Set",
    "order_date": "2024-01-10",
    "expected_delivery": "2024-01-12",
    "actual_delivery": "2024-01-18",
    "special_circumstance": "Birthday Gift",
    "previous_complaints": 0
  }
}

Basic Prompt:
"Write a response to the customer complaint."

Enhanced Prompt:
"Craft a personalised response to our premium customer's delivery delay complaint:

Key Requirements:
1. Acknowledge their loyalty status and history
2. Express genuine understanding of the birthday gift context
3. Explain the delay with transparency
4. Offer specific compensation
5. Provide future assurance

Format:
- Personalised greeting
- Empathetic acknowledgment
- Clear explanation
- Concrete solution
- Goodwill gesture
- Future prevention
- Personal sign-off

Tone Guidelines:
- Professional yet warm
- Genuinely apologetic
- Solution-focused
- Premium service level
- Relationship-building"

Why it works better: Combines empathy with specific actions while acknowledging customer value.
```

### Example 3: Cross-Cultural Communication
```
Test Data:
international_project.json:
{
  "project": {
    "name": "Global E-commerce Platform Launch",
    "teams": {
      "UK": {
        "location": "London",
        "timezone": "GMT",
        "work_style": "Direct communication",
        "team_size": 8
      },
      "Japan": {
        "location": "Tokyo",
        "timezone": "JST (GMT+9)",
        "work_style": "Consensus-based",
        "team_size": 6
      },
      "UAE": {
        "location": "Dubai",
        "timezone": "GST (GMT+4)",
        "work_style": "Relationship-focused",
        "team_size": 4
      }
    },
    "deadlines": {
      "feedback_needed_by": "2024-02-15",
      "launch_date": "2024-03-01"
    }
  }
}

Basic Prompt:
"Request project feedback from international teams."

Enhanced Prompt:
"Create culturally-adapted feedback requests for our international project teams:

Requirements for each version:
1. Appropriate greeting time (timezone-aware)
2. Cultural communication style
3. Proper formality level
4. Clear but culturally sensitive deadlines
5. Acknowledgment of local customs

Format each request with:
- Local time reference
- Cultural acknowledgments
- Clear but adaptable deadlines
- Feedback format options
- Response flexibility
- Appropriate sign-off

Include:
- UK version (direct style)
- Japan version (consensus style)
- UAE version (relationship style)"

Why it works better: Respects cultural nuances while maintaining project requirements.
```

## Practice Exercises

### Exercise 1: Technical Communication
```
Test Data:
system_update.json:
{
  "update": {
    "type": "Security Protocol Implementation",
    "technical_details": {
      "protocol": "OAuth 2.0 + JWT",
      "changes": [
        "Bearer token authentication",
        "Refresh token implementation",
        "2FA requirement"
      ],
      "system_impact": {
        "downtime": "2 hours",
        "affected_services": [
          "API endpoints",
          "Mobile app",
          "Admin dashboard"
        ]
      }
    },
    "user_impact": {
      "login_changes": true,
      "password_reset": required,
      "new_features": ["Single Sign-On", "Remember Me Option"]
    }
  }
}

Basic Prompt:
"Write an announcement about the system update."

Enhanced Prompt:
"Create three versions of the system update announcement:

1. Technical Version (Development Team):
   - Full technical specifications
   - API documentation changes
   - Implementation timeline
   - Testing requirements

2. IT Support Version:
   - Key changes overview
   - User impact summary
   - Troubleshooting guides
   - Support response templates

3. End-User Version:
   - Simple change explanation
   - Required actions
   - Benefits explanation
   - Support contact details

Each version should include:
- Timeline
- Impact assessment
- Required actions
- Support resources"
```

## Tips for Tone Control
- Use specific tone markers
- Consider cultural context
- Maintain consistency
- Adapt to audience expertise
- Balance formality with clarity

## Common Tone Mistakes to Avoid
- Mixing formal and informal language
- Using inappropriate humour
- Over-complicating simple messages
- Ignoring cultural sensitivity
- Being too casual in formal contexts 