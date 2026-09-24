# Gemini CLI System Instructions

## Project Architecture
This is a monorepo containing a Python FastAPI backend and a Node.js Vite React + TypeScript frontend.

## Global Assistant Rules
*   **Pathing:** Always provide the full relative path when editing or generating files (e.g., `frontend/src/App.tsx`).
*   **Conciseness:** Provide direct code solutions with minimal conversational filler.
*   **Dependencies:** Do not introduce new third-party libraries to `requirements.txt` or `package.json` without asking first. 

## Backend Rules (Python/FastAPI)
*   **Typing:** Use strict Python type hints.
*   **Concurrency:** Default to `async def` for API endpoints.
*   **Validation:** Use Pydantic models for all request and response schemas.
*   **Structure:** Keep routing logic in `backend/app/api/` and business logic separate.

## Frontend Rules (Node/React/TypeScript)
*   **Components:** Use functional components and modern React hooks. Do not use class components.
*   **Typing:** Use strict TypeScript interfaces. Never use `any`.
*   **Linting:** Ensure all code conforms to ESLint rules.
*   **State:** Keep local state near where it is used; elevate state only when necessary.


# Gemini CLI System Instructions

## Project Overview
**App Name:** MyAjo
**Purpose:** A digital Rotating Savings and Credit Association (ROSCA / Ajo) platform enabling group financial contributions, automated payout round tracking, and peer-to-peer slot swapping.

**Core Features:**
*   **Authentication & Group Management:** Secure JWT authentication, group creation, member onboarding, and recurring contribution cycle setup.
*   **Contribution Dashboard & Real-Time Status:** Live visibility into total uploaded pool funds, verified member contributions, and pending/overdue payments for the active round.
*   **Payout Queue & Peer-to-Peer Slot Swapping:** Visual distribution timeline allowing members to request, negotiate, and execute slot exchanges with fellow group members for urgent liquidity needs.
*   **Audit Ledger & History:** Transparent transaction logs tracking total round payouts, historical contributions, and swap approvals.
*   **Notification System:** Automated reminders for upcoming contribution deadlines and alerts for slot-swap requests.

## Project Architecture
This is a monorepo containing a Python FastAPI backend and a Node.js Vite React + TypeScript frontend.
... (keep your existing rules below) ...