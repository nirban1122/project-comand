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
> 
> render.yaml
> 
> prisma/schema.prisma
> 
> package.json (both)
> 
> .env.example (both)
> 
> Server setup code
> 
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
> 
> Seed data file
> 
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
> 
> Frontend: Auth pages, hooks, stores, components
> 
> All TypeScript types



### PROMPT 4: Auth Testing & Security
```text
Before we move forward, review the auth system I'll copy to you:

For security:
1. Check for SQL injection vulnerabilities
2. Verify password hashing is correct (bcrypt)
3. Check JWT secret handling
4. Verify CORS is properly configured
5. Check for XSS vulnerabilities in forms

For functionality:
1. Test login/register flow manually
2. Check error messages are user-friendly
3. Verify tokens are properly stored
4. Check refresh token logic

Suggest improvements and provide fixed versions of any issues.

```
### GEMINI (ALTERNATIVE FOR THIS):
```text
In Gemini chat, ask:
"Review my authentication code for security issues 
and suggest improvements [paste your code]"
```


## 📚 PHASE 2: Courses & Lessons System



### PROMPT 5: Courses Backend
```text

Build the courses system backend for my German learning app.

API Endpoints needed:

1. GET /api/courses
   - Return all courses (A1, A2, B1, B2, C1, C2)
   - Include: title, level, description, total lessons, cover image
   - Include user progress if authenticated
   - Return: Array of courses
   
2. GET /api/courses/:id
   - Return single course with all details
   - Include: all lessons count, total hours, difficulty
   
3. GET /api/courses/:id/lessons
   - Return all lessons for a course in order
   - Include: lesson title, order, is_completed (for user)
   
4. POST /api/courses/:id/enroll
   - Enroll user in course
   - Create initial progress records

Controllers needed:
- courseController.js with all logic
- Proper error handling
- Validate courseId exists
- Check user is authenticated (where needed)

Include:
- SQL queries (through Prisma)
- Error handling
- Response formatting
- Proper HTTP status codes
```
CLAUDE WILL GIVE YOU:

> Backend courses routes
> 
>courseController.js
> 
> Database queries
> 
> Error handling


### PROMPT 6: Courses Frontend
```text
Build the courses listing page for React.

Components needed:

1. CoursesPage.jsx
   - Fetch all courses on mount
   - Display in grid (responsive)
   - Filter by level (A1, A2, B1, etc.)
   - Show loading state
   - Show error state
   - Each course shows: title, level, progress %, button

2. CourseCard.jsx
   - Display: course title, level, image, progress bar
   - Click to navigate to course
   - Show "Continue" if in progress, "Start" if new
   - Show estimated hours
   
3. Integrate with Zustand store
   - courseStore.js
   - State: courses array, loading, error, selectedCourse
   - Actions: fetchCourses, selectCourse
   
4. Create hooks
   - useCourses.js - Custom hook for course operations
   
5. Styling
   - Use Tailwind + Shadcn UI
   - Mobile responsive
   - Skeleton loading state

Make it look professional and modern.

```

CLAUDE WILL GIVE YOU:
>
> All React components
>
> Zustand store
>
> Custom hooks
>
> API calls setup
>
> Styling

## 📝 PROMPT 7: Lessons System
```text
Build the lesson page system (where students learn German).

Backend:

1. GET /api/lessons/:id
   - Return: title, description, content (HTML), 
             video URL, audio URL, key vocabulary
   - Track if user completed this lesson
   
2. POST /api/lessons/:id/complete
   - Mark lesson as completed
   - Award XP points
   - Update user progress
   - Check if all lessons in course complete
   
3. GET /api/lessons/:id/exercises
   - Return exercises for this lesson

Frontend:

1. LessonPage.jsx
   - Fetch lesson content
   - Display lesson title, content, images
   - Embedded video player (YouTube)
   - Audio player for pronunciation
   - Key vocabulary section
   - Exercises section (show exercise cards)
   - "Mark complete" button
   - "Next lesson" button
   - Progress indicator
   
2. VideoPlayer.jsx
   - Embed YouTube videos
   - Simple controls
   
3. AudioPlayer.jsx
   - Play/pause audio
   - Show pronunciation guide
   
4. VocabularyList.jsx
   - Display key words with definitions
   - German word | English translation | Audio
   
5. LessonNavigation.jsx
   - Show current lesson in course
   - Show next/previous lessons
   - Progress percentage

Styling:
- Clean, readable layout
- Good typography for learning
- Mobile optimized

```
### 📄 File Reference
PHASE ( 3 ) Exercises & Quizzes/2.Quiz System.md
### 🎯 Engineering Prompt
```text
Build the interactive exercise system.

Backend:

1. GET /api/exercises/:id
   - Return: exercise details, question, choices (without answers yet)
   - Include: difficulty, type, XP reward
   
2. POST /api/exercises/:id/submit
   - Accept user's answer
   - Check if correct
   - Award XP if correct
   - Create exercise attempt record
   - Return: isCorrect, explanation, xpEarned
   
3. GET /api/exercises/:id/feedback
   - Return detailed feedback for submitted answer

Exercise types to support:
- Multiple choice (1 correct answer)
- Multiple correct (multiple correct answers)
- Fill in the blank
- Translation
- Listening comprehension

Controllers:
- exerciseController.js with full logic
- Answer validation
- XP calculation
- Error handling

Frontend:

1. ExercisePage.jsx
   - Display exercise question
   - Load and show exercise based on type
   - Show submission form
   - Display feedback after submission
   - Show XP earned
   - Show "Next exercise" or "Back to lesson"
   
2. MultipleChoiceExercise.jsx
   - Show question
   - Show radio buttons for each choice
   - Submit button
   - Disabled after answer
   
3. FillBlankExercise.jsx
   - Show sentence with blank
   - Text input for answer
   - Submit button
   
4. TranslationExercise.jsx
   - Show sentence to translate
   - Text input
   - Submit button
   - Hint button (optional)
   
5. ListeningExercise.jsx
   - Play audio
   - Show question about audio
   - Multiple choice options
   
6. FeedbackDisplay.jsx
   - Show if correct/incorrect
   - Show explanation
   - Show correct answer if wrong
   - Show XP earned
   - Next button

Include:
- Form validation
- Loading states
- Error handling
- Immediate feedback
- TypeScript types
- Accessibility features
```
## 📊 PHASE 4: Dashboard & User Profiles
### 📄 File Reference
PHASE ( 4 ) Dashboard & User Profile/1.Dashboard System.md
### 🎯 Engineering Prompt
```text
Build the course quiz/assessment system.

Backend:

1. GET /api/quizzes
   - Return all available quizzes
   
2. GET /api/quizzes/:id
   - Return quiz questions without answers
   - Include: title, description, total questions, time limit
   
3. POST /api/quizzes/:id/submit
   - Accept all answers at once
   - Calculate score
   - Check if passed (usually 70%)
   - Create QuizScore record
   - Return: final score, passed status, detailed results
   
4. GET /api/quizzes/results/:id
   - Return user's quiz score and details

Frontend:

1. QuizzesPage.jsx
   - List all available quizzes
   - Show level, title, attempts, best score
   - "Start quiz" button
   
2. QuizPage.jsx
   - Display quiz title and instructions
   - Show timer (if timed)
   - Display questions one at a time or all
   - Progress indicator
   - Submit button at end
   
3. QuizQuestion.jsx
   - Display single question
   - Show choices/inputs
   - Next/Previous buttons
   - Questions counter
   
4. QuizResults.jsx
   - Show final score
   - Show pass/fail status
   - Show correct answers for wrong ones
   - Option to download certificate if passed
   - Retry button
   
5. QuizCertificate.jsx
   - Generate certificate
   - Display certificate info
   - Download/print option

Include:
- Timer functionality
- Progress tracking
- Score calculation
- Certificate generation (PDF - optional for MVP)
- Retry logic
```
### 📄 File Reference
PHASE ( 4 ) Dashboard & User Profile/2.User Profile.md
### 🎯 Engineering Prompt
```text

Build the user dashboard (home page after login).

Backend:

1. GET /api/stats
   - Return user statistics:
     - Total XP earned
     - Total lessons completed
     - Total courses in progress
     - Courses completed
     - Learning streak (days)
     - Current level/progress
     
2. GET /api/dashboard
   - Return: recent courses, current lessons, progress, stats
   - Personalized recommendations

Frontend:

1. Dashboard.jsx (Home page after login)
   - Greeting message (Hi, {username}!)
   - User stats card:
     - Total XP points (big number)
     - Lessons completed
     - Courses in progress
     - Learning streak
   - "Continue learning" section:
     - Show course they're in progress on
     - Show next lesson to do
     - Progress bar
   - "Recommended courses" section:
     - Show 3-4 recommended courses
   - Recent activity
   - Quick start buttons
   
2. StatCard.jsx
   - Display individual stat
   - Icon + number + label
   - Animated counter (optional)
   
3. ProgressBar.jsx
   - Show course/lesson progress
   - Percentage
   - Visual bar
   
4. ContinueLearning.jsx
   - Show current course
   - Show next lesson
   - "Continue" button
   - Progress info
   
5. Recommendations.jsx
   - Show next recommended course
   - Why recommended?
   - "Start course" button

Styling:
- Dashboard is welcoming and motivating
- Clear hierarchy
- Mobile responsive
- Icons and colors for different courses
```
## 🚀 PHASE 5: Deployment & Optimization
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/1.Deploy to Render.md
### 🎯 Engineering Prompt
```text
Build the user profile page.

Backend:

1. GET /api/profile
   - Return user profile info
   - Return user statistics
   - Return completed certificates
   
2. PUT /api/profile
   - Update user profile (name, bio, photo, preferences)
   
3. GET /api/profile/certificates
   - Return all user's certificates/achievements

Frontend:

1. ProfilePage.jsx
   - User info section:
     - Profile photo
     - Name
     - Email
     - Native language
     - Member since
     - Bio/About
   - Stats section:
     - Total XP
     - Courses completed
     - Lessons completed
     - Current streak
     - Longest streak
   - Certificates section:
     - List of completed courses
     - Download certificate button
   - Learning preferences
   - Delete account option
   
2. ProfileHeader.jsx
   - Display profile info
   - Edit button
   - Upload photo (optional)
   
3. StatsList.jsx
   - Detailed statistics
   - Charts (bar chart of courses progress)
   
4. CertificatesList.jsx
   - List all certificates
   - Download each one
   - Share certificate (optional)
   
5. EditProfileModal.jsx
   - Edit form for profile
   - Update button
   - Cancel button

Include:
- Form validation
- File upload for profile photo
- Success/error messages
- Loading states

```
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/2.Performance & Optimization.md
### 🎯 Engineering Prompt
```text
Help me deploy my full-stack German learning app to Render.

I need:

1. Complete render.yaml configuration
   - Frontend service (React)
   - Backend service (Node.js)
   - PostgreSQL database service
   - Environment variables
   - Build and start commands
   
2. Deployment instructions
   - Push to GitHub
   - Connect GitHub to Render
   - Deploy via blueprint
   
3. Environment setup
   - Production .env variables
   - Database connection string
   - JWT secret generation
   - CORS configuration
   
4. Database migration on deploy
   - Run Prisma migrations automatically
   - Seed data (optional)
   
5. Troubleshooting guide
   - Common errors and fixes
   - Logs access
   - Debugging tips

My repo structure:
- /frontend (React)
- /backend (Node.js)
- Root level render.yaml

Provide complete render.yaml and all necessary configs.

```
### 📄 File Reference
PHASE ( 5 ) Deployment & Polish/3.Error Handling & Logging.md
### 🎯 Engineering Prompt
```text

Review my app for performance issues and provide optimization tips.

Areas to review:
1. Database queries - any N+1 problems?
2. Frontend bundle size - any unused dependencies?
3. API response times - any slow endpoints?
4. Database indexes - are they optimal?
5. Caching - what should we cache?
6. Image optimization
7. Code splitting opportunities
8. Loading states and skeleton screens

Suggest:
1. Database query optimizations
2. Frontend optimizations (lazy loading, code splitting)
3. API response optimization
4. Caching strategies
5. Monitor/logging setup
6. SEO improvements

Provide code examples for each optimization.
```
## 🎨 PHASE 6: UI Components
### 📄 File Reference
PHASE ( 6 ) UI Components (V0.DEV)/Beautiful UI Components.md
### 🎯 Engineering Prompt
```text
Build comprehensive error handling and logging for my app.

Backend:

1. Error handling middleware
   - Catch all errors
   - Format error responses
   - Log errors
   - Don't expose sensitive info
   
2. Logging setup
   - Log all API calls
   - Log errors with stack traces
   - Log authentication attempts
   - Log performance metrics
   
3. Error types
   - Validation errors
   - Auth errors
   - Database errors
   - Server errors
   - Not found errors

Frontend:

1. Global error handling
   - Catch async errors
   - Display user-friendly messages
   - Log errors to backend
   
2. Error boundary component
   - Catch React errors
   - Display fallback UI
   
3. API error handling
   - Intercept failed requests
   - Retry logic
   - User notifications

Provide:
- Error handling middleware
- Logger utility
- Error boundary component
- Global error handler
- TypeScript error types
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
