# Credit Saison AMA + Agentic AI Prototype

Interactive prototype for Credit Saison India's AI-powered AMA assistant with 3 agentic tools.

## What's Inside

- **AMA Assistant**: 110 pre-defined questions across 8 categories with contextual AI responses
- **Credit Score Agent**: Conversational credit score fetch via Experian (mocked)
- **Money Insights Agent**: AA-based PFM with spending analysis and Finsights dashboard (mocked)
- **BBPS Agent**: Bill payments for Mobile, Electricity, DTH, Broadband (mocked)
- **Session Memory**: AI remembers your score and financial data for personalized follow-ups
- **Intent Detection**: Natural language routing to the right agent

## Quick Deploy to GitHub Pages

### Option 1: Fastest (Manual Upload)

1. Create a new GitHub repo (e.g., `credit-saison-ama-prototype`)
2. Upload `index.html` to the root of the repo
3. Go to **Settings > Pages**
4. Under "Source", select **Deploy from a branch**
5. Choose `main` branch, `/ (root)` folder
6. Click Save
7. Your prototype will be live at `https://yourusername.github.io/credit-saison-ama-prototype/`

### Option 2: Via Git CLI

```bash
git init credit-saison-ama-prototype
cd credit-saison-ama-prototype
cp /path/to/index.html .
git add index.html
git commit -m "Credit Saison AMA prototype"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/credit-saison-ama-prototype.git
git push -u origin main
```

Then enable GitHub Pages in repo Settings.

### Option 3: Netlify Drop (Zero Config)

1. Go to [https://app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop the `index.html` file
3. Get a live URL instantly

### Option 4: Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. In the folder with `index.html`, run: `vercel`
3. Follow prompts. Done.

## How to Test

1. Open the deployed URL on a mobile browser for the best experience
2. Try these flows:
   - Tap **Credit Score** card on home screen
   - Type "cibil" or "check my score" in chat
   - Complete the credit score flow, then ask "How can I improve my score?"
   - Tap **Money Insights**, complete the flow, then ask "How much did I spend on food?"
   - Type "pay my electricity bill"
   - Try vague queries like "help" or "documents needed"

## Files

- `index.html` — Self-contained prototype (React + Babel, no build step needed)
- `credit-saison-ama-prototype.jsx` — Source React component (for integration into your app codebase)
- `README.md` — This file

## Tech Notes

- Single-file HTML with React 18, Babel standalone, no build tools needed
- All data is mocked (no real API calls)
- Session memory persists within a single page session (resets on refresh)
- Mobile-first design (390x844 viewport, simulates iPhone frame)
- Works on desktop too (centered phone frame)
