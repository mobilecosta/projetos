É uma plataforma web completa, construída em Next.js (App Router), para gestão de benefícios de refeição/ alimentação via vouchers digitais. Ela conecta quatro perfis principais:
Admin da plataforma
Empresas (enterprise)
Estabelecimentos (establishment)
Colaboradores (employees)
Ideal para quem quer lançar um negócio tipo “vale refeição digital” ou um sistema white‑label de benefícios corporativos. Quem tiver interesse no projeto to aceitando qualquer valor monetario e disponibilizarei o link do github ou codigo zip do projeto.  Hoje ele já ta integrado ao stripe para assinatira de clientes. Vou deixar umas telas do projeto. Obs.: projeto foi criado com auxio de agentes de AI mas que maior parte do projeto foi criado por mim.

Principais Módulos
Painel Admin
Gestão de empresas (cadastro, edição, detalhes).
Gestão global de colaboradores, estabelecimentos, departamentos, etc.
Relatórios consolidados e visão geral da operação.
Fluxos de autenticação próprios de admin, incluindo recuperação e redefinição de senha.
Painel da Empresa (Enterprise)
Gestão de colaboradores (cadastro, listagem, filtros).
Gestão de departamentos, estabelecimentos parceiros e tipos de refeição.
Módulo de relatórios e pagamentos com:
filtros por período, status e estabelecimento,
exportação de dados para Excel,
visão de tokens/fichas utilizados.
Configurações e notificações específicas da empresa.
Painel do Estabelecimento
Visão de transações realizadas com vouchers.
Relatórios detalhados com gráficos (Recharts) e KPIs:
pagamentos, fichas processadas, status das transações etc.
Módulo de pagamentos/recebíveis, com listagem e exportação.
Relatórios por período, tipo de refeição, status, busca por colaborador.
Telas responsivas e focadas em operação diária do estabelecimento.
Área do Colaborador
Login específico de colaborador.
Acesso às informações de uso (transações, estabelecimentos, relatórios).
Fluxos de autenticação separados por tipo de usuário.
Autenticação & Segurança
Múltiplos fluxos de login:
Admin
Enterprise
Establishment
Collaborator
Recuperação de senha com token via URL (reset password).
Honeypot simples anti‑bot em formulários sensíveis.
Uso de JWT/ sessão (via rotas em api/auth/..., prontas para integrar com qualquer provider de e‑mail/senha).
Faturamento com Stripe
Integração pronta com Stripe para cobrança recorrente:
create-checkout-session para assinatura.
create-portal-session para o cliente gerenciar a assinatura.
Webhook /api/stripe/webhook para eventos de cobrança.
Ideal para transformar o Digivoucher em SaaS de assinatura.
Stack Técnica
Frontend / Backend
Next.js 15 (App Router) com Turbopack.
React 19.
Estrutura moderna de pastas /src/app com rotas server e client components.
Banco & ORM
Prisma ORM (prisma/client + prisma), com estrutura pronta de lib/prisma.
Migrations e scripts configurados:
prisma:generate
prisma:migrate
prisma:studio
UI e Componentes
Radix UI (radix-ui/react-*) como base de acessibilidade.
Componentes de UI prontos (buttons, inputs, cards, tabs, tooltips, etc.).
Ícones com Lucide e Tabler Icons.
Gráficos com Recharts e ApexCharts.
Sistema de notificações com sonner.
Layouts modernos, responsivos e com foco em usabilidade em desktop e mobile.
Outros Destaques Técnicos
Integração com Upstash Redis + Ratelimit (já preparada no package.json) para rate limiting.
Uso de Zod para validação de formulários e regras de negócio.
Exportação de relatórios para Excel (xlsx).
Arquitetura de APIs REST em /api/... bem organizada por domínio (auth, collaborators, enterprise, establishment, billing, etc.).
Benefícios para Quem Comprar
Produto quase pronto para produção:
Estrutura completa de autenticação, multi‑painel, relatórios, pagamentos e faturamento via Stripe.
Base sólida para um SaaS de benefícios:
Já dividido em papéis (admin, empresa, estabelecimento, colaborador).
Fácil de customizar branding e regras de negócio específicas.
Tecnologias modernas e bem suportadas:
Next.js 15, React 19, Prisma, Stripe, Radix UI.
Facilita encontrar desenvolvedores e manter o projeto no longo prazo.
Código organizado por domínios de negócio:
api/auth/..., api/enterprise/..., api/establishment/..., api/collaborator/...
Facilita extensão, auditoria e manutenção.
