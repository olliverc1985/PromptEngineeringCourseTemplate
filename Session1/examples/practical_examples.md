# Session 1: Practical Examples

## Standard Format Guidelines
```
Each example in this course follows this structure:

1. Context
   - Background information
   - Prerequisites
   - Target audience

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
   - Security considerations
   - Accessibility requirements
   - Performance guidelines
```

## Review Checkpoints
At the end of each section, verify:
1. Understanding
   □ Core concepts clear
   □ Examples relevant
   □ Practice exercises attempted
   □ Solutions understood

2. Implementation
   □ Code tested
   □ Security checked
   □ Accessibility verified
   □ Performance optimised

3. Documentation
   □ Comments clear
   □ Requirements documented
   □ Changes tracked
   □ Updates noted

## 1. What is Prompt Engineering?

### Example 1: Definition and Importance
```
Test Data:
Sample Story for Improvement:
"Once there was a penguin. He was shy. He met a polar bear. They became friends."

Basic Prompt: 
"Write a story"

Enhanced Prompt: 
"Write a 500-word children's story with these specifications:
- Main theme: Friendship and sharing
- Target age: 6-8 years old
- Characters: A shy penguin and an outgoing polar bear
- Setting: Arctic winter
- Must include: A moral lesson about helping others
- Tone: Warm and encouraging
- Format: Include dialogue and descriptive scenes
- Reading level: Simple vocabulary with occasional challenging words"

Why it works better: The enhanced prompt provides specific parameters that guide the AI to create content matching exact requirements.
```

### Example 2: Common Interpretation Patterns
```
Test Data:
Original Business Text:
"Our company sells food delivery services. We have an app. Customers can order food. 
Restaurants can join our platform. We make money from commissions. We want to grow bigger."

Basic Prompt: 
"Make this text better"

Enhanced Prompt:
"Review and improve this business proposal text using:
1. Professional business language
2. Specific target market details
3. Clear value proposition
4. Market size data
5. Revenue streams

Format the output as:
- Executive Summary (2-3 sentences)
- Market Opportunity (2-3 bullet points)
- Value Proposition (1-2 sentences)
- Business Model (2-3 bullet points)
- Target Market (specific demographics)"

Why it works better: The enhanced prompt provides clear improvement criteria and desired output structure.
```

### Example 3: Impact on Output Quality
```
Test Data:
Coffee Shop Details:
- Name: Bean Scene
- Location: Manchester City Centre
- Current Revenue: £15,000/month
- Peak Hours: 8-10am, 12-2pm
- Quiet Periods: 2-5pm
- Staff: 6 part-time, 2 full-time
- Current Marketing: Social media only
- Competition: 5 chain cafes within 500m

Basic Prompt: 
"Give me ideas for my coffee shop"

Enhanced Prompt:
"Suggest 5 actionable marketing strategies for my independent coffee shop with these specific parameters:
- Location: City centre, Manchester
- Monthly marketing budget: £1,000
- Target audience: Young professionals (25-35)
- USP: Speciality coffee and workspace environment
- Current challenges: High competition, need to increase weekday footfall
- Business goals: 20% increase in weekday morning customers

For each strategy, please provide:
1. Implementation steps
2. Estimated costs
3. Expected timeline
4. Success metrics
5. Potential challenges"

Why it works better: The enhanced prompt provides specific context and requirements for more relevant and actionable suggestions.
```

## 2. Command-Based Prompts

### Example 1: Basic Command
```
Test Data:
Team Information:
- Department: Marketing
- Team Size: 8 people
- Names: Sarah (Lead), James, Emma, Michael, Lisa, David, Rachel, Tom
- Available Meeting Rooms: Conference A (capacity 12), Conference B (capacity 8)
- Working Hours: 9am-5pm GMT
- Current Projects: Q1 Review, Q2 Planning, Brand Refresh

Basic Prompt:
"Write a professional email to schedule a team meeting."

Enhanced Prompt:
"Write a professional email to schedule a quarterly planning meeting with these specifications:
- Recipient: Marketing team (8 people)
- Purpose: Q2 2024 campaign planning
- Duration: 2 hours
- Preferred dates: Next Tuesday or Wednesday
- Location: Conference Room A or Zoom
- Pre-meeting requirements: Review Q1 performance metrics
- Attachments needed: Q1 report and agenda
- Tone: Professional but friendly
- Include: Response deadline (24 hours)"
```

## 3. Question-Based Prompts

### Example 1: Simple Question
```
Test Data:
Current Marketing Stats:
Website Visits: 15,000/month
Conversion Rate: 2.3%
Average Order Value: £42
Customer Acquisition Cost: £18
Social Media Followers: 5,200
Email List Size: 3,800
Engagement Rate: 4.1%

Basic Question:
"What are the key components of an effective marketing strategy?"

Enhanced Question:
"Based on our current metrics, what are the top 3 components we should focus on to improve our marketing ROI, considering our £5,000 monthly budget and B2C focus?"
```

## 4. Scenario-Based Prompts

### Example 1: Basic Scenario
```
You are a customer service representative handling a complaint about a delayed delivery. Write a response to the customer.
```

### Example 2: Detailed Scenario
```
You are a customer service representative at an online clothing store. A customer has written a complaint about receiving the wrong size dress for their daughter's wedding, which is in 3 days. The correct size is currently out of stock. Write a response that addresses their concerns and offers solutions.
```

## 5. Context-Setting Prompts

### Example 1: Simple Context
```
Context: You are an HR professional.
Task: Write guidelines for conducting performance reviews.
```

### Example 2: Detailed Context
```
Context: You are an HR professional at a tech startup with 50 employees. The company has never had formal performance reviews before, and the workforce is primarily millennials and Gen Z.
Task: Write guidelines for implementing a new performance review system that focuses on growth and development rather than traditional metrics.
```

## 6. Understanding AI Interpretation

### Example 1: How AI Processes Prompts
```
Poor: Tell me about cats
Better: Describe the key characteristics and behaviours of domestic cats, including their physical features and typical pet care needs.

Why it works better: The second version provides clear parameters and specific aspects to focus on.
```

### Example 2: Common Interpretation Patterns
```
Ambiguous: Make it better
Clear: Improve this text by:
1. Correcting any grammatical errors
2. Enhancing clarity
3. Making the tone more professional
4. Maintaining the original message

Why it works better: The clear version provides specific actions and criteria for improvement.
```

### Example 3: Avoiding Ambiguity
```
Ambiguous: Write something creative about the weather
Clear: Write a 100-word description of a rainy day in London, focusing on:
- The sounds of rain on windows
- The mood of pedestrians
- The effect on city traffic

Why it works better: The clear version specifies length, subject focus, and key elements to include.
```

### Example 4: AI Interpretation Patterns
```
Task: Understanding how AI processes different types of information

1. Pattern Recognition
Poor: "Find similar items"
Better: "Identify products with similar price points, target audience, and market positioning to [specific product]"

Why it works: Provides specific comparison criteria and context

2. Contextual Understanding
Poor: "What happened in the meeting?"
Better: "Summarise the key decisions and action items from the quarterly planning meeting held on [date], focusing on budget allocation and project timelines"

Why it works: Provides specific context and focus areas

3. Numerical Processing
Poor: "Calculate the growth"
Better: "Calculate the year-over-year growth rate for Q1 2024 compared to Q1 2023, expressing the result as a percentage and highlighting any significant factors affecting the change"

Why it works: Specifies calculation method and required format

4. Sequential Logic
Poor: "Fix the problem"
Better: "Analyse the customer complaint about website loading times:
1. Check server response times
2. Review database query efficiency
3. Examine client-side performance
4. Propose optimisation solutions"

Why it works: Breaks down the task into logical steps
```

## Practice Exercises

### Exercise 1: Sales Analysis
```
Test Data:
sales_data.csv:
Date,Product,Units,Revenue,Cost
2024-01-01,Coffee Beans,45,£225.00,£112.50
2024-01-01,Pastries,78,£195.00,£58.50
2024-01-02,Tea Selection,32,£128.00,£44.80
2024-01-02,Coffee Beans,51,£255.00,£127.50
2024-01-03,Pastries,92,£230.00,£69.00

Basic Prompt:
"Analyse this sales data"

Enhanced Prompt:
"Analyse the provided sales data to:
1. Calculate profit margins by product
2. Identify best and worst performing products
3. Spot sales trends across dates
4. Suggest optimal inventory levels
5. Recommend pricing adjustments

Format the analysis as:
- Executive Summary
- Product Performance Analysis
- Trend Analysis
- Inventory Recommendations
- Pricing Strategy"
```

### Exercise 2: Customer Service
```
Test Data:
customer_case.json:
{
  "customer": {
    "type": "Premium subscription",
    "issue": "Mobile app login failing",
    "lastContact": "3 days ago",
    "subscription": {
      "value": "£49.99/month",
      "startDate": "2022-03-15",
      "plan": "Business Pro"
    },
    "history": {
      "previousIssues": [],
      "supportTickets": 1,
      "paymentStatus": "Current"
    },
    "deviceInfo": {
      "platform": "iOS 16.5",
      "appVersion": "2.4.1",
      "lastLogin": "2024-01-15"
    }
  }
}

Basic Prompt:
"Help resolve the customer's problem"

Enhanced Prompt:
"Create a detailed support response for a premium customer experiencing mobile app login issues:

1. Acknowledge the customer's status and issue
2. Reference their specific device and app details
3. Provide step-by-step troubleshooting instructions
4. Include escalation options if needed
5. Set clear expectations for resolution timeline

Format the response with:
- Personalised greeting
- Issue acknowledgment
- Troubleshooting steps
- Alternative solutions
- Follow-up plan
- Contact information"
```

## Tips for Success
- Start simple and build complexity
- Be specific about requirements
- Include relevant context
- Consider the audience
- Use clear, unambiguous language

## Common Mistakes to Avoid
- Being too vague
- Providing contradictory instructions
- Overcomplicating simple requests
- Forgetting to specify important details
- Using ambiguous language 