# Project Pitch (Task Tracker)
**To**: Dr. Jeffry Babb

**From**: Toluwani D. Adeoti

**Date**: 9/13/2025

**Subject**: Project Pitch – Accessible AI-Enhanced Task Tracker

## Part A (Project Pitch)
### 1. Problem Statement
Students and early-career professionals often face multiple competing responsibilities, including coursework, job obligations, and personal projects. Managing these tasks efficiently requires tools that are both simple to use and reliable. While numerous project management platforms exist—such as Jira, Trello, and Asana—these systems are often feature-rich and complex, presenting steep learning curves that can deter users seeking lightweight task tracking. Moreover, many of these platforms do not consistently implement accessibility standards, making them less inclusive for users with disabilities.

Additionally, the rise of AI in productivity tools has introduced both opportunities and challenges. AI can assist in task prioritization and summarization, but transparency in AI outputs is limited in most existing solutions. Users rarely know how AI recommendations are generated or whether they are influenced by biases in underlying data. As a result, there is a need for a task tracking solution that is lightweight, accessible, and AI-transparent, balancing usability with ethical considerations.

The proposed solution is a minimal Django-based Task Tracker. This system allows users to create, read, update, and delete tasks, optionally including metadata such as due date, priority, and completion status. To demonstrate the potential of AI augmentation, the system includes an optional feature that generates short task summaries or priority recommendations. All AI prompts and outputs are logged to ensure full transparency, providing a model for responsible AI usage within productivity applications.
### 2. Stakeholders
-	Primary Users: Students and early-career professionals seeking a simple, distraction-free task tracking experience. They require a system that is intuitive and minimally intrusive.
-	Secondary Users: Instructors, team leads, and accessibility reviewers who evaluate usability, user experience, and compliance with accessibility standards.
-	Other Stakeholders:
	-	IT administrators, responsible for deployment and ongoing maintenance of the application.
	-	Ethics reviewers, tasked with evaluating AI transparency and potential misuse.
	-	Accessibility advocates, ensuring compliance with WCAG 2.2 and promoting inclusive design principles.
Engaging these stakeholders throughout development ensures that the system meets both functional and ethical requirements while remaining practical for end users.
### 3. Scope & Minimal Viable Artifact (2 Weeks)
The project is scoped to a 2-week minimal viable artifact (MVP) that delivers core functionality while maintaining professional quality and accessibility. The MVP includes:
-	CRUD Functionality: Users can create, read, update, and delete tasks, including task title, description, due date, and completion status.
-	Front-End Interface: A simple web interface using Django templates provides an intuitive, responsive layout.
-	Accessibility Baseline: Implementation of alt text, ARIA roles, and a high-contrast visual style ensures compliance with basic accessibility guidelines.
-	AI Feature (Optional): Users can generate short task summaries or priority suggestions. All AI interactions are logged to ensure transparency and accountability.
-	Documentation: GitHub repository with README, AI disclosure log, and a system sketch diagram to support understanding and reproducibility.
This scope prioritizes feasibility, usability, and ethical AI integration, allowing the team to deliver a functional and testable artifact within the two-week window.
### 4. Success Metrics
To evaluate the MVP, the following criteria will be measured:
1.	Users can successfully create, edit, delete, and view tasks without encountering errors.
2.	The system passes WCAG 2.2 quick accessibility checks, including contrast, alt text, and ARIA labeling.
3.	AI features are optional, clearly documented, and logged for full transparency.
4.	Project artifacts—including the GitHub repository, documentation, and exported PDF memo—meet professional standards for clarity, completeness, and organization.
Meeting these metrics demonstrates that the MVP satisfies both functional and ethical requirements, providing a foundation for future development or feature expansion.
### 5. System Sketch
The system follows a straightforward architecture:
Flow:
Frontend (Django templates) → Backend (Django views) → Database (SQLite, Tasks table) → Optional AI service → Logged interactions (for transparency)
-	Frontend: Provides forms and interfaces for task CRUD operations.
-	Backend: Processes requests, applies business logic, and manages communication with the database and AI service.
-	Database: Stores tasks and metadata, ensuring persistent state.
-	AI Service: Optionally processes task data to provide summaries or prioritization suggestions.
-	Logging: Captures AI outputs and user interactions to maintain accountability and transparency. 
### 6. Evidence Base
1.	McKinsey & Company. (2023). The rise of lightweight productivity tools: Digital adoption trends in the modern workforce. McKinsey & Company. https://www.mckinsey.com
2.	National Institute of Standards and Technology. (2023). Artificial Intelligence Risk Management Framework (AI RMF 1.0). U.S. Department of Commerce. https://www.nist.gov/ai-risk-management
3.	World Wide Web Consortium (W3C). (2023). Web Content Accessibility Guidelines (WCAG) 2.2. https://www.w3.org/WAI/WCAG22/
These sources provide empirical support for lightweight, accessible productivity tools and guidelines for ethical AI implementation.
### 7. Risk Register
Risk	Likelihood	Impact	Mitigation
Scope creep (adding too many features)	Medium	High	Freeze MVP to CRUD + one AI feature to maintain timeline feasibility
Accessibility gaps	Medium	Medium	Test with WCAG 2.2 quick checks; review with a screen reader to ensure compliance
AI misuse/privacy	Medium	High	Use only demo/synthetic data; disclose all AI outputs in logs for transparency
Proactively addressing these risks ensures that the system remains functional, accessible, and ethically sound while staying within the two-week project timeline.

 

