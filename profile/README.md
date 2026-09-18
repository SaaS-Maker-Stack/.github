<div align="center">

<img src="https://raw.githubusercontent.com/SaaS-Maker-Stack/saas-maker/main/docs/assets/brand/logo-banner.png" alt="SaaS Maker" width="480">

**Open-source starter for multi-tenant SaaS products — FastAPI + PostgreSQL backend, React 19 + shadcn/ui frontend, admin panel, Kamal deploys. Brand it, add your modules, ship.**

Auth · organizations · roles · invitations · email verification · sessions · admin panel — done before you write a line

</div>

```bash
uvx saas-maker new my-saas
uvx saas-maker generate module invoice --fields "number:str,amount:float,due:date?" --status "draft,sent,paid"
```

One command gives you three configured services (API, tenant app, admin panel), each
its own repo, with the database created and migrated, the brand color applied, and
Kamal ready. `generate module` adds a tenant-scoped CRUD — table, API, page, sidebar
entry and tests on both sides — in seconds, following one non-negotiable rule: every
query filters by organization, other tenants get 404.

> Built from the boilerplate behind several real products; extracted, cleaned up and
> open-sourced so the next one starts on day one.

| | |
|---|---|
| 🚀 Start here | [`saas-maker`](https://github.com/SaaS-Maker-Stack/saas-maker) — the template: docs, design system, submodules |
| 📦 The generator | [`cli`](https://github.com/SaaS-Maker-Stack/cli) on [PyPI](https://pypi.org/project/saas-maker/) |
| 🧠 The API | [`backend`](https://github.com/SaaS-Maker-Stack/backend) — FastAPI + SQLModel + Alembic + PostgreSQL |
| 🖥 The tenant app | [`frontend`](https://github.com/SaaS-Maker-Stack/frontend) — React 19 + Vite + shadcn/ui + Tailwind 4 |
| 🎛 The admin panel | [`admin`](https://github.com/SaaS-Maker-Stack/admin) — platform admins, separate auth |
| 🤖 Agent skills | [`skills`](https://github.com/SaaS-Maker-Stack/skills) — teach Claude Code, Cursor or Codex the conventions (`npx skills add SaaS-Maker-Stack/skills`) |

Currently **v0.1** — issues and feedback are very welcome. Apache-2.0.
