# Project Kickoff Questionnaire

Use this questionnaire with Claude Code to plan and set up your fullstack web app. Copy the sections you need or use the full questionnaire.

---

## Quick Start Prompt

Copy and paste this to Claude to get started:

```
I want to build a new web app. Please ask me the project kickoff questions to understand what I'm building, then help me set up the project structure and configuration.
```

---

## Full Questionnaire

### 1. Project Overview

**What are you building?**
- [ ] SaaS platform
- [ ] E-commerce / marketplace
- [ ] Social / community platform
- [ ] Dashboard / analytics tool
- [ ] Content management system
- [ ] Portfolio / marketing site
- [ ] Internal tool / admin panel
- [ ] Other: _______________

**Describe your project in 1-2 sentences:**
> _Your answer here_

**Who is your target user?**
> _Your answer here_

---

### 2. Frontend Setup

**Framework:**
- [ ] Next.js 15 (recommended - App Router, Server Components)
- [ ] Next.js 14 (Pages Router)
- [ ] Vite + React
- [ ] Other: _______________

**Styling approach:**
- [ ] Tailwind CSS (recommended)
- [ ] CSS Modules
- [ ] Styled Components / Emotion
- [ ] Other: _______________

**UI Component library:**
- [ ] shadcn/ui (recommended - copy/paste components, full control)
- [ ] Radix UI (headless primitives)
- [ ] Chakra UI
- [ ] Material UI
- [ ] Build from scratch
- [ ] Other: _______________

**Design preferences:**
- [ ] Dark mode only
- [ ] Light mode only
- [ ] Both (with toggle)
- [ ] System preference

**Do you have existing designs?**
- [ ] Yes, Figma/design files
- [ ] Yes, reference sites I want to match
- [ ] No, need design guidance
- [ ] Minimal UI is fine

---

### 3. Authentication

**Authentication approach:**
- [ ] Email/password
- [ ] Social login (Google, Twitter, etc.)
- [ ] Passkeys/WebAuthn
- [ ] Magic link / passwordless
- [ ] No authentication needed

**Auth provider:**
- [ ] Supabase Auth (recommended)
- [ ] NextAuth.js
- [ ] Clerk
- [ ] Auth0
- [ ] Custom implementation

---

### 4. Database & Backend

**Do you need a database?**
- [ ] Yes
- [ ] No
- [ ] Not sure

**If yes, what data needs to be stored?**
- [ ] User profiles / preferences
- [ ] Transaction history / analytics
- [ ] Content (posts, comments, etc.)
- [ ] Files / media metadata
- [ ] Other: _______________

**Database preference:**
- [ ] Supabase (recommended - Postgres + realtime + auth + storage)
- [ ] PlanetScale (MySQL)
- [ ] Neon (Postgres)
- [ ] MongoDB
- [ ] SQLite (local/simple)
- [ ] Other: _______________

**ORM preference:**
- [ ] Prisma (recommended - type-safe, great DX)
- [ ] Drizzle
- [ ] Raw SQL
- [ ] Other: _______________

**Do you need realtime features?**
- [ ] Yes (live updates, notifications, chat)
- [ ] No
- [ ] Maybe later

---

### 5. API & Data Fetching

**API approach:**
- [ ] Server Actions (Next.js - recommended for simple cases)
- [ ] tRPC (type-safe API)
- [ ] REST API
- [ ] GraphQL
- [ ] Combination

**External APIs you'll integrate:**
- [ ] Payment processor (Stripe, etc.)
- [ ] Email service (Resend, SendGrid, etc.)
- [ ] Analytics (PostHog, Mixpanel, etc.)
- [ ] Other: _______________

---

### 6. File Storage

**Do you need file/media storage?**
- [ ] Yes
- [ ] No
- [ ] Maybe later

**If yes, what types?**
- [ ] Images (avatars, thumbnails)
- [ ] Documents
- [ ] Large files / videos

**Storage preference:**
- [ ] Supabase Storage (recommended if using Supabase)
- [ ] AWS S3
- [ ] Cloudflare R2
- [ ] Uploadthing
- [ ] Other: _______________

---

### 7. Deployment & Infrastructure

**Deployment target:**
- [ ] Vercel (recommended for Next.js)
- [ ] Netlify
- [ ] Railway
- [ ] AWS
- [ ] Self-hosted
- [ ] Other: _______________

**Environment needs:**
- [ ] Development (local)
- [ ] Staging
- [ ] Production

**Do you need background jobs/workers?**
- [ ] Yes (notifications, processing, etc.)
- [ ] No
- [ ] Not sure

---

### 8. Testing Requirements

**Testing approach:**
- [ ] Unit tests (Vitest/Jest)
- [ ] Integration tests
- [ ] E2E tests (Playwright/Cypress)
- [ ] Minimal/manual testing only

**CI/CD:**
- [ ] GitHub Actions (recommended)
- [ ] Other CI
- [ ] None yet

---

### 9. Project Structure

**Monorepo or single app?**
- [ ] Monorepo (recommended for frontend + backend + shared packages)
- [ ] Single app (frontend only)
- [ ] Not sure

**If monorepo, what packages?**
- [ ] Frontend (Next.js)
- [ ] Backend API
- [ ] Shared types/utils
- [ ] Marketing site
- [ ] Mobile app

---

### 10. Timeline & Priorities

**What's the priority order?**
1. _______________
2. _______________
3. _______________

**MVP scope - what's the minimum to launch?**
> _Your answer here_

**Any hard deadlines?**
> _Your answer here_

---

### 11. Existing Code & Constraints

**Starting from:**
- [ ] Scratch (new project)
- [ ] Existing codebase (need to integrate)
- [ ] Fork of another project
- [ ] Template

**Any technical constraints?**
> _Your answer here_

**Team size:**
- [ ] Solo developer
- [ ] Small team (2-5)
- [ ] Larger team (5+)

---

## After Answering

Once you've filled this out, Claude can help you:

1. **Generate project structure** - Create the folder layout and initial files
2. **Configure tooling** - Set up TypeScript, ESLint, Prettier, etc.
3. **Set up database schema** - Design your Prisma/Supabase schema
4. **Create component library** - Set up shadcn/ui with your theme
5. **Plan the build** - Break down into tasks and milestones

---

## Example Usage

```
I filled out the project kickoff questionnaire:

**Building:** SaaS dashboard for team project management
**Target user:** Small teams who want a simple project tracker
**Frontend:** Next.js 15, Tailwind, shadcn/ui, dark mode
**Auth:** Email/password + Google login via Supabase Auth
**Database:** Supabase for user profiles and project data
**Storage:** Supabase Storage for file attachments
**Deploy:** Vercel
**Priority:** 1) Auth flow 2) Project CRUD 3) Team invites

Please help me set up the project structure and create the initial configuration files.
```
