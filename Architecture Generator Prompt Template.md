# Architecture Generator Prompt Template
# Copy and customize the prompt below for any new project

---

## THE PROMPT

```
Create an interactive React (.jsx) architecture document for [PROJECT NAME] — [one-line description].

Use this exact structure and format:

**File format:** Single React JSX file using Tailwind CSS utility classes only (no external CSS). Use useState from React. Export a default component.

**Layout:** Tabbed interface with a header (icon + title + version), horizontal tab navigation, white card content area, and a footer. Max width ~4xl, gray-50 background.

**Required Tabs (6):**

1. 📋 Overview Tab
   - Centered hero with emoji icon, project name, tagline, and description
   - Grid of design principles (cards with title + description)
   - Highlighted callout box for scalability/future vision

2. 📑 Requirements Tab
   - Toggle between Functional and Non-Functional views (with counts)
   - Summary bar showing categories count, total requirements, and priority legend
   - Expandable category accordions (icon + colored label + count)
   - Each requirement has: ID (e.g., FR-001), name, description, and MoSCoW priority tag (Must/Should/Could) for functional; no priority for non-functional
   - Bottom callout box with contextual notes per section
   - Aim for 50-70 functional requirements across 8-10 categories
   - Aim for 30-40 non-functional requirements across 6-7 categories (Performance, Security, Scalability, Availability, Usability, Compliance, Maintainability)

3. 🏗️ Architecture Tab
   - Layered accordion structure (5 layers: Presentation, API Gateway, Core Services, Data/Infrastructure, Integration)
   - Each layer: colored header with icon, name, component count
   - Nested accordion for each component with bullet-point implementation details
   - Use distinct colors per layer

4. 🗃️ Data Model Tab
   - Entity cards with monospace entity name (colored badge) + field list
   - Highlight boxes explaining key architectural decisions (e.g., anonymity, data flow, separation of concerns)

5. 🛠️ Tech Stack Tab
   - Grouped by category (Frontend, Backend, [Domain-Specific], Database, Infrastructure)
   - Each item: tech name in colored monospace badge + purpose description
   - Grid layout (2 columns on desktop)

6. 🗺️ Roadmap Tab
   - 5 phases with numbered circle badges, phase name, duration estimate
   - Expandable bullet lists per phase
   - Post-roadmap callout box for future expansion

**Data architecture:** Store ALL content in a single `architectureData` const object at the top of the file. Tabs render from this data. This makes it easy to modify content without touching component code.

**Styling rules:**
- Each layer/category gets a unique hex color
- Use color + "40" for borders, color + "10" for backgrounds, color + "08" for subtle fills, color + "15" for badges
- Accordion expand/collapse with ▲/▼ indicators
- Text sizes: headers sm, body xs, IDs 10px mono
- Hover states on interactive elements
- Responsive: works on mobile with overflow-x-auto where needed

**The project context:**
[DESCRIBE YOUR PROJECT HERE — what it does, who it serves, key domain concepts, any specific technologies or constraints you want included]

**Domain-specific requirements to emphasize:**
[LIST ANY SPECIFIC FEATURES OR REQUIREMENTS THAT ARE CRITICAL TO YOUR PROJECT]
```

---

## EXAMPLE ADAPTATIONS

### For a Healthcare Patient Portal:
```
The project context:
A multi-tenant SaaS patient portal for healthcare clinics. Patients can book appointments, view lab results, message doctors, manage prescriptions, and handle billing. Must be HIPAA compliant. Integrates with EHR systems (Epic, Cerner). Supports telemedicine video visits.

Domain-specific requirements to emphasize:
- HIPAA compliance throughout (BAA, PHI encryption, access logging)
- EHR/EMR integration via HL7 FHIR APIs
- Telemedicine video visits with waiting room
- Prescription management with pharmacy integration
- Patient consent management workflows
```

### For an E-Commerce Marketplace:
```
The project context:
A multi-vendor marketplace platform where sellers list products, buyers browse and purchase, and the platform handles payments, shipping coordination, and dispute resolution. Think Etsy/Amazon hybrid. Must support multiple currencies and international shipping.

Domain-specific requirements to emphasize:
- Seller onboarding and verification workflows
- Multi-currency payment processing with split payouts
- Product catalog with faceted search and recommendations
- Order lifecycle with shipping carrier integration
- Review/rating system with fraud detection
- Dispute resolution and refund workflows
```

### For an EdTech Learning Platform:
```
The project context:
An online learning platform for professional certifications. Instructors create courses with video, quizzes, and hands-on labs. Students track progress, earn certificates, and join cohort-based programs. Must support proctored exams and continuing education credits.

Domain-specific requirements to emphasize:
- Course builder with multimedia content types
- Proctored exam engine with anti-cheating measures
- Certificate generation with blockchain verification
- Learning path and prerequisite management
- Cohort management with scheduled releases
- CE/CPE credit tracking and reporting to governing bodies
```

---

## TIPS FOR BEST RESULTS

1. **Be specific about your domain** — the more context you give about your industry and users, the more relevant the requirements and architecture will be.

2. **Mention compliance/regulatory needs** — if your domain has specific regulations (HIPAA, PCI-DSS, GDPR, SOX), mention them explicitly.

3. **State your scale expectations** — "serves 500 users" vs "serves 5 million users" produces very different architectures.

4. **Include integration needs** — list any third-party systems the platform must connect to.

5. **Specify if you want blockchain, AI/ML, or other specialized components** — these add dedicated layers to the architecture.

6. **If the output is too long and gets cut off**, ask: "Continue from where you left off" or break it into: "Generate the data object first, then the components."