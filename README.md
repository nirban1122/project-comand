# 📑 MASTER PROMPT ARCHITECTURE: GERMAN LEARNING APP
This master document compiles your entire phase-by-phase development



# MAIN ARCHITECTURE OF THIS PROJECT:
┌────────────────────────────────────────┐
│                                               │
│  CLAUDE (Main) - Architecture + Full Code     │
│  "You are here" - Primary coder for full-stack│
│                                               │
├─────────────────────────────────────── ┤
│                                               │
│  GEMINI - Brainstorming + Alternatives        │
│  Quick ideas, features, testing strategies    │
│                                               │
├───────────────────────────────────—────┤
│                                               │
│  V0.DEV - UI Components                       │
│  Beautiful React components with Shadcn/UI    │
│                                               │
├────────────────────────────────────────┤
│                                               │
│  GitHub Copilot - Real-time Code Assist (Optional) │
│  In-editor suggestions while you code         │
│                                               │
└────────────────────────────────────────┘



## 🏗️ PHASE 0: Project Setup & Architecture
### 📄 File Reference
PHASE ( 0 )Project Setup & Architecture/1.MAIN ARCHITECTURE.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Principal Software Architect         │
│                                      │
│ TASK:                                │
│ Define a comprehensive technical     │
│ architecture blueprint for a full-   │
│ stack German language learning       │
│ platform.                            │
│                                      │
│ SYSTEM REQUIREMENTS:                 │
│ 1. User onboarding infrastructure    │
│ 2. Structured video/text lessons     │
│ 3. Interactive grammar exercises     │
│ 4. Real-time feedback loops          │
│ 5. Progress tracking dashboards      │
│ 6. Scalable, secure API routing      │
│                                      │
│ EXPECTED OUTPUTS:                    │
│ * Definitive tech stack selections   │
│ * Global monorepo structures         │
│ * Code splitting parameters          │
│ * Environment variable structures    │
│ * State management architecture      │
│   optimized for ultra-low latency    │
│   client response profiles           │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 0 )Project Setup & Architecture/2.initialsetup(claude).md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Senior DevOps Engineer               │
│                                      │
│ TASK:                                │
│ Generate a precise initialization    │
│ script and structural deployment     │
│ guide using the baseline technical   │
│ architecture design.                 │
│                                      │
│ SYSTEM REQUIREMENTS:                 │
│ 1. Initialize backend server space   │
│ 2. Initialize frontend workspace     │
│ 3. Configure root dependencies       │
│                                      │
│ CONFIGURATIONS TO INCLUDE:           │
│ * TypeScript (tsconfig.json)         │
│ * ESLint & Prettier rules            │
│ * EditorConfig specifications        │
│ * Tailwind CSS theme setups          │
│ * Initial environment variable       │
│   injection hooks                    │
│                                      │
│ VALIDATION CRITERIA:                 │
│ Code must compile with zero warnings │
│ and strict typing patterns.          │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 0 )Project Setup & Architecture/3.Db Schema (Claude).md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Lead Database Administrator          │
│                                      │
│ TASK:                                │
│ Write a production-ready relational  │
│ schema model for the German learning │
│ platform using modern ORM syntax.    │
│                                      │
│ TARGET DATA TABLES:                  │
│ 1. Users & Profiles                  │
│ 2. UserProgress & AuditLogs          │
│ 3. Courses, Modules & Lessons        │
│ 4. Exercises & Submissions           │
│ 5. Quizzes                           │
│                                      │
│ SCHEMA REQUIREMENTS:                 │
│ * Explicit table relationships       │
│ * Primary & foreign key mappings     │
│ * Performance-tuned indexes          │
│ * Strict cascade constraints         │
│ * Data integrity & type safety       │
│ * Initial migration configurations   │
└──────────────────────────────────────┘

```
## 🔐 PHASE 1: Authentication System
### 📄 File Reference
PHASE ( 1) Authentication System/1.Auth sys(Claude).md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Senior Security Engineer             │
│                                      │
│ TASK:                                │
│ Build a robust backend and frontend  │
│ user authentication flow.            │
│                                      │
│ CORE FEATURES:                       │
│ 1. Secure registration pipeline      │
│ 2. Secure login infrastructure       │
│ 3. Token lifecycle management        │
│                                      │
│ SECURITY PROTOCOLS:                  │
│ * Secure JWT architecture            │
│ * HTTP-only cookie storage or        │
│   encrypted local storage sets       │
│ * Role-Based Access Control (RBAC)   │
│   middleware (Admin vs Student)      │
│ * Inputs sanitation layers           │
│ * Salted password hashing logic      │
│ * Validation payload schemas         │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 1) Authentication System/2.AUTH TEST AND SECURITY(Claude).md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ QA Security Tester                   │
│                                      │
│ TASK:                                │
│ Write an automated integration and   │
│ unit test suite to stress-test the   │
│ authentication system layer.         │
│                                      │
│ VULNERABILITY TARGETS:               │
│ 1. Malformed/invalid JWT structures  │
│ 2. Token expiration edge cases       │
│ 3. Brute-force entry attempts        │
│ 4. XSS scripts via inputs            │
│ 5. SQL/NoSQL injections              │
│                                      │
│ VALIDATION CRITERIA:                 │
│ Assert correct failure codes, error  │
│ responses, and payload response      │
│ schemas across all scenarios.        │
└──────────────────────────────────────┘

```
## 📚 PHASE 2: Courses & Lessons System
### 📄 File Reference
PHASE ( 2 ) Courses & Lessons/1.Courses Backend.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Senior Backend Developer             │
│                                      │
│ TASK:                                │
│ Develop high-performance relational  │
│ API endpoints for the educational    │
│ routing architecture.                │
│                                      │
│ ARCHITECTURE PATHWAY:                │
│ Courses ➔ Levels (A1/A2/B1) ➔        │
│ Modules ➔ Lessons                    │
│                                      │
│ LOGIC REQUIRED:                      │
│ * Paginated data query controllers   │
│ * User progress tracking flags       │
│ * Lesson status maps (Completed/     │
│   In-Progress/Locked)                │
│ * Full administrative CRUD routes    │
│   for dynamic content creation       │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 2 ) Courses & Lessons/2.Lessons System.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Frontend Engineer                    │
│                                      │
│ TASK:                                │
│ Create an immersive, component-      │
│ driven user interface for the main   │
│ Lesson View screen.                  │
│                                      │
│ RENDER CAPABILITIES:                 │
│ 1. Rich text descriptions            │
│ 2. Embedded Markdown engines         │
│ 3. Native audio players (for pronunciation)│
│ 4. Video media playback boxes        │
│ 5. Vocabulary glossary definitions   │
│                                      │
│ APPLICATION STATE LOGIC:             │
│ Build immediate, persistent client-  │
│ to-server sync hooks that save progress│
│ whenever a user finishes a module.   │
└──────────────────────────────────────┘

```
## 📝 PHASE 3: Exercises & Quizzes
### 📄 File Reference
PHASE ( 3 ) Exercises & Quizzes/1.Exercise System.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Educational UX Developer             │
│                                      │
│ TASK:                                │
│ Build an interactive exercise engine │
│ optimized for language retention.    │
│                                      │
│ EXERCISE VARIATIONS:                 │
│ 1. Standard Multiple Choice (MCQ)    │
│ 2. Fill-in-the-Blanks text entry     │
│ 3. Interactive word reordering drag- │
│    and-drop block interfaces         │
│                                      │
│ UI EVALUATION FEEDBACK:              │
│ * Instant state changes (Success-    │
│   Green / Error-Red graphics)        │
│ * Inline context tooltips displaying │
│   grammatical corrections upon fault │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 3 ) Exercises & Quizzes/2.Quiz System.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Core Logic Systems Engineer          │
│                                      │
│ TASK:                                │
│ Engineer a high-stakes, time-boxed   │
│ Module Quiz System.                  │
│                                      │
│ SYSTEM SPECIFICATIONS:               │
│ 1. Secure client countdown timers    │
│ 2. Server-side validation tickers    │
│ 3. Live quiz progress caching        │
│ 4. Strict step submission engines    │
│ 5. Auto-grading database script      │
│                                      │
│ FINAL MATRIX GENERATION:             │
│ Compute precise final scores, run-   │
│ time duration logs, and output a     │
│ granular database assessment card.   │
└──────────────────────────────────────┘

```
## 📊 PHASE 4: Dashboard & User Profiles
### 📄 File Reference
PHASE ( 4 ) Dashboard & User Profile/1.Dashboard System.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Full-Stack Product Developer         │
│                                      │
│ TASK:                                │
│ Build the primary student activity   │
│ and tracking dashboard system.       │
│                                      │
│ DATA INTERFACES TO RENDER:           │
│ 1. Overall progress percentages      │
│ 2. Daily check-in streak counters    │
│ 3. Total complete lesson summaries   │
│ 4. Interactive contribution activity │
│    heatmap timeline grids            │
│                                      │
│ SPEED REQUIREMENT:                   │
│ Implement aggressive backend caching │
│ layers to ensure page initialization │
│ runs with low server-side loads.     │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 4 ) Dashboard & User Profile/2.User Profile.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ UI Layout Specialist                 │
│                                      │
│ TASK:                                │
│ Create the main interactive settings │
│ panel and user profile manager.      │
│                                      │
│ CONTROL BLOCKS REQUIRED:             │
│ 1. Profile information modifiers     │
│    (Avatars, text tags, emails)      │
│ 2. Language target threshold updates │
│ 3. App-wide light/dark mode triggers │
│ 4. Core account self-service flags   │
│    (Password resets, wiping files)   │
│                                      │
│ DATA REUREMENT:                      │
│ Wire all interaction fields directly │
│ to secure database mutation loops.   │
└──────────────────────────────────────┘

```
## 🚀 PHASE 5: Deployment & Optimization
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/1.Deploy to Render.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Infrastructure Specialist            │
│                                      │
│ TASK:                                │
│ Write declarative configurations,    │
│ deployment manifests, and system      │
│ parameters to host the app on Render.│
│                                      │
│ DELIVERABLES:                        │
│ * Production shell build commands    │
│ * Start-up package script controls   │
│ * Port reverse proxy routing rules   │
│ * Multi-cluster memory allocation    │
│ * Automated API health check routes  │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/2.Performance & Optimization.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Web Performance Engineer             │
│                                      │
│ TASK:                                │
│ Audit, trace, and speed-optimize     │
│ all global runtime paths.            │
│                                      │
│ TACTICS TO IMPLEMENT:                │
│ 1. Asset compression protocols       │
│ 2. Dynamic client-side code splitting │
│ 3. Component lazy-loading wrappers   │
│ 4. Global browser data caching       │
│ 5. DB connection pooling models      │
│                                      │
│ OBJECTIVE:                           │
│ Minimize Time-to-First-Byte (TTFB)   │
│ to guarantee high speed on mobile.   │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/3.Error Handling & Logging.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ Site Reliability Engineer (SRE)      │
│                                      │
│ TASK:                                │
│ Engineer a comprehensive, centralized │
│ runtime exception catching system.   │
│                                      │
│ ARCHITECTURAL CORES:                 │
│ 1. Unified try-catch wrapper logic   │
│ 2. Custom typed application faults   │
│ 3. Production terminal log formatters│
│ 4. Client error UI fallback boundaries│
│                                      │
│ CONSTRAINT:                          │
│ Never expose raw server stack traces │
│ or infrastructure directories to the │
│ end-user application logs.           │
└──────────────────────────────────────┘

```
## 🎨 PHASE 6: UI Components
### 📄 File Reference
PHASE ( 6 ) UI Components (V0.DEV)/Beautiful UI Components.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ UI/UX Prompt Engineer (v0.dev Expert)│
│                                      │
│ TASK:                                │
│ Provide programmatic design schemas   │
│ using Tailwind CSS utilities.        │
│                                      │
│ DESIGN ELEMENTS TO BUILD:            │
│ 1. Dark-glass language containers    │
│ 2. Micro-interactive layout sidebars │
│ 3. Smooth animated study flashcards  │
│ 4. Highly accessible responsive modals│
│                                      │
│ COMPLIANCE FACTOR:                   │
│ Color palettes and text contrasts    │
│ must adhere strictly to standard     │
│ accessible WCAG readability rules.   │
└──────────────────────────────────────┘

```
## 🧪 PHASE 7: Testing & Quality Assurance
### 📄 File Reference
PHASE ( 7 ) Testing & Quality (GEMINI)/1.Testing Strategy.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ QA Lead Engineer                     │
│                                      │
│ TASK:                                │
│ Architect the system end-to-end user │
│ flow automation matrices.            │
│                                      │
│ TARGET TEST SEQUENCES:               │
│ 1. Happy path: User finishes lesson  │
│ 2. Validation: Mismatched keys/auth  │
│ 3. State integrity during networks   │
│    dropping unexpectedly             │
│ 4. Layout integrity tests across      │
│    extreme responsive screen breaks  │
└──────────────────────────────────────┘

```
### 📄 File Reference
PHASE ( 7 ) Testing & Quality (GEMINI)/2.Future Road map and ideas.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐
│ ACT AS:                              │
│ EdTech Product Visionary             │
│                                      │
│ TASK:                                │
│ Formulate the post-launch Version 2.0│
│ scale backlog and module roadmap.    │
│                                      │
│ EXTENSION SCENARIOS:                 │
│ 1. Gamification badge frameworks     │
│ 2. Live user-to-user leaderboards    │
│ 3. Conversational AI speaking bots   │
│ 4. Spaced-Repetition flashcard       │
│    intervals (SRS learning logic)    │
└──────────────────────────────────────┘

```
