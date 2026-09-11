# DiagramWise

### Intelligent Diagram Generation, Editing & Validation Platform

> **Transform natural-language scenarios into editable, standards-aware diagrams — understand, validate, refine, and export with confidence.**

---

## 📌 Table of Contents

* [About DiagramWise](#-about-diagramwise)
* [Problem Statement](#-problem-statement)
* [Proposed Solution](#-proposed-solution)
* [Project Objectives](#-project-objectives)
* [Target Users](#-target-users)
* [Key Features](#-key-features)
* [Supported Diagram Types](#-supported-diagram-types)
* [How DiagramWise Works](#-how-diagramwise-works)
* [System Workflow](#-system-workflow)
* [AI-Assisted Structure Analysis](#-ai-assisted-structure-analysis)
* [Rule-Based Validation](#-rule-based-validation)
* [Interactive Diagram Editor](#-interactive-diagram-editor)
* [Diagram Explanation](#-diagram-explanation)
* [Suggested Corrections](#-suggested-corrections)
* [Academic Mode](#-academic-mode)
* [Auto Layout](#-auto-layout)
* [Save and Version History](#-save-and-version-history)
* [Templates](#-templates)
* [Export](#-export)
* [System Architecture](#-system-architecture)
* [Technology Stack](#-technology-stack)
* [Project Structure](#-project-structure)
* [Database Design](#-database-design)
* [Core Data Model](#-core-data-model)
* [Installation](#-installation)
* [Environment Variables](#-environment-variables)
* [Running the Project](#-running-the-project)
* [Using DiagramWise](#-using-diagramwise)
* [Example](#-example)
* [API Overview](#-api-overview)
* [Validation Workflow](#-validation-workflow)
* [Development Roadmap](#-development-roadmap)
* [MVP Scope](#-mvp-scope)
* [Future Enhancements](#-future-enhancements)
* [Security Considerations](#-security-considerations)
* [Testing](#-testing)
* [Project Significance](#-project-significance)
* [Contributing](#-contributing)
* [Author](#-author)

---

# 🧠 About DiagramWise

**DiagramWise** is a web-based intelligent diagram generation and editing platform designed to help students, software developers, business analysts, and project managers create **clear, editable, structured, and standards-aware diagrams from natural-language scenarios**.

Creating software engineering and project management diagrams can be challenging, especially when the underlying scenario is complex. Users often need to understand a textual description, identify relevant elements, determine relationships, select appropriate notation, manually construct the diagram, organize its layout, and finally verify whether the result follows the expected standard.

DiagramWise aims to simplify this entire process.

Instead of simply generating a static diagram from a prompt, DiagramWise follows a structured approach:

```text
Natural-Language Scenario
          ↓
   AI Scenario Analysis
          ↓
 Structure Extraction
          ↓
   User Review & Editing
          ↓
    Diagram Generation
          ↓
   Rule-Based Validation
          ↓
 Interactive Diagram Editor
          ↓
     Explain / Refine
          ↓
      Save / Export
```

The core philosophy of DiagramWise is:

> **The AI suggests the structure, the system validates it, and the user controls the final diagram.**

---

# ❗ Problem Statement

Students and novice developers often struggle to transform textual system requirements into appropriate software engineering diagrams.

For a complex scenario, users need to determine:

* What should be represented?
* Which actors or entities are relevant?
* Which elements should be excluded?
* What actions or processes exist?
* Which elements are connected?
* What type of relationship should be used?
* Which diagram notation is appropriate?
* How should the diagram elements be positioned?
* Does the final diagram follow standard notation?
* Are unnecessary or incorrect elements present?

Traditional diagramming tools provide powerful drawing capabilities, but they generally assume that the user already understands the required diagram notation.

On the other hand, generic AI tools can generate diagrams quickly but may produce results that are:

* Overly complex
* Structurally incorrect
* Inconsistent
* Difficult to edit
* Poorly organized
* Missing important relationships
* Containing unnecessary elements
* Not aligned with expected academic or industry notation

Therefore, there is a need for a system that combines:

**AI-assisted scenario understanding + structured diagram generation + rule-based validation + interactive editing + visual explanation.**

---

# 💡 Proposed Solution

DiagramWise provides a guided workflow for transforming natural-language scenarios into structured and editable diagrams.

Instead of directly generating an image, DiagramWise first converts the user's scenario into a structured diagram model.

For example:

```text
Scenario
   ↓
Actors
   ↓
Use Cases
   ↓
Relationships
   ↓
Validation
   ↓
Diagram
```

The user can review and modify the extracted structure before generating the final diagram.

This approach provides several advantages:

* The generated diagram remains editable.
* Diagram elements can be validated individually.
* Relationships can be checked.
* The underlying structure can be stored.
* The diagram can be regenerated without starting from scratch.
* Users can understand why elements and relationships were suggested.

---

# 🎯 Project Objectives

## Primary Objective

To develop an intelligent and user-friendly platform capable of generating, editing, validating, explaining, saving, and exporting software engineering and project management diagrams from natural-language scenarios.

## Specific Objectives

1. Allow users to describe systems or processes using natural language.
2. Automatically identify relevant diagram elements.
3. Identify potential relationships between elements.
4. Allow users to review and modify the extracted structure.
5. Generate diagrams using appropriate notation.
6. Provide an interactive and editable diagram canvas.
7. Validate diagrams using predefined structural rules.
8. Highlight potential structural issues.
9. Explain why elements and relationships were included.
10. Suggest possible corrections without automatically overriding user decisions.
11. Provide automatic diagram layout assistance.
12. Allow users to save and manage diagrams.
13. Support diagram version history.
14. Provide commonly used export formats.
15. Gradually support multiple diagram types.

---

# 👥 Target Users

## 🎓 University Students

DiagramWise is particularly useful for students studying:

* Information Systems
* Computer Science
* Software Engineering
* Business Information Systems
* System Analysis and Design
* Project Management

Students can use DiagramWise for:

* Assignments
* Practical sessions
* Reports
* Presentations
* Exam preparation
* Software project documentation

---

## 👨‍💻 Junior Developers

Developers can use DiagramWise to visualize:

* System requirements
* User interactions
* Application processes
* Object relationships
* System architecture
* Functional workflows

---

## 🧑‍💼 Business and System Analysts

Analysts can use the platform to transform textual requirements into structured visual representations.

---

## 📋 Project Managers

Project managers can use DiagramWise for:

* Work Breakdown Structures
* Process visualization
* Project planning
* System overviews
* Documentation

---

# ✨ Key Features

## 1. Natural-Language Scenario Input

Users can describe a system or process using ordinary language.

Example:

> "A student logs into the university registration system, selects courses, and submits the registration. The system checks prerequisites and seat availability before confirming the registration."

DiagramWise analyzes the scenario and extracts relevant information.

---

## 2. AI-Assisted Structure Analysis

The AI identifies potential:

* Actors
* Entities
* Actions
* Processes
* Events
* Relationships
* External systems

The extracted information is presented to the user before diagram generation.

---

## 3. User Review and Modification

Users can review the AI-generated structure and:

* Add elements
* Remove elements
* Rename elements
* Modify descriptions
* Change relationships
* Approve the structure

The user remains in control instead of blindly accepting the AI output.

---

## 4. Automatic Diagram Generation

Once the structure is approved, DiagramWise converts the structured representation into a visual diagram.

```text
Structured JSON
      ↓
Diagram Nodes
      ↓
Diagram Edges
      ↓
Layout Engine
      ↓
Interactive Canvas
```

---

## 5. Interactive Diagram Editor

Users can modify generated diagrams manually.

Supported operations can include:

* Drag elements
* Move elements
* Rename elements
* Add elements
* Delete elements
* Duplicate elements
* Add relationships
* Delete relationships
* Change relationship types
* Zoom
* Pan
* Undo
* Redo
* Align elements
* Distribute elements
* Auto-layout

---

## 6. Standards-Aware Validation

DiagramWise uses rule-based validation to identify possible structural problems.

For example, a Use Case Diagram can be checked for:

* Missing system boundary
* Missing actors
* Missing use cases
* Invalid relationships
* Duplicate elements
* Invalid source/target relationships
* Self-connections
* Unconnected elements
* Potentially incorrect relationship types
* Excessive unnecessary relationships

Example validation result:

```text
Diagram Validation
────────────────────────────

Score: 92 / 100

✓ Actors are valid
✓ Use cases are defined
✓ System boundary exists
✓ Relationships have valid endpoints
✓ No duplicate elements

⚠ 1 relationship requires review
```

---

# 🤖 AI + Rule Engine

One of the central architectural principles of DiagramWise is that AI-generated information should not automatically be considered correct.

The responsibilities are separated:

| Component        | Responsibility                          |
| ---------------- | --------------------------------------- |
| AI Service       | Understand natural-language scenarios   |
| Structure Engine | Build structured diagram representation |
| Rule Engine      | Validate diagram structure              |
| Layout Engine    | Arrange diagram elements                |
| Diagram Editor   | Allow manual modifications              |
| User             | Make final decisions                    |

This creates a more reliable workflow than simply asking an AI system to generate a diagram image.

### Generic AI approach

```text
Scenario
   ↓
AI
   ↓
Diagram Image
```

### DiagramWise approach

```text
Scenario
   ↓
AI
   ↓
Structured Diagram Model
   ↓
Validation Engine
   ↓
Layout Engine
   ↓
Editable Diagram
```

---

# 🧩 AI-Assisted Structure Analysis

AI is primarily responsible for **natural-language understanding**.

For example:

### Scenario

> "A customer places an order through an online pharmacy. The payment gateway processes the payment."

The AI can identify:

### Actors

```text
Customer
Payment Gateway
```

### Use Cases

```text
Place Order
Process Payment
```

### Relationship

```text
Customer → Place Order
Payment Gateway → Process Payment
```

The AI output can then be converted into structured JSON.

Example:

```json
{
  "actors": [
    {
      "id": "customer",
      "name": "Customer"
    }
  ],
  "useCases": [
    {
      "id": "place_order",
      "name": "Place Order"
    }
  ],
  "relationships": [
    {
      "source": "customer",
      "target": "place_order",
      "type": "association"
    }
  ]
}
```

Because the diagram is represented as structured data, it remains editable and reusable.

---

# 🔍 "Why Is This Here?" Feature

DiagramWise can provide explanations for individual elements and relationships.

For example, selecting:

```text
Payment Gateway
```

could display:

> **Why is this here?**

> Payment Gateway is represented as an external actor because it interacts with the pharmacy system while operating outside the system boundary.

Similarly, selecting:

```text
<<include>>
```

could provide an explanation of why the relationship was suggested.

This turns DiagramWise from simply being a diagram generator into an **educational diagramming assistant**.

---

# 💡 Suggested Corrections

DiagramWise should not silently modify user diagrams.

Instead, it can provide suggestions.

Example:

### Current Relationship

```text
Place Order ───── Make Payment
Association
```

### Suggested Relationship

```text
Place Order ───── <<include>> ───── Make Payment
```

### Reason

> Payment is described as a required part of completing the order, so an `include` relationship may be more appropriate.

The user can then choose:

```text
[ Apply Change ]     [ Keep Current ]
```

The final decision remains with the user.

---

# 🎓 Academic Mode

DiagramWise can provide a dedicated **Academic Mode** designed for students.

When enabled, the system can:

* Apply standard diagram notation
* Perform structural validation
* Explain relationships
* Highlight questionable structures
* Identify unnecessary elements
* Provide educational explanations
* Produce report-friendly exports

This mode makes DiagramWise particularly useful for academic assignments and practical sessions.

---

# 🎨 Interactive Diagram Editor

The editor is one of the most important parts of the application.

A generated diagram should never become a static image that users cannot modify.

The editor allows users to refine the AI-generated result.

### Example

AI generates:

```text
Place Order
```

The user decides the preferred terminology is:

```text
Submit Order
```

The user can simply select the element and rename it.

---

# 🔗 Relationship Editing

Users can select relationships and change their types where applicable.

Possible relationship types include:

```text
Association
Include
Extend
Generalization
Dependency
```

The application can provide contextual explanations for each relationship.

For example:

> **Include:** Used when one use case always requires another behavior as part of its execution.

---

# 📐 Automatic Layout

Generated diagrams should be visually organized.

The layout engine can automatically:

* Position elements
* Maintain spacing
* Align nodes
* Reduce line crossings
* Maintain hierarchy
* Organize actors
* Fit diagrams to the canvas

Possible layout options include:

```text
Balanced
Compact
Horizontal
Vertical
```

Users can still manually adjust the generated layout.

---

# 💾 Save and Version History

Since DiagramWise stores diagrams as structured data, users can save and reopen them without losing their underlying structure.

Example:

```text
Online Pharmacy System
Use Case Diagram
Status: Validated
Last Edited: Today
```

### Version history

```text
Version 1
Initial generated diagram

Version 2
Added Track Order

Version 3
Changed payment relationship
```

Users can potentially restore previous versions.

---

# 📚 Templates

DiagramWise can provide ready-made templates and scenarios.

Example templates:

* University Course Registration
* Library Management System
* Hospital Appointment System
* Online Pharmacy
* Food Delivery System
* Hotel Reservation System
* E-Commerce System
* Emergency Response System

Templates can help beginners understand how different diagram structures are created.

---

# 📤 Export

Completed diagrams can be exported in commonly used formats.

### Planned formats

* PNG
* SVG
* PDF

### Potential advanced formats

* Mermaid
* PlantUML
* Draw.io-compatible formats

PDF export is particularly useful for:

* University assignments
* Project reports
* Presentations
* Documentation

---

# 📊 Supported Diagram Types

DiagramWise is designed to support multiple software engineering and project management diagrams.

## UML Diagrams

* Use Case Diagram
* Activity Diagram
* Sequence Diagram
* Class Diagram
* State Machine Diagram
* Component Diagram
* Deployment Diagram

## Project Management

* Work Breakdown Structure (WBS)

### Recommended MVP

The first release should focus on:

1. Use Case Diagram
2. Activity Diagram
3. Sequence Diagram

Additional diagram types can be added after the core architecture becomes stable.

---

# 🔄 How DiagramWise Works

The complete workflow is:

```text
┌──────────────────────┐
│  Enter Scenario      │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Select Diagram Type  │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ AI Structure Analysis│
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Review Structure     │
│ Actors / Elements    │
│ Relationships        │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Generate Diagram     │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Rule-Based Validation│
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Interactive Editor   │
└──────────┬───────────┘
           ↓
     ┌─────┼─────┐
     ↓     ↓     ↓
   Edit Validate Explain
     │     │     │
     └─────┼─────┘
           ↓
┌──────────────────────┐
│ Save / Version /     │
│ Export               │
└──────────────────────┘
```

---

# 🏗️ System Architecture

```text
                         ┌───────────────┐
                         │     USER      │
                         └───────┬───────┘
                                 │
                                 ▼
                       ┌──────────────────┐
                       │  React Frontend  │
                       └────────┬─────────┘
                                │
              ┌─────────────────┼─────────────────┐
              │                 │                 │
              ▼                 ▼                 ▼
       ┌─────────────┐   ┌──────────────┐  ┌──────────────┐
       │   Diagram   │   │  Structure   │  │ Validation   │
       │   Editor    │   │  Analysis UI │  │     UI       │
       └──────┬──────┘   └──────┬───────┘  └──────┬───────┘
              │                 │                 │
              └─────────────────┼─────────────────┘
                                │
                                ▼
                       ┌─────────────────┐
                       │ Node/Express API│
                       └────────┬────────┘
                                │
             ┌──────────────────┼──────────────────┐
             │                  │                  │
             ▼                  ▼                  ▼
      ┌────────────┐     ┌────────────┐     ┌────────────┐
      │ AI Service │     │Rule Engine │     │  MongoDB   │
      └─────┬──────┘     └─────┬──────┘     └────────────┘
            │                  │
            └─────────┬────────┘
                      ▼
              ┌───────────────┐
              │ Diagram JSON  │
              └───────┬───────┘
                      ▼
              ┌───────────────┐
              │ Layout Engine │
              └───────┬───────┘
                      ▼
              ┌───────────────┐
              │ Editable      │
              │ Canvas        │
              └───────────────┘
```

---

# 🛠️ Technology Stack

| Layer             | Technology                 |
| ----------------- | -------------------------- |
| Frontend          | React                      |
| Build Tool        | Vite                       |
| Diagram Editor    | React Flow                 |
| Styling           | CSS / Tailwind CSS         |
| Backend           | Node.js                    |
| API Framework     | Express.js                 |
| Database          | MongoDB                    |
| AI                | Large Language Model API   |
| Authentication    | JWT                        |
| State Management  | React State / Zustand      |
| API Communication | Axios / Fetch              |
| Version Storage   | MongoDB                    |
| Source Control    | Git / GitHub               |
| Frontend Hosting  | Vercel                     |
| Backend Hosting   | Node.js-compatible hosting |

> The exact technologies may vary according to the implementation. The stack above represents the recommended architecture for DiagramWise.

---

# 📁 Project Structure

A recommended project structure is:

```text
DiagramWise/
│
├── frontend/
│   │
│   ├── public/
│   │
│   ├── src/
│   │   ├── components/
│   │   │   ├── layout/
│   │   │   ├── editor/
│   │   │   ├── nodes/
│   │   │   ├── edges/
│   │   │   └── modals/
│   │   │
│   │   ├── pages/
│   │   │   ├── Dashboard.jsx
│   │   │   ├── CreateDiagram.jsx
│   │   │   ├── StructureAnalysis.jsx
│   │   │   ├── DiagramEditor.jsx
│   │   │   ├── MyDiagrams.jsx
│   │   │   └── Templates.jsx
│   │   │
│   │   ├── services/
│   │   │   ├── api.js
│   │   │   ├── diagramService.js
│   │   │   └── aiService.js
│   │   │
│   │   ├── utils/
│   │   │   ├── validation.js
│   │   │   ├── layout.js
│   │   │   └── diagramParser.js
│   │   │
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
├── backend/
│   │
│   ├── controllers/
│   │   ├── diagramController.js
│   │   ├── aiController.js
│   │   └── authController.js
│   │
│   ├── models/
│   │   ├── User.js
│   │   ├── Diagram.js
│   │   ├── DiagramVersion.js
│   │   └── Template.js
│   │
│   ├── routes/
│   │   ├── diagramRoutes.js
│   │   ├── aiRoutes.js
│   │   └── authRoutes.js
│   │
│   ├── services/
│   │   ├── aiService.js
│   │   ├── validationService.js
│   │   └── layoutService.js
│   │
│   ├── middleware/
│   │   └── authMiddleware.js
│   │
│   ├── config/
│   │   └── db.js
│   │
│   ├── server.js
│   └── package.json
│
├── .gitignore
├── README.md
└── LICENSE
```

---

# 🗄️ Database Design

## User Collection

```text
User
├── _id
├── name
├── email
├── password
└── createdAt
```

---

## Diagram Collection

```text
Diagram
├── _id
├── userId
├── name
├── type
├── scenario
├── nodes
├── edges
├── validation
├── createdAt
└── updatedAt
```

---

## Diagram Version Collection

```text
DiagramVersion
├── _id
├── diagramId
├── versionNumber
├── nodes
├── edges
├── changeDescription
└── createdAt
```

---

## Template Collection

```text
Template
├── _id
├── name
├── type
├── description
├── nodes
└── edges
```

---

# 🧩 Core Diagram Data Model

A diagram is represented as structured data rather than a static image.

```text
Diagram
│
├── Metadata
│   ├── Name
│   ├── Type
│   └── Scenario
│
├── Nodes
│   ├── Actor
│   ├── Use Case
│   ├── Entity
│   └── System Boundary
│
└── Edges
    ├── Association
    ├── Include
    ├── Extend
    ├── Generalization
    └── Dependency
```

This enables the same diagram to be:

```text
Generated
   ↓
Edited
   ↓
Validated
   ↓
Saved
   ↓
Reopened
   ↓
Modified
   ↓
Exported
```

without losing its underlying structure.

---

# ⚙️ Installation

## Prerequisites

Before installing DiagramWise, ensure that the following are available:

* Node.js
* npm
* MongoDB or MongoDB Atlas
* Git
* A supported AI API account/key

Verify Node.js:

```bash
node --version
```

Verify npm:

```bash
npm --version
```

Verify Git:

```bash
git --version
```

---

# 📥 Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
```

Navigate into the project:

```bash
cd DiagramWise
```

---

# 📦 Install Frontend Dependencies

```bash
cd frontend
npm install
```

---

# 📦 Install Backend Dependencies

Open another terminal:

```bash
cd backend
npm install
```

---

# 🔐 Environment Variables

Create a `.env` file inside the backend directory.

Example:

```env
PORT=5000

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

AI_API_KEY=your_ai_api_key
```

### Important

Do **not** commit `.env` files to GitHub.

Add the following to `.gitignore`:

```text
.env
.env.local
node_modules/
dist/
```

---

# ▶️ Running the Project

## Start Backend

Inside the `backend` directory:

```bash
npm run dev
```

or, depending on the configured scripts:

```bash
npm start
```

The backend should run on a local port such as:

```text
http://localhost:5000
```

---

## Start Frontend

Inside the `frontend` directory:

```bash
npm run dev
```

The Vite development server will provide a local URL such as:

```text
http://localhost:5173
```

Open the displayed URL in your browser.

---

# 🖥️ Using DiagramWise

## Step 1 — Create a Diagram

Select:

```text
Create Diagram
```

---

## Step 2 — Select Diagram Type

Choose a diagram type.

For example:

```text
Use Case Diagram
```

---

## Step 3 — Enter Scenario

Enter a natural-language description.

Example:

```text
A university student logs into the registration system,
selects courses and submits registration. The system checks
prerequisites and seat availability before confirming the
registration.
```

---

## Step 4 — Analyze Scenario

DiagramWise analyzes the scenario and identifies:

```text
Actors
Use Cases
Relationships
External Systems
```

---

## Step 5 — Review Structure

The user reviews the extracted information.

For example:

```text
Actors

✓ Student

Use Cases

✓ Login
✓ Select Courses
✓ Submit Registration
✓ Check Prerequisites
✓ Check Seat Availability
✓ Confirm Registration
```

The user can:

```text
[ Add ]
[ Edit ]
[ Delete ]
```

elements before generation.

---

## Step 6 — Generate Diagram

After approving the structure:

```text
Generate Diagram
```

DiagramWise creates the editable diagram.

---

## Step 7 — Validate

The rule engine checks the diagram.

Example:

```text
✓ System boundary exists
✓ Actor relationships are valid
✓ No duplicate nodes

⚠ One relationship requires review
```

---

## Step 8 — Edit

Users can modify the diagram manually.

---

## Step 9 — Explain

Users can select elements and relationships to understand why they were included.

---

## Step 10 — Save and Export

The final diagram can be saved and exported.

---

# 🧪 Example

Consider the following scenario:

> "An online pharmacy allows customers to register and log in, search medicines, view medicine details, add medicines to a cart, place orders, make payments, and track orders. Pharmacists can manage medicine information and update stock. Administrators can manage users and monitor orders. The system uses an external payment gateway to process payments."

DiagramWise may extract:

### Actors

```text
Customer
Pharmacist
Administrator
Payment Gateway
```

### Use Cases

```text
Register
Login
Search Medicines
View Medicine Details
Add to Cart
Place Order
Make Payment
Track Order
Manage Medicines
Update Stock
Manage Users
Monitor Orders
```

### Relationships

```text
Customer ───── Search Medicines
Customer ───── Place Order
Customer ───── Track Order

Place Order ─── <<include>> ─── Make Payment

Pharmacist ───── Manage Medicines
Pharmacist ───── Update Stock

Administrator ── Manage Users
Administrator ── Monitor Orders

Payment Gateway ── Make Payment
```

The user can then review, modify, validate, and generate the final diagram.

---

# 🔌 API Overview

The backend can expose RESTful API endpoints such as:

## Authentication

```text
POST /api/auth/register
POST /api/auth/login
GET  /api/auth/me
```

---

## Diagram Management

```text
GET    /api/diagrams
GET    /api/diagrams/:id
POST   /api/diagrams
PUT    /api/diagrams/:id
DELETE /api/diagrams/:id
```

---

## AI Analysis

```text
POST /api/ai/analyze
POST /api/ai/generate
POST /api/ai/explain
```

---

## Validation

```text
POST /api/validation/validate
POST /api/validation/suggestions
```

---

## Version History

```text
GET  /api/diagrams/:id/versions
POST /api/diagrams/:id/versions
GET  /api/diagrams/:id/versions/:versionId
```

> The exact endpoint names should match the implementation in the backend.

---

# 🔎 Validation Workflow

The validation process can follow this architecture:

```text
                    Diagram
                       │
                       ▼
               ┌───────────────┐
               │   Validator   │
               └───────┬───────┘
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
      Structure    Relations     Elements
       Checks        Checks        Checks
          │            │            │
          └────────────┼────────────┘
                       ▼
                Validation Result
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
          Valid                Issues
                                 │
                                 ▼
                           Suggestions
```

The validator should provide useful feedback rather than simply returning:

```text
Invalid
```

Instead:

```text
Issue:
Payment relationship may require review.

Reason:
The scenario describes payment as a required part of placing
the order.

Suggested action:
Consider an <<include>> relationship.
```

---

# 🚀 Development Roadmap

## Phase 1 — Foundation

* Set up React/Vite
* Set up Node.js/Express
* Connect MongoDB
* Create application layout
* Configure routing
* Establish frontend/backend communication

### Milestone

Basic DiagramWise application is operational.

---

## Phase 2 — Diagram Editor

Implement:

* Actor
* Use Case
* System Boundary
* Relationships
* Dragging
* Selection
* Editing
* Delete
* Zoom/pan
* Undo/redo

### Milestone

> Users can manually create a Use Case Diagram.

---

## Phase 3 — AI Structure Analysis

Implement:

```text
Scenario
   ↓
AI
   ↓
Actors
   ↓
Use Cases
   ↓
Relationships
```

Allow users to review and modify the generated structure.

---

## Phase 4 — Automatic Generation

Convert:

```text
Structured JSON
      ↓
Diagram Nodes
      ↓
Diagram Edges
      ↓
Layout
      ↓
Interactive Canvas
```

### Milestone

> Scenario → Editable Diagram

---

## Phase 5 — Validation

Implement:

* Structural rules
* Relationship validation
* Missing-element detection
* Duplicate detection
* Invalid connection detection
* Unconnected element detection
* Validation score

---

## Phase 6 — Explanation

Implement:

* Explain element
* Explain relationship
* Why is this here?
* Show explanation on diagram
* Suggested corrections

---

## Phase 7 — Persistence

Implement:

* Save diagrams
* My Diagrams
* Templates
* Version history
* Restore previous versions

---

## Phase 8 — Export

Implement:

* PNG
* SVG
* PDF

---

## Phase 9 — Additional Diagram Types

Expand support to:

```text
Use Case
   ↓
Activity
   ↓
Sequence
   ↓
Class
   ↓
State
   ↓
Component
   ↓
Deployment
   ↓
WBS
```

---

# 🎯 MVP Scope

The project should not attempt to implement every diagram type immediately.

The recommended MVP is:

```text
                  DiagramWise MVP
                        │
                        ▼
                 Enter Scenario
                        │
                        ▼
                Select Use Case
                        │
                        ▼
              AI Structure Analysis
                        │
                        ▼
             Review / Modify Structure
                        │
                        ▼
                 Generate Diagram
                        │
                        ▼
                Diagram Editor
                        │
              ┌─────────┼─────────┐
              ▼         ▼         ▼
            Edit     Validate   Explain
              │         │         │
              └─────────┼─────────┘
                        ▼
                      Save
                        │
                        ▼
                     Export
```

### MVP should focus on quality rather than quantity.

A strong implementation of:

* Use Case Diagram
* AI structure extraction
* Editing
* Validation
* Explanation
* Save
* Export

is more valuable than seven poorly implemented diagram types.

---

# 🔮 Future Enhancements

Potential future features include:

## More Diagram Types

* Class Diagram
* Activity Diagram
* Sequence Diagram
* State Diagram
* Component Diagram
* Deployment Diagram
* WBS
* BPMN

---

## Collaboration

Future versions could allow multiple users to work on the same diagram.

Potential features:

* Real-time collaboration
* Comments
* Mentions
* Shared workspaces
* Permission management

---

## AI Improvements

Potential enhancements:

* Better scenario understanding
* Context-aware suggestions
* Diagram quality scoring
* Automatic simplification
* Ambiguity detection
* Alternative diagram suggestions
* Multi-diagram generation from one scenario

---

## Educational Features

Potential features include:

* Interactive UML tutorials
* Diagram quizzes
* Practice scenarios
* Relationship explanations
* Student progress tracking
* Academic assessment mode

---

## Advanced Export

Potential support:

* Mermaid
* PlantUML
* Draw.io
* SVG
* PDF
* PNG

---

# 🔐 Security Considerations

DiagramWise should follow standard web application security practices.

Important considerations include:

* Password hashing
* JWT-based authentication
* Protected API routes
* Input validation
* API request validation
* Environment variable protection
* Secure AI API key storage
* CORS configuration
* Rate limiting
* Protection against unauthorized diagram access
* Sanitization of user-generated content

Sensitive credentials should never be stored directly in frontend code or committed to GitHub.

---

# 🧪 Testing

Testing should cover multiple layers of the application.

## Unit Testing

Test:

* Validation rules
* Data transformations
* Diagram parsing
* Relationship logic
* Utility functions

---

## API Testing

Test:

* Authentication
* Diagram creation
* Diagram retrieval
* Diagram updating
* Diagram deletion
* AI analysis
* Validation endpoints

---

## Frontend Testing

Test:

* Diagram creation
* Node editing
* Edge creation
* Dragging
* Undo/redo
* Save operations
* Validation display
* Export functionality

---

## User Acceptance Testing

Students and potential users can evaluate:

* Ease of use
* Accuracy
* Diagram clarity
* Editing experience
* AI usefulness
* Validation usefulness
* Explanation quality

---

# 🌟 What Makes DiagramWise Different?

DiagramWise is not simply another AI diagram generator.

### Traditional Diagramming Tool

```text
User understands diagram
        ↓
User manually draws
        ↓
User validates manually
```

### Generic AI Diagram Generator

```text
User enters scenario
        ↓
AI generates diagram
        ↓
User hopes it is correct
```

### DiagramWise

```text
User enters scenario
        ↓
AI analyzes scenario
        ↓
System extracts structure
        ↓
User reviews structure
        ↓
Diagram generated
        ↓
Rule engine validates
        ↓
User edits diagram
        ↓
System validates again
        ↓
System explains decisions
        ↓
User approves final result
        ↓
Save / Export
```

The key difference is:

> **DiagramWise combines AI assistance with structured representation, rule-based validation, interactive editing, and educational explanation.**

---

# 💎 Unique Value Proposition

### Full Version

> **DiagramWise transforms natural-language scenarios into editable, standards-aware diagrams while helping users understand, validate, and refine the structure behind them.**

### Short Version

> **An AI-assisted platform for generating, editing, explaining, and validating software engineering diagrams.**

### Portfolio Version

> **DiagramWise is an intelligent diagramming platform that converts natural-language requirements into editable diagrams and combines AI-assisted generation with rule-based validation and interactive editing.**

---

# 🏆 Project Significance

DiagramWise demonstrates the integration of several important areas of software engineering and information systems.

## UI/UX

The project demonstrates:

* User research
* Problem identification
* User flows
* Information architecture
* Wireframing
* High-fidelity UI design
* Interaction design
* Complex editor UX
* Usability testing
* Design systems

---

## Frontend Development

The project demonstrates:

* React
* Vite
* State management
* Interactive canvas development
* Drag-and-drop interactions
* API integration
* Complex UI components
* Diagram visualization

---

## Backend Development

The project demonstrates:

* Node.js
* Express
* REST API development
* MongoDB
* Database modeling
* Authentication
* Data persistence

---

## Artificial Intelligence

The project demonstrates:

* Natural-language processing
* LLM integration
* Prompt engineering
* Structured AI output
* AI-assisted decision making
* Human-in-the-loop AI

---

## Software Engineering

The project demonstrates:

* UML concepts
* Graph-based structures
* Rule-based validation
* Layout algorithms
* Version management
* System architecture
* API design
* Modular software development

---

# 👩‍💻 Development Philosophy

DiagramWise follows a **human-in-the-loop** approach.

The application does not attempt to completely replace the user's decision-making.

Instead:

```text
             AI
              │
              │ Suggestions
              ▼
           USER
              │
              │ Decisions
              ▼
           SYSTEM
              │
              │ Validation
              ▼
        FINAL DIAGRAM
```

This ensures that the user remains responsible for the final diagram while receiving intelligent assistance throughout the process.

---

# 🤝 Contributing

Contributions are welcome.

To contribute:

### 1. Fork the repository

```bash
git fork <repository>
```

### 2. Clone your fork

```bash
git clone <your-fork-url>
```

### 3. Create a feature branch

```bash
git checkout -b feature/your-feature
```

### 4. Make your changes

Implement and test your changes.

### 5. Commit

```bash
git add .
git commit -m "Add: your feature"
```

### 6. Push

```bash
git push origin feature/your-feature
```

### 7. Create a Pull Request

Submit a pull request describing:

* What was changed
* Why it was changed
* How it was tested


---

# 👩‍💻 Author

**DiagramWise**

### Intelligent Diagram Generation, Editing & Validation Platform

Developed as a software engineering / information systems project.

---

# ⭐ Final Project Vision

DiagramWise aims to make diagram creation less complicated by changing the way users approach diagramming.

Instead of starting with:

> **"How do I draw this diagram?"**

users can start with:

> **"Let me explain my scenario."**

DiagramWise then helps them:

```text
Understand
    ↓
Structure
    ↓
Generate
    ↓
Validate
    ↓
Edit
    ↓
Explain
    ↓
Export
```

The ultimate goal is to create a platform where users do not simply receive a diagram, but **understand the structure behind the diagram and remain in control of the final result.**

---

## 🚀 DiagramWise

> **Think it. Structure it. Validate it. Diagram it.**
