# 📚 Product Prompt Library

A curated collection of AI prompts for product managers and product teams to accelerate backlog building, product discovery, and digital product development.

---

## Table of Contents

1. [User Stories & Backlog Items](#1-user-stories--backlog-items)
2. [Epics & Themes](#2-epics--themes)
3. [Backlog Prioritization](#3-backlog-prioritization)
4. [Product Discovery & User Research](#4-product-discovery--user-research)
5. [Problem Framing & Opportunity Assessment](#5-problem-framing--opportunity-assessment)
6. [Product Requirements Documents (PRD)](#6-product-requirements-documents-prd)
7. [Feature Specifications](#7-feature-specifications)
8. [Roadmap Planning](#8-roadmap-planning)
9. [Stakeholder Communication](#9-stakeholder-communication)
10. [Metrics & Success Criteria](#10-metrics--success-criteria)
11. [Digital Product Creation](#11-digital-product-creation)
12. [Competitive Analysis](#12-competitive-analysis)

---

## 1. User Stories & Backlog Items

### Generate a user story from a feature idea
```
Write a user story for the following feature idea: [feature idea].
Use the format: "As a [user type], I want to [action], so that [benefit]."
Include acceptance criteria as a checklist.
```

### Expand a user story with sub-tasks
```
Given this user story: "[user story]"
Break it down into concrete development tasks that a team could estimate and implement.
List each task as a bullet point with a brief description.
```

### Generate multiple user stories from an epic
```
I have this epic: "[epic description]"
Generate 5–8 user stories that would compose this epic, covering the main user journeys.
Use the "As a / I want / So that" format and include acceptance criteria for each.
```

### Refine a vague backlog item
```
This backlog item is unclear: "[vague item]"
Rewrite it as a clear, actionable user story with acceptance criteria. Ask me any clarifying questions before rewriting if needed.
```

### Generate edge cases and error scenarios
```
For this user story: "[user story]"
List all edge cases, error states, and boundary conditions that should be covered by the acceptance criteria.
```

---

## 2. Epics & Themes

### Define an epic from a business goal
```
Our business goal is: "[business goal]"
Define a product epic that addresses this goal. Include:
- Epic title
- Problem statement
- Who it affects
- High-level scope (what's in and out)
- Expected business value
```

### Break a theme into epics
```
We have this product theme: "[theme]"
Break it into 3–5 epics, each with a short title and one-sentence description of the value it delivers.
```

### Write an epic hypothesis statement
```
Write a hypothesis statement for this epic: "[epic title and description]"
Use the format: "We believe that [building/changing X] for [user type] will result in [outcome]. We will know this is true when [measurable signal]."
```

---

## 3. Backlog Prioritization

### RICE scoring
```
I have the following backlog items: [list of items]
Score each item using the RICE framework (Reach, Impact, Confidence, Effort) on a scale of 1–10.
Provide a final RICE score and a recommended priority order with a brief rationale.
```

### MoSCoW prioritization
```
Given these features for our next release: [list of features]
And our constraints: [time/team/budget constraints]
Classify each feature as Must Have, Should Have, Could Have, or Won't Have (MoSCoW).
Explain the reasoning for each classification.
```

### Value vs. Effort matrix
```
Evaluate these backlog items on a 2x2 Value vs. Effort matrix: [list of items]
Categorize each as: Quick Wins (high value, low effort), Major Projects (high value, high effort), Fill-ins (low value, low effort), or Hard Slogs (low value, high effort).
```

### Prioritize with competing stakeholder requests
```
I have competing requests from different stakeholders:
[Stakeholder A wants: ...]
[Stakeholder B wants: ...]
[Stakeholder C wants: ...]
Help me evaluate these requests against our product goal "[product goal]" and suggest a prioritization with rationale.
```

### Create a sprint backlog
```
From this product backlog: [list of items with rough sizes]
Our team velocity is [X] story points per sprint and this sprint is [N] weeks.
Suggest a sprint backlog, ensuring a mix of value delivery and technical health.
```

---

## 4. Product Discovery & User Research

### Generate user interview questions
```
I am researching the following problem: "[problem statement]"
My target user is: "[user persona]"
Write 10 open-ended interview questions to help me understand their needs, behaviours, and pain points related to this problem.
```

### Synthesise interview notes into insights
```
Here are raw notes from [N] user interviews about [topic]: 
[paste notes]
Identify the top 5 themes and insights. For each, note how many participants mentioned it and include a representative quote if available.
```

### Create a user persona
```
Based on the following research data: [summary of research findings]
Create a detailed user persona including:
- Name and demographic snapshot
- Goals and motivations
- Pain points and frustrations
- Current behaviours and workarounds
- What success looks like for them
```

### Design a survey for product feedback
```
I want to measure [what you want to learn] from [target audience].
Create a short survey (max 8 questions) using a mix of Likert scales, multiple choice, and one open-ended question.
Include a brief intro and keep the language friendly and concise.
```

### Identify assumptions to validate
```
We are building: "[product or feature idea]"
List the key assumptions we are making about users, the problem, and the solution.
For each assumption, suggest the fastest way to validate or invalidate it.
```

---

## 5. Problem Framing & Opportunity Assessment

### Write a problem statement
```
Here is the situation: "[background context]"
Write a clear, user-centred problem statement that describes who is affected, what the problem is, and why it matters. Avoid including a solution.
```

### Opportunity sizing
```
Help me estimate the opportunity size for this problem: "[problem]"
Target market: [description]
Available data points: [any data you have]
Walk me through a top-down or bottom-up sizing approach and give me a rough estimate with key assumptions.
```

### Jobs-to-be-Done framing
```
Reframe this feature request: "[feature request]"
Using the Jobs-to-be-Done framework, identify:
- The functional job the user is trying to accomplish
- The emotional job (how they want to feel)
- The social job (how they want to be perceived)
- Key success and failure metrics from the user's perspective
```

### How Might We (HMW) questions
```
Given this problem: "[problem statement]"
Generate 10 "How Might We..." questions that open up the solution space without prescribing a solution.
```

---

## 6. Product Requirements Documents (PRD)

### Generate a full PRD
```
Write a Product Requirements Document (PRD) for the following feature: "[feature name]"
Context: [brief product and business context]
Include these sections:
1. Overview & objective
2. Background and problem statement
3. Goals and success metrics
4. User personas and use cases
5. Functional requirements (as user stories)
6. Non-functional requirements (performance, security, accessibility)
7. Out of scope
8. Open questions
9. Dependencies and risks
```

### Write the executive summary of a PRD
```
Here is a detailed PRD: [paste PRD or summary]
Write a concise executive summary (max 200 words) for a senior leadership audience that covers: what we're building, why, for whom, and what success looks like.
```

### Review and improve a PRD
```
Review this PRD for clarity, completeness, and alignment with product best practices: [paste PRD]
Flag any missing sections, ambiguous requirements, or areas that need more detail.
Suggest improvements with specific rewrites where helpful.
```

---

## 7. Feature Specifications

### Write a feature spec
```
Write a detailed feature specification for: "[feature name]"
Product context: "[context]"
Include:
- Feature description and user value
- User flows (step by step)
- UI/UX considerations
- Functional requirements
- Edge cases and error handling
- Analytics events to track
```

### Define API requirements
```
For this feature: "[feature description]"
Define the API requirements, including:
- Endpoints needed (method, path, purpose)
- Request parameters and body schema
- Response schema
- Error codes and messages
- Authentication requirements
```

### Write a technical handoff document
```
Turn this feature spec into a developer-ready technical handoff document for: "[feature name]"
Spec: [paste spec]
Include implementation notes, data model changes, and any decisions that were made and why.
```

---

## 8. Roadmap Planning

### Build a quarterly roadmap
```
Our product goals for the next quarter are: [list of goals]
We have these themes and initiatives in our backlog: [list]
Our team capacity is: [N engineers, N designers, N weeks]
Suggest a realistic quarterly roadmap, organized by month, with rationale for sequencing decisions.
```

### Write a roadmap narrative
```
Here is our product roadmap for the next [time period]: [roadmap items]
Write a narrative that explains our strategy and sequencing to share with stakeholders. 
Tone: confident and clear. Audience: senior leadership.
```

### Identify roadmap dependencies and risks
```
Review this roadmap: [roadmap items with timelines]
Identify:
1. Dependencies between items
2. External dependencies (third parties, other teams)
3. Key risks and a suggested mitigation for each
```

### Create a "Now / Next / Later" roadmap
```
We have these potential initiatives: [list of initiatives]
Our current product focus is: [focus area]
Organise these into a Now / Next / Later roadmap framework. Provide a brief rationale for each placement.
```

---

## 9. Stakeholder Communication

### Write a product update email
```
Write a product update email to [audience, e.g., "the whole company"] covering:
- What we shipped this [week/sprint/month]: [list of items]
- What we're working on next: [list of items]
- Any blockers or decisions needed from stakeholders
Keep it concise, positive, and focused on value delivered.
```

### Prepare for a stakeholder review meeting
```
I have a stakeholder review meeting about [topic] with [audience].
Help me prepare by:
1. Suggesting a clear agenda (30 minutes)
2. Anticipating the top 5 questions or objections I might face
3. Drafting a one-page briefing document
```

### Handle a feature request diplomatically
```
A stakeholder has requested this feature: "[feature request]"
This feature is not on our current roadmap because: "[reason]"
Help me draft a response that:
- Acknowledges the request and the underlying need
- Explains our current priorities
- Keeps the relationship positive and the door open
```

### Write a release announcement
```
We are releasing [feature/product name] on [date].
Key capabilities: [list]
Target users: [users]
Write an internal release announcement and a short external changelog entry.
```

---

## 10. Metrics & Success Criteria

### Define success metrics for a feature
```
For this feature: "[feature name and description]"
Define a set of success metrics covering:
- Primary metric (north star for this feature)
- Secondary metrics (supporting indicators)
- Guardrail metrics (what we must not break)
Include how each metric would be measured and a realistic target.
```

### Write OKRs for a product team
```
Our company objective for this quarter is: "[objective]"
Our product team is responsible for: "[area]"
Write 3–4 Key Results for our team that are specific, measurable, and achievable in one quarter.
```

### Design an A/B test
```
We want to test this hypothesis: "[hypothesis]"
Feature being tested: "[feature]"
Help me design an A/B test including:
- Control and variant description
- Primary metric and success threshold
- Sample size estimate and recommended test duration
- Risks and what to watch for
```

### Interpret product analytics data
```
Here is a summary of our product analytics for the past [time period]: [data summary]
Identify the key trends, anomalies, and opportunities. Suggest 3 hypotheses that could explain the patterns you see and recommend next steps.
```

---

## 11. Digital Product Creation

### Ideate a new digital product
```
We want to build a digital product for [target audience] that solves [problem].
Generate 5 distinct product concepts, each with:
- Product name and tagline
- Core value proposition
- Key features (top 3)
- Revenue model
- Biggest risk
```

### Write a product vision statement
```
Write a compelling product vision statement for: "[product name]"
Context: [target users, problem solved, market]
Keep it to 2–3 sentences. It should be aspirational, user-centred, and differentiated.
```

### Create a lean canvas
```
Complete a Lean Canvas for this product idea: "[product idea]"
Fill in all nine blocks:
1. Problem
2. Customer Segments
3. Unique Value Proposition
4. Solution
5. Channels
6. Revenue Streams
7. Cost Structure
8. Key Metrics
9. Unfair Advantage
```

### Define an MVP
```
Our full product vision is: "[vision]"
We have [N] months and [team size] to build the first version.
Define an MVP that:
- Delivers core value to early adopters
- Is achievable within our constraints
- Sets us up to learn and iterate
List the features in scope and explicitly call out what is out of scope.
```

### Map a user journey
```
Map the end-to-end user journey for "[user type]" using our product to accomplish "[goal]".
For each stage, describe:
- What the user is doing
- What they are thinking / feeling
- Touchpoints with our product
- Pain points or moments of delight
- Opportunities to improve the experience
```

### Write onboarding flow copy
```
Write the copy for a [N]-step onboarding flow for [product name].
Target user: [persona]
Goal: get the user to [activation milestone] in their first session.
For each step include: headline, body text (max 2 sentences), and CTA button label.
```

---

## 12. Competitive Analysis

### Conduct a competitive landscape analysis
```
I am building [product description] in the [market/industry] space.
Identify the top 5 competitors and for each provide:
- Company name and product overview
- Target customer and positioning
- Key strengths
- Key weaknesses
- How we could differentiate
```

### Compare feature sets
```
Compare the feature sets of [Product A], [Product B], and [our product] across these dimensions: [list of dimensions].
Present the results as a comparison table and summarise where we have gaps and where we have advantages.
```

### Write a positioning statement
```
Based on this competitive analysis: [summary]
And our product strengths: [strengths]
Write a positioning statement using the format:
"For [target customer] who [need or pain point], [product name] is a [category] that [key benefit]. Unlike [main alternative], our product [key differentiator]."
```

---

## 💡 Tips for Using These Prompts

- **Add context**: The more context you give (product name, target users, constraints), the better the output.
- **Iterate**: Treat the first output as a draft. Follow up with "Make it more concise," "Add more detail to section X," or "Rewrite in a [tone] tone."
- **Combine prompts**: Use the output from one prompt as the input for another (e.g., generate a persona, then use it to write interview questions).
- **Stay in the loop**: AI outputs should be reviewed and refined. You bring the product context and judgment.

---

*Contributions welcome! Open a PR to add new prompts or improve existing ones.*
