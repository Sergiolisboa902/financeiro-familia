---
tags: [projeto/arquitetura]
---

# 🏗️ Arquitetura do Sistema

## 🏗️ Estrutura Geral
O projeto segue uma arquitetura de **Single Page Application (SPA)** sem frameworks pesados, priorizando performance e simplicidade de manutenção.

## 💻 Stack Tecnológica
- **Frontend:** HTML5, CSS3 (Vanilla com variáveis CSS para tematização), JavaScript (ES6+).
- **Backend as a Service (BaaS):** [Supabase](https://supabase.com/) para autenticação (planejado), banco de dados PostgreSQL e políticas de segurança (RLS).
- **Bibliotecas Externas:**
  - `supabase-js`: Integração direta com o banco de dados.
  - `xlsx`: Exportação de relatórios para Excel.
  - Google Fonts (DM Sans, DM Serif Display): Tipografia.

## 🗄️ Modelo de Dados
O banco de dados PostgreSQL no Supabase está estruturado em três tabelas principais:
1.  **`membros`**: Armazena os perfis da família (nome, cor de identificação).
2.  **`transacoes`**: Registro de receitas e despesas, incluindo recorrência e status de pagamento.
3.  **`metas`**: Objetivos financeiros com rastreio de valor atual vs. alvo.

## 🔄 Fluxo de Dados
1.  O usuário interage com a interface (DOM).
2.  O JavaScript captura o evento e realiza chamadas assíncronas ao Supabase via SDK.
3.  O estado local (`txs`, `members`, `goals`) é atualizado após a confirmação do backend.
4.  A função `render...` correspondente atualiza o componente visual no DOM sem recarregar a página.
