# Credit Saison AMA + Agentic AI Prototype

Interactive prototype for Credit Saison India's AI-powered AMA assistant with 3 agentic tools.

## What's Inside

- **AMA Assistant**: 110 pre-defined questions across 8 categories with contextual AI responses
- **Credit Score Agent**: Conversational credit score fetch via Experian (mocked)
- **Money Insights Agent**: AA-based PFM with spending analysis and Finsights dashboard (mocked)
- **BBPS Agent**: Bill payments for Mobile, Electricity, DTH, Broadband (mocked)
- **Session Memory**: AI remembers your score and financial data for personalized follow-ups
- **Intent Detection**: Natural language routing to the right agent

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
