# Fullstack Web App Skills

A comprehensive collection of Claude Code skills for building modern fullstack web applications. These skills provide opinionated guidance, best practices, and reusable patterns for the entire development stack.

## What's Included

### Web Development Skills

| Skill | Description |
|-------|-------------|
| `nextjs.md` | Next.js 15 with App Router, Server Components, Server Actions |
| `tailwind.md` | Tailwind CSS v4 patterns, responsive design, dark mode |
| `prisma.md` | Prisma ORM - schema design, migrations, type-safe queries |
| `supabase.md` | Supabase - RLS, Auth, Edge Functions, Realtime |
| `docker.md` | Docker and Docker Compose for development and production |
| `orval.md` | API client generation from OpenAPI specs |

### Development Workflow Skills

| Skill | Description |
|-------|-------------|
| `code-reusability.md` | Always check for existing code before writing new |
| `code-simplifier.md` | Clean up complex code at end of sessions |
| `style-system.md` | Design tokens, component patterns, accessibility |

### Commands (Slash Commands)

| Command | Description |
|---------|-------------|
| `/check-existing` | Audit existing components, styles, packages |
| `/commit` | Create well-formatted git commits |
| `/build` | Build all packages |
| `/dev` | Start development servers |
| `/test` | Run tests (Vitest/Jest) |
| `/lint` | Run ESLint |
| `/format` | Format with Prettier |
| `/type-check` | Run TypeScript checks |
| `/db-generate` | Generate Prisma client |
| `/db-push` | Push schema to database |
| `/api-generate` | Generate API client from OpenAPI |
| `/review-pr` | Review a GitHub pull request |
| `/setup` | Set up development environment |
| `/simplify` | Run code simplifier agent |
| `/clean` | Clean build artifacts |

## Getting Started

### Project Kickoff Questionnaire

Starting a new project? Use the **[PROJECT_KICKOFF.md](PROJECT_KICKOFF.md)** questionnaire to help Claude understand what you're building. It covers:

- Project type and target users
- Frontend stack (Next.js, Tailwind, UI components)
- Authentication approach
- Database and API architecture
- Deployment and infrastructure

**Quick start prompt:**
```
I want to build a new web app. Please ask me the project kickoff questions to understand what I'm building, then help me set up the project structure.
```

## Installation

Copy the `.claude` folder to your project root:

```bash
cp -r .claude /path/to/your/project/
```

Or clone this repo and copy what you need:

```bash
git clone https://github.com/0xGF/solana-fullstack-webapp-skills.git
cp -r solana-fullstack-webapp-skills/.claude /path/to/your/project/
```

## Usage

Once the `.claude` folder is in your project, Claude Code will automatically pick up the skills and commands.

### Skills

Skills are automatically loaded based on context. You can also explicitly invoke them:

```
Use the nextjs skill
Use the prisma skill
```

### Commands

Commands are invoked with a slash:

```
/commit fix: resolve login issue
/build
/test frontend
/dev backend
```

## Stack Preferences

These skills are opinionated and prefer:

- **Framework**: Next.js 15 with App Router
- **Styling**: Tailwind CSS v4
- **Database**: Prisma with PostgreSQL
- **Backend**: Supabase or custom API

## Customization

Feel free to modify these skills for your specific needs:

1. Edit skill files to match your project patterns
2. Update commands to use your project's script names
3. Add new skills for project-specific guidance
4. Remove skills you don't need

## Contributing

Contributions welcome! Please:

1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## License

MIT License - feel free to use, modify, and distribute.

## Credits

Built with modern web development best practices.
