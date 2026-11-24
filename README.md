# projeto IA — pnpm workspace

Monorepo com pnpm workspaces: React (Vite) em `apps/web` e NestJS em `apps/api`.

## Requisitos

- Node.js 20+
- [pnpm](https://pnpm.io) 9+

## Instalação

Na raiz do monorepo:

```bash
pnpm install
```

## Scripts na raiz

| Script | Descrição |
|--------|-----------|
| `pnpm dev:web` | Vite/React em modo desenvolvimento (`apps/web`) |
| `pnpm dev:api` | NestJS `start:dev` (`apps/api`) |
| `pnpm build:web` | Build de produção do frontend |
| `pnpm build:api` | Build de produção da API |
| `pnpm start:web` | Preview do build Vite |
| `pnpm start:api` | Sobe a API compilada (`start:prod`) |

Os atalhos usam `pnpm --filter` com os pacotes `@projeto/web` e `@projeto/api`.

## Estrutura

```
.
├── apps/
│   ├── web/   # React + Vite (TypeScript)
│   └── api/   # NestJS (TypeScript)
├── package.json
├── pnpm-workspace.yaml
└── pnpm-lock.yaml
```
