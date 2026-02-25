# Superprompt: Scalable Architecture & Infrastructure Design

## Purpose
Use this prompt with an AI assistant to define the architecture and infrastructure of any technological project that needs to scale. Fill in the placeholders in `[brackets]` before submitting, or let the AI ask you for the missing details.

---

## The Prompt

```
You are a senior solutions architect and infrastructure engineer with deep expertise in cloud-native systems, distributed architectures, and scalable platform design.

I need your help designing the architecture and infrastructure for the following project:

**Project Overview**
- Project name: [e.g., "Real-time analytics platform for e-commerce"]
- Core problem it solves: [brief description]
- Target users / customers: [e.g., "10,000 SMB merchants initially, scaling to 1M+"]
- Current stage: [idea / MVP / growth / scale]

**Functional Requirements**
- Key features and capabilities: [list the main features]
- Critical user journeys: [e.g., "user uploads data → system processes → dashboard updates in < 2s"]
- Integrations needed: [e.g., "Stripe, Salesforce, external REST APIs"]

**Non-Functional Requirements**
- Expected load at launch: [requests/day, concurrent users, data volume]
- Expected load in 12–24 months: [growth targets or projections]
- Latency targets: [e.g., "< 200ms p99 for API responses"]
- Availability target: [e.g., "99.9% uptime"]
- Data residency / compliance constraints: [e.g., "GDPR, HIPAA, data must stay in EU"]
- Security requirements: [e.g., "SOC 2, zero-trust network, encryption at rest and in transit"]

**Tech Context**
- Preferred cloud provider(s): [AWS / GCP / Azure / multi-cloud / on-premise / no preference]
- Existing tech stack (if any): [languages, frameworks, databases already in use]
- Team size and expertise: [e.g., "5 engineers, strong Python/JS, no Kubernetes experience yet"]
- Budget constraints: [e.g., "< $5,000/month initially"]

---

Based on the information above, please provide a comprehensive architecture and infrastructure plan that covers:

1. **Architecture Pattern**
   - Recommended high-level architecture (monolith / microservices / modular monolith / event-driven / serverless / hybrid) with justification.
   - Key architectural principles to follow (e.g., twelve-factor app, CQRS, SAGA pattern).

2. **Component Breakdown**
   - All major system components (frontend, backend services, data layer, messaging, etc.).
   - Responsibilities and boundaries of each component.
   - Communication protocols between components (REST, gRPC, WebSockets, message queues).

3. **Data Architecture**
   - Database selection per component/use case (relational, NoSQL, time-series, graph, vector, etc.) with rationale.
   - Data flow and data ownership model.
   - Caching strategy (where, what, and how long to cache).
   - Backup, retention, and disaster recovery approach.

4. **Infrastructure & Cloud Design**
   - Cloud services to use (compute, storage, networking, managed services) with specific service names.
   - Infrastructure as Code (IaC) tooling recommendation (Terraform, Pulumi, CDK, etc.).
   - Environment strategy (dev / staging / production) and promotion workflow.
   - Networking topology (VPC design, subnets, peering, CDN, DNS, load balancing).

5. **Scalability Strategy**
   - Horizontal vs. vertical scaling decisions per component.
   - Auto-scaling triggers and policies.
   - Stateless design patterns and session management approach.
   - Database scaling strategy (read replicas, sharding, connection pooling).

6. **Observability & Reliability**
   - Logging, metrics, and tracing stack.
   - Key SLIs/SLOs to define and monitor.
   - Alerting strategy (who gets alerted, on what, at what threshold).
   - On-call and incident response process outline.

7. **Security & Compliance**
   - Identity and access management (IAM) strategy.
   - Secrets management approach.
   - Network security controls (WAF, firewall rules, DDoS protection).
   - Data privacy controls and compliance checklist for stated requirements.

8. **CI/CD & Developer Experience**
   - Recommended CI/CD pipeline stages and tooling.
   - Branching strategy and deployment frequency target.
   - Feature flagging and rollback strategy.
   - Local development environment setup guidance.

9. **Cost Estimation**
   - Rough monthly cost at launch and at projected scale.
   - Top cost drivers and optimization levers.
   - FinOps practices to adopt from day one.

10. **Roadmap & Migration Path**
    - Phase 0 (MVP): minimum infrastructure to ship.
    - Phase 1 (Growth): changes needed to handle 10× load.
    - Phase 2 (Scale): changes needed to handle 100× load.
    - Technical debt to consciously accept now and address later.

Please also call out:
- The **top 3 risks** in this architecture and how to mitigate them.
- Any **assumptions** you made where my inputs were ambiguous.
- A **decision log** for the most important architectural trade-offs you made.

Format the output with clear headings, bullet points, and—where useful—ASCII diagrams or Mermaid diagram code blocks to illustrate the architecture.
```

---

## Tips for Getting the Best Results

- **Be specific with numbers.** Vague load estimates ("a lot of users") produce generic answers. Even rough estimates ("~50k daily active users in year 1") unlock much more actionable advice.
- **Iterate section by section.** After the AI produces the full plan, follow up on individual sections: *"Expand on the database sharding strategy for section 3"* or *"Give me the Terraform module structure for section 4."*
- **Challenge trade-offs.** Ask the AI to argue for an alternative: *"Make the case for a monolith instead of microservices for my stage."*
- **Validate costs.** Use the AI-generated estimate as a starting point, then verify with the cloud provider's pricing calculator.
- **Re-run at each growth stage.** Architecture needs change. Revisit this prompt when you hit Phase 1 or Phase 2 milestones.
