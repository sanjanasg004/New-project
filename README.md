# New-projecc:\Users\Sanjana\App
|-- .env.example
|-- .gitignore
|-- README.md
|-- docker-compose.local.yml
|-- package.json
|-- pnpm-workspace.yaml
|-- turbo.json
|
|-- apps/
|   |-- web/
|   |   |-- next-env.d.ts
|   |   |-- next.config.ts
|   |   |-- package.json
|   |   |-- tsconfig.json
|   |   |-- src/
|   |   |   |-- app/(auth)/layout.tsx, page.tsx
|   |   |   |-- app/(dashboard)/layout.tsx, page.tsx
|   |   |   |-- app/api/v1/route.ts
|   |   |   |-- app/layout.tsx, page.tsx
|   |   |   |-- components/ui/index.ts
|   |   |   |-- features/{auth-profile,job-tracker,readiness,resume,notifications,analytics}/index.ts
|   |   |   |-- lib/index.ts
|   |   |-- tests/unit/.gitkeep
|   |
|   |-- worker/
|       |-- package.json
|       |-- tsconfig.json
|       |-- src/
|       |   |-- main.ts
|       |   |-- queues/index.ts
|       |   |-- jobs/{ingestion,relevance,readiness,resume,notifications,analytics}/index.ts
|       |   |-- schedulers/index.ts
|       |   |-- connectors/job-sources/index.ts
|       |   |-- providers/{ai,email,storage}/index.ts
|
|-- packages/
|   |-- db/
|   |   |-- package.json
|   |   |-- tsconfig.json
|   |   |-- prisma/schema.prisma
|   |   |-- src/client.ts
|   |
|   |-- modules/
|   |   |-- package.json
|   |   |-- tsconfig.json
|   |   |-- {auth-profile,job-tracker,readiness,resume,notifications,analytics}/
|   |       |-- src/{domain,application,infrastructure,contracts}/index.ts
|   |
|   |-- ai-gateway/
|   |   |-- package.json
|   |   |-- tsconfig.json
|   |   |-- src/
|   |       |-- index.ts, model-router.ts
|   |       |-- providers/{openrouter.free,groq.free,huggingface}.ts
|   |       |-- fallback/{rule-based,templates}.ts
|   |       |-- cache/prompt-cache.ts
|   |
|   |-- events/
|   |   |-- package.json
|   |   |-- tsconfig.json
|   |   |-- src/outbox.ts, event-types.ts
|   |
|   |-- shared/
|   |   |-- package.json
|   |   |-- tsconfig.json
|   |   |-- src/{types,errors,logger,utils,validators}/index.ts
|   |
|   |-- config/
|       |-- package.json
|       |-- tsconfig.json
|       |-- src/{env,feature-flags,security}.ts
|
|-- infra/
|   |-- docker/postgres/init.sql
|   |-- scripts/{up-local,down-local,reset-local}.sh
|
|-- docs/
|   |-- prd/README.md
|   |-- architecture/README.md
|   |-- runbooks/README.md
|   |-- testing/README.md
|
|-- scripts/README.mdt
