# Guilherme Valente

**Desenvolvedor Full Stack** · Apucarana-PR

Construo sistemas de gestão que entram em produção. Em 18 meses programando, entreguei
8 sistemas completos — do modelo do banco ao deploy — para confecção, escola, escritório
de advocacia, e-commerce e eventos.

Hoje meu trabalho está em **PHP, Laravel e Vue**.

### 🔗 [Ver o portfólio completo →](https://gui-valente-01.github.io)

---

## Onde estou agora

```
Backend    PHP 8.2 · Laravel 12 · Sanctum · Node.js · TypeScript
Frontend   Vue 3 · Pinia · Vue Router · React 19 · Tailwind CSS
Dados      MySQL/MariaDB · PostgreSQL · Eloquent · Prisma · Supabase
Qualidade  PHPUnit · Vitest · Playwright · GitHub Actions
```

## Projetos

| Projeto | O que é | Stack |
|---|---|---|
| **[Kanban FAP](https://github.com/Gui-Valente-01/kanban-fap)** | Quadros colaborativos com arrastar e soltar, checklists e histórico de ações | Laravel 12 · Vue 3 · Pinia · MariaDB |
| **[ConfecControl](https://github.com/Gui-Valente-01/ConfecControl)** | ERP multiempresa para confecções: do pedido ao chão de fábrica e ao financeiro | Next.js 16 · Prisma 6 · PostgreSQL · Playwright |
| **CaseFlow** _(repositório fechado)_ | SaaS jurídico com portal do cliente e integração com o DataJud do CNJ | Next.js 16 · Supabase · RLS · Stripe |
| **[Eventify AI](https://github.com/Gui-Valente-01/eventify-ai)** | Gera o site de um evento por IA, do briefing ao link pago | Next.js 16 · Gemini · Stripe · Supabase |
| **[Gestão Escolar](https://github.com/Gui-Valente-01/Gestao-Escolar)** | Notas, frequência e comunicação com a família, com 6 perfis de acesso | Next.js · Prisma · PostgreSQL |
| **[El Roi](https://github.com/Gui-Valente-01/El-Roi)** | Loja de streetwear com checkout Stripe e controle de estoque | Next.js · Supabase · Stripe |
| **[EcoApuca](https://github.com/Gui-Valente-01/EcoApuca)** | Reciclagem com pontos, rodando na borda da Cloudflare | React 19 · Vite 8 · Workers · Drizzle |
| **[Casamento](https://github.com/Gui-Valente-01/Casamento)** | Site com painel de edição próprio, publicado sem servidor | JavaScript · Supabase · PL/pgSQL |

## Algumas decisões técnicas que valem o clique

- **Reposicionamento de card com lock de linha** — transação com `lockForUpdate` para que duas
  requisições simultâneas não dupliquem nem percam card · [`CardPositioner.php`](https://github.com/Gui-Valente-01/kanban-fap/blob/main/app/Services/CardPositioner.php)
- **Recebimento idempotente em transação Serializable** — o maior risco de um financeiro é cobrar
  duas vezes · [`financeiro/actions.ts`](https://github.com/Gui-Valente-01/ConfecControl/blob/main/src/app/financeiro/actions.ts)
- **Arrastar e soltar sem biblioteca** — Pointer Events cobrindo mouse e toque no mesmo caminho, com
  auto-scroll · [`useArrastarCards.js`](https://github.com/Gui-Valente-01/kanban-fap/blob/main/resources/js/composables/useArrastarCards.js)
- **Gerador de PDF escrito byte a byte** — boletim sem nenhuma biblioteca de PDF, a partir da
  leitura do formato · [`export.ts`](https://github.com/Gui-Valente-01/Gestao-Escolar/blob/main/src/lib/export.ts)

## Contato

[![E-mail](https://img.shields.io/badge/E--mail-gui.valente2105@gmail.com-B4530A?style=flat-square&logo=gmail&logoColor=white)](mailto:gui.valente2105@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-guivalente-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/guivalente)
[![Portfólio](https://img.shields.io/badge/Portfólio-gui--valente--01.github.io-1B2836?style=flat-square&logo=github&logoColor=white)](https://gui-valente-01.github.io)
