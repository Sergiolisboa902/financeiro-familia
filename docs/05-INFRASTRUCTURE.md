---
tags: [projeto/infra]
---

# 🛠️ Infraestrutura e Configuração

## 🌐 Ambiente de Hospedagem
- **Frontend:** Pode ser hospedado em qualquer provedor de estáticos (Vercel, Netlify, GitHub Pages).
- **Backend/Banco de Dados:** [Supabase](https://supabase.com/).

## 🗄️ Banco de Dados (Supabase/PostgreSQL)
O esquema está definido no arquivo `supabase-schema.sql`.

### Tabelas Principais:
- **`membros`**: `id`, `nome`, `cor`.
- **`transacoes`**: `id`, `tipo`, `valor`, `descricao`, `data`, `categoria`, `membro_id`, `recorrencia`, `status`, `data_vencimento`.
- **`metas`**: `id`, `nome`, `valor_alvo`, `valor_atual`, `prazo`, `cor`.

## ⚙️ Configuração Local
Para rodar o projeto localmente:
1. Abra o arquivo `index.html` diretamente no navegador (ou via Live Server).
2. As credenciais do Supabase estão em `supabase-config.js`.

> ⚠️ **Atenção:** Atualmente as chaves do Supabase estão expostas no código (Client Side). Para produção, recomenda-se configurar políticas de RLS restritivas.

## 📦 Dependências Externas (CDNs)
- Supabase SDK: `https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2`
- XLSX: `https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js`
- Google Fonts: `DM Sans` e `DM Serif Display`.
