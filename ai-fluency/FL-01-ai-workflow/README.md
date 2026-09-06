# Assignment FL-01: AI Workflow Audit & Tool Setup

**Track:** General AI Fluency  
**Phase:** Onboarding (Week 1)  

---

## 1. Workflow Audit Table

| Task | Classification | One-Line Rationale |
| :--- | :--- | :--- |
| Writing core backend architecture logic | Just me | High-stakes trade-offs and structural choices require deep context and human system design intuition. |
| Making final security decisions & credential handling | Just me | Critical security policies cannot rely on AI assumptions; human oversight is mandatory. |
| Formatting and linting Python code | Fully automate | Deterministic, rules-based tasks are best handled by pre-commit hooks, Black, and Flake8. |
| Writing unit test boilerplate and edge cases | Delegate to AI with review | Saves repetitive setup time, but generated assertions require human review for accuracy. |
| Summarizing technical documentation/ whitepapers | Collaborate with AI | AI rapidly extracts key concepts, while I cross-examine API constraints and ask follow-up questions. |
| Drafting initial API endpoint code from spec | Delegate to AI with review | Speeds up boilerplate generation (FastAPI models/routes), but code needs manual performance checks. |
| Writing weekly project status updates | Delegate to AI with review | AI formats raw bullet points into readable updates, which I review for accuracy before sharing. |
| Debugging complex runtime errors & stack traces | Collaborate with AI | AI helps brainstorm potential root causes, while I step through code and test fix hypotheses. |
| Planning weekly study and project milestones | Collaborate with AI | AI suggests balanced schedules based on my goals, which I tweak for realistic execution. |
| Extracting action items from lecture notes | Delegate to AI with review | Quickly distills dense markdown notes into actionable tasks that I review and refine. |
| Explaining complex algorithms to peers | Collaborate with AI | AI assists in generating analogies, which I adapt to fit my peer's technical background. |
| Setting up Docker container configs | Delegate to AI with review | AI generates baseline Dockerfiles/compose files, which I tune for environment variables and security. |

---

## 2. Target Tasks & Success Definitions

### Task 1: Drafting Initial REST API Endpoint Boilerplate (FastAPI)
* **Description:** Generating initial route definitions, request/response models (Pydantic), and controller stubs from a specification.
* **Success Definition ("Done Well"):** The generated code runs without syntax errors, includes type hints, implements correct HTTP status codes (200, 400, 404, 500), and requires under 5 minutes of manual adjustments.

### Task 2: Writing Unit Tests for Business Logic Functions
* **Description:** Generating pytest test suites for backend logic modules.
* **Success Definition ("Done Well"):** Generates comprehensive pytest cases covering happy paths, boundary conditions, and edge cases, achieving over 85% line coverage with zero failing test executions on first run.

### Task 3: Summarizing Technical Documentation / API Specs
* **Description:** Extracting setup instructions, rate limits, and key endpoints from multi-page API documentation.
* **Success Definition ("Done Well"):** Distills documentation into a concise 1-page summary covering authentication requirements, base URLs, key endpoints, rate limits, and error formats without omitting critical technical constraints.

---

## 3. Toolkit Setup & Verification

* **ChatGPT Account:** Created & active.
* **Claude Account:** Created & active.
* **Anthropic Academy Account:** Created & enrolled in *AI Fluency: Framework & Foundations* (Module 1 completed).

### Claude Project Configuration

**Project Name:** `FlyRank Backend & AI Engineering`

**Custom Instructions:**
> "I am a backend and AI engineering intern working on high-performance web applications and systems. 
> 
> Preferred Tone & Style:
> - Direct, concise, and technical.
> - Prioritize clean Python (FastAPI/Pytest) with type hints and explicit error handling.
> - Minimize conversational fluff; jump straight to code or structured technical explanations.
> - Highlight trade-offs and edge cases explicitly."

---