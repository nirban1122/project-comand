# 📑 MASTER PROMPT ARCHITECTURE: GERMAN LEARNING APP
This master document compiles your entire phase-by-phase development



# MAIN ARCHITECTURE OF THIS PROJECT:

─────────────────                  
➡️  CLAUDE (Main) - Architecture + Full Code     
 "You are here" - Primary coder for full-stack  
                                                   
─────────────────
                                          
➡️  GEMINI - Brainstorming + Alternatives 
    Quick ideas, features, testing strategies 
                                      
────────────────────
                
➡️  V0.DEV - UI Components                    
    Beautiful React components with Shadcn/UI     
                                                
──────────────────────
                                                    
➡️ GitHub Copilot - Real-time Code Assist (Optional)
   In-editor suggestions while you code              
                                                  
─────────────────────────



## Mobile Development Workflow-


### Using GitHub.dev (No installation needed):


STEP 1: Go to github.com/yourname/repo

STEP 2: Press '.' (dot) on keyboard

STEP 3: VS Code opens in browser!

STEP 4: Edit files in the editor

STEP 5: Commit from Source Control tab

STEP 6: Push to main

STEP 7: Render auto-deploys (5 min)

STEP 8: Test at https://your-app.onrender.com






## Using Termux (Android):

```text
$ apt update && apt upgrade -y
```
```trxt
$ apt install git nodejs npm
```
```text
$ git clone your-repo
```
```text
$ cd german-learning-app/frontend
```
```text
$ npm install
```
```text
$ npm run dev (to test locally)
```
```text
$ git add .
```
```text
$ git commit -m "Add feature"
```
```text
$ git push origin main
```
```text
(Render auto-deploys)
```




## Vibe Coding Workflow:

DAY 1 (SETUP):
1. Come back to this chat → Copy PROMPT 1
2. Paste in Claude (here) → Get project structure
3. Copy PROMPT 2 → Get database schema
4. Create files from Claude's output in GitHub.dev

DAY 2 (AUTH):
1. Copy PROMPT 3 → Give to Claude
2. Get auth code → Create files
3. Test on localhost
4. Copy PROMPT 4 → Review code

DAY 3-5 (COURSES & LESSONS):
1. Copy PROMPT 5 → Claude (backend)
2. Copy PROMPT 6 → Claude (frontend)
3. Copy PROMPT 7 → Claude (lessons)
4. Create files → Test → Deploy to Render

DAY 6-7 (EXERCISES):
1. Copy PROMPT 8 → Claude
2. Copy PROMPT 9 → Claude
3. Build components → Test

DAY 8-9 (DASHBOARD):
1. Copy PROMPT 10 → Claude
2. Copy PROMPT 11 → Claude
3. Build & integrate

DAY 10 (DEPLOY):
1. Copy PROMPT 12 → Claude
2. Follow Render deployment
3. Push to GitHub → Auto-deploy
4. Live! 🎉

DAY 11+ (POLISH):
1. Copy PROMPT 15 → V0.dev → Get beautiful components
2. Copy PROMPT 16 → Gemini → Testing ideas
3. Copy PROMPT 17 → Gemini → Feature roadmap



## PROMPT DISTRIBUTION MAP 🗺️-

```text

PHASE 1: SETUP
├─ PROMPT 1 → CLAUDE (Project structure)
└─ PROMPT 2 → CLAUDE (Database schema)

PHASE 2: AUTH
├─ PROMPT 3 → CLAUDE (Full auth system)
└─ PROMPT 4 → CLAUDE (Security review) or GEMINI (Quick review)

PHASE 3: COURSES & LESSONS
├─ PROMPT 5 → CLAUDE (Courses backend)
├─ PROMPT 6 → CLAUDE (Courses frontend)
└─ PROMPT 7 → CLAUDE (Lessons system)

PHASE 4: EXERCISES & QUIZZES
├─ PROMPT 8 → CLAUDE (Exercise system)
└─ PROMPT 9 → CLAUDE (Quiz system)

PHASE 5: DASHBOARD & PROFILE
├─ PROMPT 10 → CLAUDE (Dashboard)
└─ PROMPT 11 → CLAUDE (User profile)

PHASE 6: DEPLOYMENT
├─ PROMPT 12 → CLAUDE (Render deployment)
├─ PROMPT 13 → CLAUDE (Optimization)
└─ PROMPT 14 → CLAUDE (Error handling)

PHASE 7: UI POLISH
└─ PROMPT 15 → V0.DEV (Beautiful components)

PHASE 8: QUALITY & GROWTH
├─ PROMPT 16 → GEMINI (Testing strategy)
└─ PROMPT 17 → GEMINI (Feature ideas)
```


## 🏗️ PHASE 0: Project Setup & Architecture

### PROMPT 1: Initial Setup & Project Structure
```text
I'm building a German language learning website for international 
students using React, Node.js, and PostgreSQL on Render.

I need you to:

1. Create the complete project structure for my repo
2. Generate render.yaml for deployment
3. Create Prisma schema for German learning platform
4. Generate package.json for both frontend and backend
5. Create .env.example files
6. Generate initial Express server setup
7. Create React + Vite initial setup
8. Provide all necessary configuration files

Project details:
- Frontend: React + Vite + Tailwind + Shadcn UI
- Backend: Node.js + Express + Prisma
- Database: PostgreSQL (Render)
- Hosting: Render (free tier initially)
- Mobile development: GitHub.dev + Termux

Include TypeScript support and modern best practices.
Please provide each file separately so I can create them one by one.

```
CLAUDE WILL GIVE YOU:
> Complete folder structure
> render.yaml
> prisma/schema.prisma
> package.json (both)
> .env.example (both)
> Server setup code
> Client setup code


### PROMPT 2: Database Schema Deep Dive
```text
Using the German learning platform schema you created, 
I need detailed Prisma models for:

1. User (with profile, preferences, native language)
2. Course (A1-C2 levels)
3. Lesson (with content, video, audio)
4. Exercise (multiple types: multiple choice, fill-blank, listening)
5. Progress tracking
6. Quiz system
7. Flashcards (vocabulary)
8. User statistics

For each model:
- Add all necessary fields
- Add relationships
- Add indexes for performance
- Add validation
- Add timestamps (createdAt, updatedAt)
- Add unique constraints where needed

Also provide:
- Migration commands
- Seed file with sample A1 German course data
- Sample lessons (5-10) with exercises

Make it production-ready with proper constraints.

```
CLAUDE WILL GIVE YOU:
> Complete Prisma schema
> Seed data file
> Migration setup


## 🔐 PHASE 1: Authentication System



### PROMPT 3: Complete Auth System
```text
Build the complete authentication system for my German learning app.

BACKEND (Node.js/Express):
1. User registration endpoint (POST /api/auth/register)
   - Email validation
   - Password hashing (bcrypt)
   - Input validation
   - Error handling
   
2. User login endpoint (POST /api/auth/login)
   - Email/password verification
   - JWT token generation
   - Refresh token logic
   - Error messages
   
3. JWT verification middleware
   - Check token validity
   - Extract user from token
   - Protect routes
   
4. Password reset flow (optional but include)

FRONTEND (React):
1. Register page component
   - Email input
   - Password input
   - Password confirmation
   - Submit button
   - Link to login
   - Form validation
   - Error messages
   - Loading state
   
2. Login page component
   - Email/password inputs
   - "Remember me" checkbox
   - Submit button
   - Forgot password link
   - Link to register
   - Error messages
   - Loading state
   
3. useAuth custom hook
   - Login function
   - Register function
   - Logout function
   - Get current user
   
4. Zustand auth store
   - user state
   - isLoading state
   - error state
   - setUser action
   - logout action

Include:
- Full TypeScript types
- Error handling
- Loading states
- Toast notifications
- Protected route component
- Password validation rules
- CORS configuration

Provide each file separately.

```
CLAUDE WILL GIVE YOU:
> Backend: auth routes, controllers, middleware, JWT utils
> Frontend: Auth pages, hooks, stores, components
> All TypeScript types
### 📄 File Reference
PHASE ( 1) Authentication System/2.AUTH TEST AND SECURITY(Claude).md
### 🎯 Engineering Prompt
```text


```
## 📚 PHASE 2: Courses & Lessons System
### 📄 File Reference
PHASE ( 2 ) Courses & Lessons/1.Courses Backend.md
### 🎯 Engineering Prompt
```text


```
### 📄 File Reference
PHASE ( 2 ) Courses & Lessons/2.Lessons System.md
### 🎯 Engineering Prompt
```text


```
## 📝 PHASE 3: Exercises & Quizzes
### 📄 File Reference
PHASE ( 3 ) Exercises & Quizzes/1.Exercise System.md
### 🎯 Engineering Prompt
```text


```
### 📄 File Reference
PHASE ( 3 ) Exercises & Quizzes/2.Quiz System.md
### 🎯 Engineering Prompt
```text

```
## 📊 PHASE 4: Dashboard & User Profiles
### 📄 File Reference
PHASE ( 4 ) Dashboard & User Profile/1.Dashboard System.md
### 🎯 Engineering Prompt
```text

```
### 📄 File Reference
PHASE ( 4 ) Dashboard & User Profile/2.User Profile.md
### 🎯 Engineering Prompt
```text


```
## 🚀 PHASE 5: Deployment & Optimization
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/1.Deploy to Render.md
### 🎯 Engineering Prompt
```text
┌──────────────────────────────────────┐


```
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/2.Performance & Optimization.md
### 🎯 Engineering Prompt
```text


```
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/3.Error Handling & Logging.md
### 🎯 Engineering Prompt
```text


```
## 🎨 PHASE 6: UI Components
### 📄 File Reference
PHASE ( 6 ) UI Components (V0.DEV)/Beautiful UI Components.md
### 🎯 Engineering Prompt
```text

```
## 🧪 PHASE 7: Testing & Quality Assurance
### 📄 File Reference
PHASE ( 7 ) Testing & Quality (GEMINI)/1.Testing Strategy.md
### 🎯 Engineering Prompt
```text

```
### 📄 File Reference
PHASE ( 7 ) Testing & Quality (GEMINI)/2.Future Road map and ideas.md
### 🎯 Engineering Prompt
```text


```
