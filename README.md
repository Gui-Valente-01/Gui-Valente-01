<div align="center">

Guilherme Valente

Desenvolvedor Full Stack

Construo sistemas de gestão que entram em produção.

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1000&color=FF9142&center=true&vCenter=true&width=850&lines=PHP+8.2+%E2%80%A2+Laravel+12+%E2%80%A2+Vue+3;Next.js+%E2%80%A2+React+%E2%80%A2+TypeScript;SaaS+%E2%80%A2+PostgreSQL+%E2%80%A2+Supabase;Do+banco+ao+deploy." alt="Typing SVG" />

<br/>





</div>

> whoami

Sou o Guilherme Valente, de Apucarana-PR.

Em 18 meses programando, construí 8 sistemas completos, passando por modelagem de banco, backend, frontend, autenticação, integrações, testes e deploy.

Hoje meu foco principal está em:

PHP 8.2
Laravel 12
Vue 3
MySQL / MariaDB
APIs REST
Arquitetura de sistemas

Mas minha experiência também inclui:

Next.js React TypeScript PostgreSQL Supabase Prisma Stripe Cloudflare Vercel

📊 Painel

<div align="center">

Indicador

Valor

Commits

264

Sistemas

8

Meses de código

18

Testes automatizados

61+

</div>

01 — Ritmo de trabalho

Commits por mês

Mar 2026   ███                                  6
Abr 2026   ████                                 7
Mai 2026   █████████████████████████           58
Jun 2026   ██████████████████                  41
Jul 2026   ███████████████████████████         64
Ago 2026   ██████████████████████████████████  88

Agosto de 2026 já era o maior mês quando os dados foram medidos em 24/08.

02 — Minha evolução

Período

Marco

Fev 2025

Primeiras linhas em C na faculdade

Out 2025

Primeiro repositório e início do versionamento com Git

Mar 2026

Python e Node — transição para aplicações web

Mai 2026

Primeiro SaaS: Eventify AI

Jun–Jul 2026

ConfecControl, CaseFlow e Gestão Escolar em paralelo

Ago 2026

Migração do foco para PHP, Laravel 12 e Vue 3

03 — Tecnologias

Backend








Frontend








Dados






Qualidade & Infra










04 — Projetos

🟠 Kanban FAP

Foco atual • Laravel + Vue

Quadros Kanban compartilhados entre usuários, com API REST em Laravel e SPA em Vue. Cards possuem responsável, prazo, etiquetas, checklists, comentários e histórico de ações.

Métricas: 9 commits • 197 arquivos • 61 testes

Stack

Laravel 12 PHP 8.2 Sanctum 4 Vue 3 Pinia 3 Vite 6 MariaDB

Destaques técnicos

Mover card com transação e lock de linha
Executado com DB::transaction, tentativas de retry e lockForUpdate para evitar conflitos em movimentações simultâneas.

app/Services/CardPositioner.php

7 Policies com bloqueio em cascata
Autorização distribuída em controllers e policies, com bloqueio herdado por estrutura.

app/Policies/CardPolicy.php

Drag and drop escrito do zero
Pointer Events para mouse e toque, limiar de movimento e auto-scroll com requestAnimationFrame.

resources/js/composables/useArrastarCards.js



🏭 ConfecControl

ERP multiempresa

ERP web para confecções: do pedido ao chão de fábrica e ao financeiro, com várias empresas no mesmo sistema e planos por funcionalidade.

Métricas: 105 commits • 280 arquivos • 35 testes

Stack

Next.js 16 React 19 TypeScript Prisma 6 PostgreSQL Playwright Sentry

Destaques técnicos

Recebimento idempotente em transação Serializable
Baixas financeiras protegidas contra duplicidade, com chave de idempotência.

src/app/financeiro/actions.ts

Matriz de 27 capacidades no servidor
Plano e cargo são transformados em permissões verificadas no backend.

src/lib/capabilities.ts

Anexo validado por magic bytes
O arquivo é validado pelo conteúdo binário, não apenas pela extensão.

src/lib/upload-validation.ts



⚖️ CaseFlow

SaaS jurídico • Código privado

Gestão de processos para escritórios de advocacia, com portal próprio para o cliente acompanhar seus casos.

Métricas: 50 commits • 210 arquivos • 26,7k linhas

Stack

Next.js 16 React 19 Supabase PostgreSQL + RLS Stripe Sentry GitHub Actions

Destaques técnicos

Integração com o DataJud do CNJ
Consome a API pública de processos do Conselho Nacional de Justiça.

src/lib/datajud.ts

Sincronização de andamentos com deduplicação por hash
Cron busca novas movimentações sem duplicar registros.

src/lib/court-sync.ts

RLS multi-tenant testado em SQL
Harness próprio para provar que um escritório não consegue ler dados de outro.

docs/rls-test-harness.sql

🔒 Repositório privado. Código disponível para demonstração em conversa técnica.

🤖 Eventify AI

IA + Pagamentos

Geração de sites de eventos por IA, do briefing ao link pago e publicado, incluindo confirmação de presença.

Métricas: 29 commits • 167 arquivos • 8 testes

Stack

Next.js 16 React 19 Google Gemini Supabase Stripe Vitest

Destaques técnicos

Webhook Stripe verificado manualmente
Assinatura HMAC conferida sem SDK pesado e proteção contra replay.

lib/stripeWebhook.ts

Pipeline de 9 agentes
Agentes especializados montam partes do briefing antes da geração final.

lib/agents/orchestrator.ts

28 policies de RLS
A regra de negócio também é protegida no banco.

supabase/migrations/



🎓 Gestão Escolar

No ar • 6 perfis de acesso

Sistema para notas, frequência, ocorrências e comunicação com a família. Cada perfil vê somente sua área.

Métricas: 20 commits • 144 arquivos • 24 modelos

Stack

Next.js 14 Prisma 5 PostgreSQL Zod Recharts Vitest

Destaques técnicos

Autorização em 3 camadas
Rota, action e vínculo de dados.

src/services/teacher.service.ts

Gerador de PDF escrito manualmente
Objetos, stream de texto, paginação e tabela xref construídos diretamente.

src/lib/export.ts

Correção de problema N+1
Consultas agregadas para reduzir múltiplas leituras.

src/services/teacher.service.ts




👕 El Roi

E-commerce

Loja de streetwear com checkout Stripe, painel administrativo e controle de estoque.

Métricas: 13 commits • 73 arquivos • 4,5k linhas

Stack

Next.js 14 TypeScript Supabase Stripe Zustand Zod

Destaques técnicos

Preços revalidados no servidor
O preço final vem do banco, não do valor enviado pelo navegador.

src/app/api/checkout/route.ts

Sessão admin HMAC-SHA256
Sessão assinada com WebCrypto.

src/lib/admin-session.ts

Rollback quando o Stripe falha
Evita pedidos órfãos em caso de falha na abertura da sessão de pagamento.

src/app/api/checkout/route.ts



♻️ EcoApuca

Edge computing • CI ativo

Sistema de reciclagem com pontos para Apucarana: cidadão acumula, operador valida e a gestão acompanha.

Métricas: 7 commits • 38 arquivos • CI ativo

Stack

React 19 Vite 8 Cloudflare Workers Drizzle ORM GitHub Actions

Destaques técnicos

Um componente, dois alvos de build
O mesmo React gera versão dinâmica e estática.

vite.static.config.ts

Teste do Worker buildado
O teste sobe o artefato real com bindings simulados.

tests/rendered-html.test.mjs

Deploy automatizado

.github/workflows/deploy.yml



💍 Casamento

JavaScript puro • Sem servidor de aplicação

Site de casamento com painel de edição próprio e confirmação de presença.

Métricas: 8 commits • 12 arquivos • JS puro

Stack

JavaScript ES6 Supabase PL/pgSQL pgcrypto GitHub Pages

Destaques técnicos

Acesso somente por SECURITY DEFINER

supabase/migration.sql

Senha com bcrypt dentro do PostgreSQL

supabase/migration.sql

Fallback offline
Nuvem → localStorage → conteúdo padrão.

assets/js/cloud.js



🧠 Como eu construo software

PROBLEMA
   ↓
REGRA DE NEGÓCIO
   ↓
MODELAGEM DE DADOS
   ↓
BACKEND / API
   ↓
FRONTEND
   ↓
AUTORIZAÇÃO & SEGURANÇA
   ↓
TESTES
   ↓
DEPLOY
   ↓
USO REAL

📈 GitHub

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Gui-Valente-01&show_icons=true&theme=github_dark&hide_border=true" />

<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Gui-Valente-01&layout=compact&theme=github_dark&hide_border=true" />

<br/>

<img src="https://streak-stats.demolab.com?user=Gui-Valente-01&theme=github-dark-blue&hide_border=true" />

</div>

📬 Contato

<div align="center">

Vamos conversar.

Estou em Apucarana-PR e disponível para oportunidades como desenvolvedor.







<br/>

BUILD • TEST • SHIP • EVOLVE

</div>
