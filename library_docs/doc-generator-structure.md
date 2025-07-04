# Core Structure Pattern

### 1. **Goal Section (Strategic Context)**

- Define the document's purpose and strategic importance
- Explain how it fits into the broader project lifecycle
- Specify the target audience and stakeholders
- Establish the document as a "source of truth" for specific decisions

Example:
```text
## Goal

To guide an AI assistant in creating a detailed, actionable Product Brief in Markdown format that serves as the foundational document for all subsequent project planning. The brief should be comprehensive enough for stakeholders at all levels - from junior developers to senior leadership - to understand the product vision, requirements, and implementation approach.

The generated product brief will serve as the single source of truth and be referenced throughout the entire development lifecycle, including features documentation, user stories, user flows, UX/UI design, content strategy, technical architecture, testing plans, and go-to-market strategy.
```

### 2. **Process Section (Execution Framework)**

- Break down document creation into discrete, sequential steps
- Include document review/analysis phases before generation
- Require validation and quality checks
- End with save/versioning instructions

Example:
```text
## Process

1. **Receive Initial Prompt:** The user provides a brief description or request for a new app/product idea.
2. **Conduct Structured Discovery:** Use the comprehensive question framework below to gather all necessary information through multiple rounds of clarifying questions.
3. **Validate Understanding:** Summarize key findings and confirm alignment before proceeding.
4. **Generate Comprehensive Product Brief:** Create a detailed brief using the enhanced structure outlined below.
5. **Review and Refine:** Ensure completeness, clarity, and actionability.
6. **Save Product Brief:** Save as `master-product-brief.md` in the `/docs` directory.
```
### 3. **Discovery Framework (Information Gathering)**

- Organize questions by thematic categories (using emojis for visual hierarchy)
- Ask specific, actionable questions rather than general ones
- Include both functional and contextual questions
- Address multiple perspectives (user, business, technical)

Example:
```text
## Structured Discovery Questions

### 🎯 Product Vision & Strategy
- **Core Vision:** What is the fundamental problem this product solves?
- **Value Proposition:** What unique value does this product provide that alternatives don't?
- **Success Definition:** What does success look like in 6 months? 1 year? 3 years?
- **Market Timing:** Why is now the right time for this product?
- **Mission Alignment:** How does this product align with broader business/personal goals?

### 👥 Target Audience & User Research
- **Primary Users:** Who are the main users? (demographics, psychographics, behaviors)
- **Secondary Users:** Are there additional user types or influencers?
- **User Segments:** How do different user groups vary in needs/behaviors?
- **Pain Points:** What specific frustrations or challenges do users currently face?
- **Current Solutions:** How do users currently solve this problem?
- **Technology Adoption:** What's their comfort level with technology?
- **Usage Context:** When, where, and how will users interact with the product?

### 🏢 Market Analysis & Competitive Landscape
- **Market Size:** What's the addressable market size and growth potential?
- **Direct Competitors:** Who are the main competitors and what are their strengths/weaknesses?
- **Indirect Competitors:** What alternative solutions exist (including manual processes)?
- **Competitive Advantage:** What sustainable competitive advantages will you have?
- **Market Trends:** What industry trends support or threaten this product?
- **Barriers to Entry:** What challenges might new competitors face?

### 🛠️ Product Requirements & Features
- **Core Features (MVP):** What are the essential features for launch?
- **Feature Prioritization:** How should features be prioritized (MoSCoW method)?
- **User Workflows:** What are the key user journeys from start to finish?
- **Integration Requirements:** What third-party services/APIs are needed?
- **Data Requirements:** What data needs to be collected, stored, and processed?
- **Collaboration Features:** Are there multi-user or team collaboration needs?
- **Offline Capabilities:** What functionality should work without internet?
- **Accessibility Requirements:** What accessibility standards must be met?

### 📱 Platform & Technical Strategy
- **Platform Strategy:** Web app, mobile app, desktop app, or multi-platform?
- **Device Support:** Which devices and screen sizes need support?
- **Browser Support:** Which browsers and versions are required?
- **Performance Requirements:** What are the speed and responsiveness expectations?
- **Scalability Needs:** What user/data volume should the system handle?
- **Security Requirements:** What security and compliance standards apply?
- **Integration Ecosystem:** What existing systems need to integrate with?

### 🎨 User Experience & Design Direction
- **Design Philosophy:** What design principles should guide the product?
- **Brand Alignment:** How should the product reflect brand identity?
- **User Interface Style:** What visual style and interaction patterns are preferred?
- **Accessibility Standards:** What accessibility guidelines must be followed?
- **Responsive Design:** How should the experience adapt across devices?
- **Internationalization:** What languages and regions need support?

### 💰 Business Model & Monetization
- **Revenue Model:** How will the product generate revenue?
- **Pricing Strategy:** What pricing model and tiers are planned?
- **Payment Processing:** How will payments be handled?
- **Free vs. Paid Features:** What's included in free vs. paid tiers?
- **Trial/Freemium:** Will there be a trial period or freemium model?
- **Billing Cycles:** What billing frequencies are offered?
- **Refund Policy:** What's the refund and cancellation policy?

### 📊 Success Metrics & Analytics
- **Key Performance Indicators:** What metrics will define success?
- **User Engagement Metrics:** How will user engagement be measured?
- **Business Metrics:** What business KPIs need tracking?
- **Analytics Requirements:** What analytics tools and tracking are needed?
- **Reporting Needs:** What reports and dashboards are required?

### 🚀 Launch & Growth Strategy
- **Go-to-Market Strategy:** How will the product be launched and promoted?
- **Marketing Channels:** What marketing channels will be used?
- **Launch Timeline:** What's the desired launch timeline?
- **Beta Testing:** Will there be beta testing or soft launch phases?
- **Growth Strategy:** How will user acquisition and retention be achieved?
- **Partnerships:** Are there strategic partnerships to consider?

### ⚖️ Legal & Compliance
- **Data Privacy:** What data privacy regulations apply (GDPR, CCPA, etc.)?
- **Terms of Service:** What legal terms and conditions are needed?
- **Intellectual Property:** Are there IP considerations or restrictions?
- **Industry Regulations:** What industry-specific regulations apply?
- **Content Moderation:** Are there content guidelines or moderation needs?

### 🛡️ Risk Assessment & Mitigation
- **Technical Risks:** What technical challenges or risks exist?
- **Market Risks:** What market or competitive risks should be considered?
- **Resource Risks:** What resource constraints or dependencies exist?
- **Regulatory Risks:** What regulatory or compliance risks apply?
- **Mitigation Strategies:** How can identified risks be minimized?
```
### 4. **Output Structure (Template)**

- Provide comprehensive markdown template with all required sections
- Use nested hierarchies for complex information
- Include placeholders with specific guidance
- Ensure template supports decision-making, not just documentation

Example:
```text
## Product Brief Structure

The generated product brief should follow this comprehensive structure:

```markdown
# Product Brief: [Product Name]

## Executive Summary
- Product vision and mission
- Key value propositions
- Target market overview
- Success metrics summary

## Product Overview
### Problem Statement
### Solution Overview
### Unique Value Proposition
### Market Opportunity

## Target Audience
### Primary User Personas
### Secondary User Personas
### User Needs and Pain Points
### User Journey Overview

## Market Analysis
### Market Size and Opportunity
### Competitive Landscape
### Competitive Advantage
### Market Trends and Timing

## Product Requirements
### Core Features (MVP)
### Feature Prioritization
### User Stories and Workflows
### Technical Requirements
### Integration Requirements
### Performance and Scalability Requirements
### Security and Compliance Requirements

## Platform and Technical Strategy
### Platform Decision and Rationale
### Technology Stack Recommendations
### Architecture Considerations
### Third-party Dependencies
### Scalability and Performance Plan

## User Experience Strategy
### Design Principles
### User Interface Direction
### Accessibility Requirements
### Responsive Design Strategy
### Internationalization Plan

## Business Model
### Revenue Strategy
### Pricing Model
### Monetization Plan
### Customer Acquisition Strategy

## Success Metrics and KPIs
### Key Performance Indicators
### User Engagement Metrics
### Business Metrics
### Analytics and Reporting Requirements

## Go-to-Market Strategy
### Launch Plan
### Marketing Strategy
### Partnership Opportunities
### Growth Strategy

## Risk Assessment
### Technical Risks
### Market Risks
### Mitigation Strategies

## Resource Requirements
### Team Structure
### Budget Considerations
### Timeline Estimates
### External Dependencies

## Next Steps
### Immediate Action Items
### Documentation Dependencies
### Stakeholder Approvals Needed
```

### 5. **Quality Assurance (Validation Framework)**

- Create specific, checkable criteria for document quality
- Include multiple validation dimensions (completeness, alignment, actionability)
- Require cross-reference validation with previous documents
- Establish measurable success criteria

Example: 
```text
Before finalizing the product brief, ensure:

- [ ] All sections are complete and detailed
- [ ] Technical requirements are specific and measurable
- [ ] User needs are clearly articulated with supporting evidence
- [ ] Competitive analysis is thorough and current
- [ ] Success metrics are SMART (Specific, Measurable, Achievable, Relevant, Time-bound)
- [ ] Risks are identified with mitigation strategies
- [ ] Next steps are actionable and assigned
- [ ] Document is suitable for both technical and non-technical stakeholders
- [ ] All assumptions are clearly stated
- [ ] Dependencies and constraints are identified
```

### 6. **Best Practices for Document Generation Rules**

Example:
```text
## Best Practices

1. **Be Specific:** Avoid vague language; use concrete examples and measurable criteria
2. **Think Systemically:** Consider how features interact and affect the overall user experience
3. **Plan for Scale:** Address both current needs and future growth scenarios
4. **Consider Edge Cases:** Think through unusual but possible user scenarios
5. **Validate Assumptions:** Clearly state assumptions and plans for validation
6. **Keep Users Central:** Every decision should be justified by user value
7. **Balance Ambition with Reality:** Set challenging but achievable goals
8. **Document Trade-offs:** Explain why certain decisions were made over alternatives
```

### 7. **Output Requirements**

Example:
```text
## Output Requirements

- **Format:** Markdown (`.md`)
- **Location:** `/docs/`
- **Filename:** `master-product-brief.md`
- **Length:** Comprehensive but concise (typically 15-25 pages)
- **Audience:** Accessible to stakeholders at all technical levels
- **Maintenance:** Include version control and update procedures
```

### 8. **Final Instructions**

Example: 
```text
## Final Instructions

1. **DO NOT** start implementing the product brief until all discovery questions are answered
2. **DO** ask follow-up questions to clarify ambiguous or incomplete responses
3. **DO** validate your understanding by summarizing key points before proceeding
4. **DO** ensure the brief is comprehensive enough to guide all subsequent project phases

5. **DO** include specific, actionable next steps and clear success criteria
```

### 9. **Success Factors**

Example: 
```text
## Key Success Factors

1. **Comprehensive but Focused:** Cover all necessary aspects without overwhelming detail
2. **Evidence-Based:** Require justification and sources for key decisions
3. **Iterative Validation:** Multiple checkpoints prevent drift from strategy
4. **Cross-Functional Design:** Serve multiple team roles and decision-making needs
5. **Future-Oriented:** Consider evolution and maintenance requirements
6. **Actionable Outputs:** Generate documents that drive concrete next steps
```


## Additional Considerations

### **Sequential Document Dependencies**

- Always require review of previous documents before starting new ones
- Create explicit integration points between documents
- Validate alignment and identify conflicts between documents
- Build knowledge progressively rather than in isolation

### **Structured Information Architecture**

- Use consistent categorization across all rules (Goals, Process, Discovery, Output, QA)
- Apply thematic grouping with visual indicators (emojis, headers)
- Create logical information hierarchies
- Ensure templates support both creation and future reference

### **Multi-Perspective Discovery**

- Include user, business, technical, and market perspectives
- Ask both "what" and "why" questions
- Address current state and future evolution
- Consider edge cases and constraints

### **Actionability Focus**

- Require specific, measurable criteria rather than general descriptions
- Include implementation guidance and next steps
- Define success metrics for each document
- Ensure outputs can drive concrete decisions

### **Quality Control Framework**

- Create multiple validation checkpoints
- Require specific evidence or justification for key decisions
- Include both content quality and strategic alignment checks
- Establish regular review and update procedures
