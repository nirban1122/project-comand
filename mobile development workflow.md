Mobile Development Workflow-


Using GitHub.dev (No installation needed):


STEP 1: Go to github.com/yourname/repo
STEP 2: Press '.' (dot) on keyboard
STEP 3: VS Code opens in browser!
STEP 4: Edit files in the editor
STEP 5: Commit from Source Control tab
STEP 6: Push to main
STEP 7: Render auto-deploys (5 min)
STEP 8: Test at https://your-app.onrender.com



Using Termux (Android):

$ apt update && apt upgrade -y
$ apt install git nodejs npm
$ git clone your-repo
$ cd german-learning-app/frontend
$ npm install
$ npm run dev (to test locally)
$ git add .
$ git commit -m "Add feature"
$ git push origin main
(Render auto-deploys)