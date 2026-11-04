<div align="center">

## 🇧🇷 Português · [🇺🇸 English](#english)

</div>

<p align="center"><strong>Isaac Marinho · Desenvolvedor Full-Stack · Brasil · UTC-3 · Remoto para o mundo</strong><br/>Disponível para projetos freelance e contratos remotos</p>

### Sobre

Trabalho com TypeScript em toda a stack, desde a primeira tela de um produto até workers em segundo plano, registros de pagamentos e transações de banco de dados.

Tenho experiência criando landing pages, dashboards e painéis administrativos. Também gosto especialmente dos desafios que exigem confiabilidade: novas tentativas, eventos duplicados, atualizações concorrentes, falhas parciais, entrega de webhooks e consistência dos dados.

### Da interface à infraestrutura

Quatro camadas em que atuo ao construir um produto completo — da interface à confiabilidade.

### Tecnologias principais

Ferramentas que uso e com as quais desenvolvo.

**FRONTEND**  
TypeScript · React · Next.js · Tailwind CSS

**BACKEND**  
Node.js · Express · Prisma · Stripe

**DADOS E SISTEMAS**  
PostgreSQL · Redis · BullMQ · Docker · GitHub Actions · Vitest

### Além do caminho feliz

Os desafios que mais me interessam — aqueles que fazem um software deixar de ser apenas uma demonstração:

`pagamentos duplicados` · `atualizações concorrentes de estoque` · `reenvio de webhooks` · `tarefas com falha` · `retentativas e backoff` · `falhas parciais` · `consistência dos dados` · `condições de corrida` · `idempotência` · `segurança transacional`

### Projetos selecionados

Projetos que cobrem diferentes camadas da stack.

#### Plataforma de processamento de tarefas assíncronas

Sistema multi-tenant de tarefas em segundo plano, projetado para processar trabalho com segurança mesmo diante de retentativas e falhas parciais.

**Tecnologias:** TypeScript · Node.js · Redis · BullMQ · PostgreSQL · Prisma

**Destaques de engenharia:** idempotência · retentativas e backoff · fila de falhas e reprocessamento · multi-tenancy · limites de taxa, cotas e concorrência · observabilidade · chaves de API com escopo

- Idempotência em duas camadas: restrição única no banco por (tenantId, idempotencyKey) e registros de efeitos por tarefa.
- Fila de mensagens com falha, fluxo automático de reprocessamento e endpoints de nova tentativa manual.
- Retentativas com backoff exponencial e jitter, separadas dos handlers de longa duração da API.
- Limites de taxa, cotas de tarefas e limites de concorrência por tenant.
- Métricas Prometheus, logs estruturados com IDs de correlação e auditoria completa de eventos por tarefa.
- API e workers em processos separados para escalar horizontalmente de forma independente.

**[Acessar repositório →](https://github.com/asyncisaac/async-job-processing-platform)**

#### Sistema de pagamentos — com ledger como base

Ledger imutável de saldos, com processamento idempotente de pagamentos e reembolsos.

**Tecnologias:** Node.js · Stripe · PostgreSQL · BullMQ · React

- Saldos calculados a partir de um ledger append-only (soma dos lançamentos), sem atualizações diretas.
- Idempotência garantida na API (chave única) e nos workers (registro único por evento de pagamento).
- Pipeline de retentativas e fila de falhas para confirmações e erros de pagamentos assíncronos.
- Reembolsos usam o mesmo fluxo de transição de status, com trilha de auditoria completa.
- Testes de integração para condições de corrida com dois workers em paralelo.

**[Acessar repositório →](https://github.com/asyncisaac/payment-system)**

#### Plataforma de e-commerce · Monorepo Full-Stack

Loja completa, autenticação, fluxo de checkout e painel administrativo.

**Tecnologias:** Next.js · React · Express · Prisma · PostgreSQL · Stripe Checkout

- Baixa atômica de estoque (`UPDATE ... WHERE stock >= qty`) com resposta 409 explícita em caso de concorrência.
- Idempotência de webhooks Stripe garantida por `event.id UNIQUE` no banco.
- Reserva de estoque restaurada automaticamente em pagamentos assíncronos expirados ou com falha.
- JWT e refresh tokens rotativos, com acesso administrativo baseado em funções.
- Observabilidade com logger pino, erros estruturados, endpoints de saúde e testes automatizados.

**[Acessar repositório →](https://github.com/asyncisaac/ecommerce-monorepo)**

#### Gamified Bug Tracker · projeto secundário

Rastreador de bugs com XP e níveis por severidade. Encerramento e concessão de XP em uma única transação. Next.js 15 App Router e interface otimista.

**Tecnologias:** Next.js 15 · Prisma · PostgreSQL

**[Acessar repositório →](https://github.com/asyncisaac/Gamified-Bug-Tracker)**

### O que posso desenvolver

- Aplicações Full-Stack com TypeScript
- MVPs SaaS e aplicações web
- Sites, landing pages e dashboards com Next.js
- APIs backend e lógica de domínio
- Integrações Stripe e fluxos de webhooks
- Modelagem de dados PostgreSQL e schemas Prisma
- Workers em segundo plano com Redis e BullMQ
- Fluxos de autenticação e autorização
- Refatoração e depuração de bases de código existentes
- Integrações com APIs de terceiros

### Vamos construir algo?

Disponível para projetos freelance e contratos remotos. Prefiro contato por e-mail ou LinkedIn.

<p align="center">
  <a href="mailto:isaacmarinho.dev@gmail.com">E-mail</a> ·
  <a href="https://linkedin.com/in/isaacmarinho-dev">LinkedIn</a> ·
  <a href="https://github.com/asyncisaac">GitHub</a>
</p>

<p align="right"><code>// asyncisaac · da interface à infraestrutura</code></p>

---

<a id="english"></a>

<div align="center">

## 🇺🇸 English · [🇧🇷 Português](#top)

</div>

<div align="center" id="top">
  <a href="#top">
    <picture>
      <source media="(prefers-color-scheme: dark)"  srcset="assets/hero-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="assets/hero-light.svg">
      <img src="assets/hero-light.svg" alt="asyncisaac — From Interface to Infrastructure" width="800">
    </picture>
  </a>
</div>

<br/>

<p align="center">
  <code><strong>Isaac Marinho</strong> · Full-Stack Developer · Brazil · UTC-3 · Remote Worldwide</code>
  <br/>
  <code>Open to freelance &amp; contract work</code>
</p>

<p align="center">
  <a href="https://github.com/asyncisaac"><img src="https://img.shields.io/badge/GitHub-asyncisaac-0a0a0a?style=for-the-badge&logo=github&logoColor=white&labelColor=262626&color=0891b2" alt="GitHub"/></a>
  &nbsp;
  <a href="https://linkedin.com/in/isaacmarinho-dev"><img src="https://img.shields.io/badge/LinkedIn-isaacmarinho--dev-0a0a0a?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=262626&color=0891b2" alt="LinkedIn"/></a>
  &nbsp;
  <a href="mailto:isaacmarinho.dev@gmail.com"><img src="https://img.shields.io/badge/Email-isaacmarinho.dev%40gmail.com-0a0a0a?style=for-the-badge&logo=protonmail&logoColor=white&labelColor=262626&color=0891b2" alt="Email"/></a>
</p>

---

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/section-divider-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/section-divider-light.svg">
  <img src="assets/section-divider-light.svg" width="800" alt="">
</picture>

### `//` about

I work with TypeScript across the full stack, from the first screen of a product down to
background workers, payment ledgers and database transactions.

I'm equally comfortable building a landing page, a dashboard or an admin panel — and I
pay special attention to the parts of a system where correctness matters: retries,
duplicate events, concurrent updates, partial failures, webhook delivery and data consistency.

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/section-divider-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/section-divider-light.svg">
  <img src="assets/section-divider-light.svg" width="800" alt="">
</picture>

### `//` from interface to infrastructure

Four layers I work on when building a complete product — not just one side of the stack.

<br/>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)"  srcset="assets/stack-flow-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/stack-flow-light.svg">
    <img src="assets/stack-flow-light.svg" width="800" alt="01 Interface → 02 Product → 03 Backend → 04 Reliability">
  </picture>
</div>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/section-divider-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/section-divider-light.svg">
  <img src="assets/section-divider-light.svg" width="800" alt="">
</picture>

### `//` core stack

Curated. Tools I actually use and build with.

<br/>

<div align="center">

**`FRONTEND`**

<img src="https://img.shields.io/badge/TypeScript-2b2b2b?style=for-the-badge&logo=typescript&logoColor=white&color=0e7490" alt="TypeScript"/>
&nbsp;<img src="https://img.shields.io/badge/React-2b2b2b?style=for-the-badge&logo=react&logoColor=white&color=0e7490" alt="React"/>
&nbsp;<img src="https://img.shields.io/badge/Next.js-2b2b2b?style=for-the-badge&logo=next.js&logoColor=white&color=0e7490" alt="Next.js"/>
&nbsp;<img src="https://img.shields.io/badge/TailwindCSS-2b2b2b?style=for-the-badge&logo=tailwindcss&logoColor=white&color=0e7490" alt="TailwindCSS"/>

<br/>

**`BACKEND`**

<img src="https://img.shields.io/badge/Node.js-2b2b2b?style=for-the-badge&logo=nodedotjs&logoColor=white&color=0e7490" alt="Node.js"/>
&nbsp;<img src="https://img.shields.io/badge/Express-2b2b2b?style=for-the-badge&logo=express&logoColor=white&color=0e7490" alt="Express"/>
&nbsp;<img src="https://img.shields.io/badge/Prisma-2b2b2b?style=for-the-badge&logo=prisma&logoColor=white&color=0e7490" alt="Prisma"/>
&nbsp;<img src="https://img.shields.io/badge/Stripe-2b2b2b?style=for-the-badge&logo=stripe&logoColor=white&color=0e7490" alt="Stripe"/>

<br/>

**`DATA & SYSTEMS`**

<img src="https://img.shields.io/badge/PostgreSQL-2b2b2b?style=for-the-badge&logo=postgresql&logoColor=white&color=0e7490" alt="PostgreSQL"/>
&nbsp;<img src="https://img.shields.io/badge/Redis-2b2b2b?style=for-the-badge&logo=redis&logoColor=white&color=0e7490" alt="Redis"/>
&nbsp;<img src="https://img.shields.io/badge/BullMQ-2b2b2b?style=for-the-badge&logo=queue&logoColor=white&color=0e7490" alt="BullMQ"/>
&nbsp;<img src="https://img.shields.io/badge/Docker-2b2b2b?style=for-the-badge&logo=docker&logoColor=white&color=0e7490" alt="Docker"/>
&nbsp;<img src="https://img.shields.io/badge/GitHub_Actions-2b2b2b?style=for-the-badge&logo=githubactions&logoColor=white&color=0e7490" alt="GitHub Actions"/>
&nbsp;<img src="https://img.shields.io/badge/Vitest-2b2b2b?style=for-the-badge&logo=vitest&logoColor=white&color=0e7490" alt="Vitest"/>

</div>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/section-divider-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/section-divider-light.svg">
  <img src="assets/section-divider-light.svg" width="800" alt="">
</picture>

### `//` beyond the happy path

The problems I find most interesting — the ones that make software stop being a demo.

<br/>

<div align="center">

`duplicate payments`
`concurrent inventory updates`
`webhook replays`
`failed jobs`
`retries & backoff`
`partial failures`
`data consistency`
`race conditions`
`idempotency`
`transaction safety`

</div>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/section-divider-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/section-divider-light.svg">
  <img src="assets/section-divider-light.svg" width="800" alt="">
</picture>

### `//` selected work

Projects that cover different layers of the stack.

---

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/flagship-banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/flagship-banner-light.svg">
  <img src="assets/flagship-banner-light.svg" width="800" alt="FLAGSHIP">
</picture>

## Async Job Processing Platform

> A multi-tenant background-job system designed to safely process work under retries and partial failures.

**Stack:**
`TypeScript` `Node.js` `Redis` `BullMQ` `PostgreSQL` `Prisma`

**Engineering highlights:**
`IDEMPOTENCY`
`RETRY / BACKOFF`
`DLQ + REPLAY`
`MULTI-TENANCY`
`RATE / QUOTA / CONCURRENCY`
`OBSERVABILITY`
`SCOPED API KEYS`

- Idempotency enforced on two layers — unique DB constraint per (tenantId, idempotencyKey) and scoped per-job effect records.
- Dead-letter queue with automatic job replay flow and manual retry endpoints.
- Retries + exponential backoff + jitter, separated from long-running API handlers.
- Per-tenant rate limits, job quotas and max concurrency caps.
- Prometheus metrics, structured logs with correlation IDs and a full per-job event audit log.
- API and workers split into separate processes for independent horizontal scaling.

**[Repository →](https://github.com/asyncisaac/async-job-processing-platform)**

---

### Payment System — Ledger-First

Immutable balance ledger with idempotent payment processing and refunds.

**Stack:**
`Node.js` `Stripe` `PostgreSQL` `BullMQ` `React`

- Balances derived from an append-only ledger (SUM of entries), never direct UPDATEs.
- Idempotency enforced at API level (unique key) and worker level (unique per-payment event row).
- Retry + dead-letter pipeline for async payment confirmations and failures.
- Refunds use the same status-transition pipeline with full audit trail.
- Concurrent race-condition integration tests with two parallel workers.

**[Repository →](https://github.com/asyncisaac/payment-system)**

---

### E-commerce Platform · Full-Stack Monorepo

Complete storefront, auth, checkout pipeline and admin panel.

**Stack:**
`Next.js` `React` `Express` `Prisma` `PostgreSQL` `Stripe Checkout`

- Atomic stock decrement (`UPDATE ... WHERE stock >= qty`) with explicit 409 on lost race.
- Stripe webhook idempotency enforced by `event.id UNIQUE` in DB.
- Stock reservation restored automatically for expired or failed async payments.
- JWT + rotating refresh tokens with role-based admin access.
- Observability hooks: pino logger, structured error payloads, health endpoints and automated tests.

**[Repository →](https://github.com/asyncisaac/ecommerce-monorepo)**

---

##### Gamified Bug Tracker · secondary / product

Bug tracker with XP / levels per severity. Single-transaction close + XP grants. Next.js 15 App Router + optimistic UI.

**Stack:** `Next.js 15` `Prisma` `PostgreSQL`

**[Repository →](https://github.com/asyncisaac/Gamified-Bug-Tracker)**

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/section-divider-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/section-divider-light.svg">
  <img src="assets/section-divider-light.svg" width="800" alt="">
</picture>

### `//` what i can build

Types of engagements that fit my stack and interests.

- Full-Stack TypeScript applications
- SaaS MVPs and web apps
- Next.js websites, landing pages & dashboards
- Backend APIs and domain logic
- Stripe integration & webhook pipelines
- PostgreSQL data modeling & Prisma schemas
- Redis / BullMQ background workers
- Authentication & authorization flows
- Refactoring & debugging existing codebases
- Third-party API integrations

<br/>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)"  srcset="assets/async-simulator-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/async-simulator-light.svg">
    <img src="assets/async-simulator-light.svg" alt="Async Pipeline Simulator — jobs crossing API → Queue → Worker, with retry and dead-letter branches" width="760">
  </picture>
</p>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="assets/section-divider-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/section-divider-light.svg">
  <img src="assets/section-divider-light.svg" width="800" alt="">
</picture>

### `//` let's build something

Open to freelance and remote contract work. Best way to reach me is email or LinkedIn.

<p align="center">
  <a href="mailto:isaacmarinho.dev@gmail.com"><img src="https://img.shields.io/badge/Send_Email-isaacmarinho.dev%40gmail.com-0a0a0a?style=for-the-badge&logo=protonmail&logoColor=white&labelColor=262626&color=0891b2" alt="Email"/></a>
  &nbsp;
  <a href="https://linkedin.com/in/isaacmarinho-dev"><img src="https://img.shields.io/badge/LinkedIn-isaacmarinho--dev-0a0a0a?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=262626&color=0891b2" alt="LinkedIn"/></a>
  &nbsp;
  <a href="https://github.com/asyncisaac"><img src="https://img.shields.io/badge/GitHub-asyncisaac-0a0a0a?style=for-the-badge&logo=github&logoColor=white&labelColor=262626&color=0891b2" alt="GitHub"/></a>
</p>

<br/>

<p align="right">
  <code>// asyncisaac · from interface to infrastructure</code>
</p>
