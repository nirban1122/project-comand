To compile all your phase-by-phase prompt requirements from your LEARNGERMAN.zip file map into a single, master file layout according to the **PROMPT DISTRIBUTION MAP.md** workflow, we can structure it sequentially.
This master document acts as a continuous engineering instruction file. You can pass sections of this directly to an AI tool (like Claude, Cursor, or Gemini) during your **Vibe Coding** or **Mobile Development** sessions.
# 📑 MASTER PROMPT ARCHITECTURE: GERMAN LEARNING APP
This single document compiles the operational design prompts, validation rules, and deployment instructions mapped out across all development cycles. Use these precise prompts to instruct your AI coding assistants sequentially.
## 🏗️ PHASE 0: Project Setup & Architecture
### 📄 File Reference: PHASE ( 0 )Project Setup & Architecture/1.MAIN ARCHITECTURE.md
```markdown
PROMPT: Act as a Principal Software Architect. Define a comprehensive technical architecture blueprint for a full-stack German language learning platform. The system must support user onboarding, structured video/text lessons, interactive grammatical exercises, real-time feedback loops, progress tracking dashboards, and scalable API routing. Provide the definitive tech stack configuration, global directory structures (monorepo format), code splitting parameters, environment variable management guidelines, and state management architectural patterns optimized for low-latency client performance.

```
### 📄 File Reference: PHASE ( 0 )Project Setup & Architecture/2.initialsetup(claude).md
```markdown
PROMPT: Act as a Senior DevOps Engineer. Generate a precise initialization script and step-by-step setup guide using the technical baseline established in the main architecture. Initialize a backend server workspace and a frontend application environment. Configure all structural dependency files, root configs (TypeScript/tsconfig, ESLint, Prettier, EditorConfig, Tailwind configs), package configurations, and initial environmental variables hooks. Ensure everything compiles with zero warnings and absolute configuration strictness.

```
### 📄 File Reference: PHASE ( 0 )Project Setup & Architecture/3.Db Schema (Claude).md
```markdown
PROMPT: Act as a Lead Database Administrator. Write a production-ready relational database schema model for a German learning platform using a modern ORM syntax. Define specific entity relationships, primary/foreign key mappings, explicit indexes, and cascade constraints for the following tables: Users, Profiles, UserProgress, Courses, Modules, Lessons, Exercises, Submissions, Quizzes, and AuditLogs. Ensure strict data integrity, type safety, optimized query structures for fast relational traversal, and provide the initial database migration configuration scripts.

```
## 🔐 PHASE 1: Authentication System
### 📄 File Reference: PHASE ( 1) Authentication System/1.Auth sys(Claude).md
```markdown
PROMPT: Act as a Senior Security Engineer. Build a robust backend and frontend authentication flow. Implement secure registration, login, and token-based session lifecycle management utilizing standard security layers (e.g., JWT securely managed via HTTP-only cookies or encrypted local storage wrappers). Include middleware for role-based route access controls (Admin vs. Student), strict input sanitation templates, automated password hashing logic with secure salts, and complete payload schemas for user validation handling.

```
### 📄 File Reference: PHASE ( 1) Authentication System/2.AUTH TEST AND SECURITY(Claude).md
```markdown
PROMPT: Act as a QA Security Tester. Write a unit and integration test suite designed exclusively to stress-test the authentication system. Implement testing logic to catch security vulnerabilities including invalid JWT structures, token expiration edge cases, credential brute-forcing mitigation handling, cross-site scripting (XSS) via auth inputs, and SQL Injection/NoSQL payload bypass attempts. Ensure mock response patterns return correct error schemas and status assertions.

```
## 📚 PHASE 2: Courses & Lessons System
### 📄 File Reference: PHASE ( 2 ) Courses & Lessons/1.Courses Backend.md
```markdown
PROMPT: Act as a Senior Backend Developer. Develop the relational API endpoints for a multi-tiered German learning structure: Courses -> Levels (A1, A2, B1) -> Modules -> Lessons. Build high-performance, paginated query controllers to retrieve lessons with their respective completion statuses, alongside structural administrative endpoints allowing content managers to programmatically create, read, update, and delete course nodes.

```
### 📄 File Reference: PHASE ( 2 ) Courses & Lessons/2.Lessons System.md
```markdown
PROMPT: Act as a Frontend Engineer. Create an immersive, component-driven Lesson View system interface. It must render diverse content types including text definitions, embedded markdown audio components for pronounciation, video playback containers, and vocabulary glossary highlights. Implement persistent local progress synchronization tracking to update the backend the moment a user completes or marks a specific lesson node.

```
## 📝 PHASE 3: Exercises & Quizzes
### 📄 File Reference: PHASE ( 3 ) Exercises & Quizzes/1.Exercise System.md
```markdown
PROMPT: Act as an Educational UX Developer. Build an interactive interactive exercise engine tailored specifically to foreign language acquisition. Implement state machine loops to run and evaluate three distinct interactive question variations: 
1. Multiple Choice Questions (MCQ).
2. Fill-in-the-blanks with inline textual entry.
3. Sentence reorganization via interactive drag-and-drop mechanics.
Provide immediate validation UI feedback handling (Green/Success or Red/Error) along with clear grammatical correction tips on incorrect user evaluation inputs.

```
### 📄 File Reference: PHASE ( 3 ) Exercises & Quizzes/2.Quiz System.md
```markdown
PROMPT: Act as a Core Logic Systems Engineer. Create a high-stakes, time-boxed Module Quiz System engine. Implement a client-side and server-validated countdown timer mechanism, an active exam progress save hook, sequential step-by-step submission logic, and an automated grading evaluator backend function. Once a quiz concludes, calculate precise score percentages, total time spent, and output a granular grading performance card to the database storage.

```
## 📊 PHASE 4: Dashboard & User Profiles
### 📄 File Reference: PHASE ( 4 ) Dashboard & User Profile/1.Dashboard System.md
```markdown
PROMPT: Act as a Full-Stack Product Developer. Build the primary Student Progress Dashboard. Aggregate multi-source data insights to visually calculate and render the active user metrics: Overall Course Progress Percentages, Current Day Streak Trackers, Lesson/Quiz Completion Counts, and an Interactive Daily Activity Heatmap grid. Ensure data fetching hooks leverage smart caching layers to minimize duplicate database load on page initialization.

```
### 📄 File Reference: PHASE ( 4 ) Dashboard & User Profile/2.User Profile.md
```markdown
PROMPT: Act as a UI Layout Specialist. Create the User Settings and Profile Panel interface. Design distinct interactive modular sub-sections: Profile Detail Updates (Avatar, name, email handling), Language Selection Goals, Application Theme Customization switches (Light vs Dark mode persistent toggles), and Account Data Management access points (Password changes or account deletions). Connect all update fields to direct operational database mutation endpoints.

```
## 🚀 PHASE 5: Deployment & Optimization
### 📄 File Reference: PHASE ( 5 ) Deployment & Polish/1.Deploy to Render.md
```markdown
PROMPT: Act as an Infrastructure Specialist. Write the declarative runtime build configurations, deploy manifests, and production orchestration parameters necessary to safely host the application stack on Render. Produce automated shell build commands, target base package script triggers, reverse proxy routing rules, cluster environment handling scripts, and production environment health check endpoint definitions.

```
### 📄 File Reference: PHASE ( 5 ) Deployment & Polish/2.Performance & Optimization.md
```markdown
PROMPT: Act as a Web Performance Engineer. Audit and optimize the system workflow layers. Implement client-side asset optimization protocols, dynamic code-splitting and component lazy-loading layouts, aggressive static data caching mechanisms, network compression utilities, and strategic database connection pooling models to drop Time-to-First-Byte (TTFB) and secure a perfect score across standard web performance metrics.

```
### 📄 File Reference: PHASE ( 5 ) Deployment & Polish/3.Error Handling & Logging.md
```markdown
PROMPT: Act as a Site Reliability Engineer (SRE). Engineer an uncompromising global error management layer. Write functional central Try-Catch middleware systems for asynchronous runtime paths, customized exception classes reflecting accurate protocol fault conditions, production-grade console logger formats, and explicit fallbacks to ensure client-facing applications never crash or expose raw source stack traces during operational exceptions.

```
## 🎨 PHASE 6: UI Components
### 📄 File Reference: PHASE ( 6 ) UI Components (V0.DEV)/Beautiful UI Components.md
```markdown
PROMPT: Act as a UI/UX Designer specialized in v0.dev prompt engineering. Provide highly descriptive component styling blueprints utilizing Tailwind CSS tokens and semantic tokens. Deliver structured component interface syntax guidelines for producing premium UI layouts: custom-molded dark-glass language select containers, side navigation blocks with fluid micro-interactions, floating flashcard action cards, and responsive modal screens built to adhere strictly to WCAG modern accessible color standards.

```
## 🧪 PHASE 7: Testing & Quality Assurance
### 📄 File Reference: PHASE ( 7 ) Testing & Quality (GEMINI)/1.Testing Strategy.md
```markdown
PROMPT: Act as a QA Lead Engineer. Design the master Quality Assurance automation matrix. Write end-to-end user flows, execution steps, and integration target criteria to safely evaluate the platform's stability. Build execution code to automate test paths for: Completing a lesson module path successfully, evaluating edge cases on mismatched password logic inputs, checking persistence layer integrity across intentional disconnections, and testing responsive mobile layout breaks.

```
### 📄 File Reference: PHASE ( 7 ) Testing & Quality (GEMINI)/2.Future Road map and ideas.md
```markdown
PROMPT: Act as an EdTech Product Visionary. Formulate an extensive version 2.0 product architecture enhancement feature backlog. Map explicit conceptual feature schemas, design strategies, and algorithmic interface logic for integrating future modules including: Gamified Badge/Reward point mechanics, Real-time peer-to-peer vocabulary leaderboards, Contextual AI-driven dialogue partner instances, and Intelligent Spaced-Repetition Review algorithms (SRS) designed to surface older flashcards right before failure points.

```
