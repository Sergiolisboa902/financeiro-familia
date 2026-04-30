
---

### 📅 2026-04-30
#### O que foi feito:
- **Correções Críticas de Bug:**
    - Erro 400 no Supabase causado pela tentativa de inserir a coluna inexistente `parcelas`.
    - TypeError no DOM (`Cannot read properties of null (reading 'style')`) causado por acessos inseguros a elementos inexistentes (`setup` e `mainApp`).
- **Melhorias de UX/UI:**
    - Correção do modal de edição: o campo de descrição não é mais limpo ao trocar a categoria.
    - Correção do botão "Excluir Lançamento" garantindo o uso do `editId` correto.
- **Novas Funcionalidades:**
    - Segmentação de visualização na aba "Contas": receitas projetadas agora aparecem separadas das despesas, facilitando o planejamento financeiro.

#### Mudanças Técnicas:
- Remoção definitiva de referências à coluna `parcelas` no `index.html`.
- Refatoração do `DOMContentLoaded` para uma inicialização defensiva.
- Adicionada função `getProjectedTxs` para melhor modularização das projeções.
- Atualização na lógica de exclusão no Supabase (`deleteTx`).

#### Próximos Passos:
1. Avaliar feedback do usuário sobre a segmentação das receitas/despesas projetadas.
2. Monitorar performance pós-refatoração do boot.
3. Iniciar o planejamento da Fase 2 (Autenticação).

---

tags: [projeto/diario]

---

### 📅 2026-04-30
#### O que foi feito:
- **Correções Críticas de Bug:**
    - Erro 400 no Supabase causado pela tentativa de inserir a coluna inexistente `parcelas`.
    - TypeError no DOM (`Cannot read properties of null (reading 'style')`) causado por acessos inseguros a elementos inexistentes (`setup` e `mainApp`).
- **Melhorias de UX/UI:**
    - Correção do modal de edição: o campo de descrição não é mais limpo ao trocar a categoria.
    - Correção do botão "Excluir Lançamento" garantindo o uso do `editId` correto.
- **Novas Funcionalidades:**
    - Segmentação de visualização na aba "Contas": receitas projetadas agora aparecem separadas das despesas, facilitando o planejamento financeiro.

#### Mudanças Técnicas:
- Remoção definitiva de referências à coluna `parcelas` no `index.html`.
- Refatoração do `DOMContentLoaded` para uma inicialização defensiva.
- Adicionada função `getProjectedTxs` para melhor modularização das projeções.
- Atualização na lógica de exclusão no Supabase (`deleteTx`).

#### Próximos Passos:
1. Avaliar feedback do usuário sobre a segmentação das receitas/despesas projetadas.
2. Monitorar performance pós-refatoração do boot.
3. Iniciar o planejamento da Fase 2 (Autenticação).

---


# 📓 Diário de Bordo (Evoluções)

## 🌟 Estado Atual
O projeto é um protótipo funcional e integrado a um backend real (Supabase). Todas as funcionalidades principais de controle financeiro estão operacionais.


---

### 📅 2026-04-30
#### O que foi feito:
- **Correções Críticas de Bug:**
    - Erro 400 no Supabase causado pela tentativa de inserir a coluna inexistente `parcelas`.
    - TypeError no DOM (`Cannot read properties of null (reading 'style')`) causado por acessos inseguros a elementos inexistentes (`setup` e `mainApp`).
- **Melhorias de UX/UI:**
    - Correção do modal de edição: o campo de descrição não é mais limpo ao trocar a categoria.
    - Correção do botão "Excluir Lançamento" garantindo o uso do `editId` correto.
- **Novas Funcionalidades:**
    - Segmentação de visualização na aba "Contas": receitas projetadas agora aparecem separadas das despesas, facilitando o planejamento financeiro.

#### Mudanças Técnicas:
- Remoção definitiva de referências à coluna `parcelas` no `index.html`.
- Refatoração do `DOMContentLoaded` para uma inicialização defensiva.
- Adicionada função `getProjectedTxs` para melhor modularização das projeções.
- Atualização na lógica de exclusão no Supabase (`deleteTx`).

#### Próximos Passos:
1. Avaliar feedback do usuário sobre a segmentação das receitas/despesas projetadas.
2. Monitorar performance pós-refatoração do boot.
3. Iniciar o planejamento da Fase 2 (Autenticação).

---


### 📅 2026-04-29
#### O que foi feito:
- **Sincronização de Contexto:** Análise profunda de todo o código fonte e estrutura do banco de dados.
- **Documentação Técnica:** Preenchimento completo dos documentos de Visão, Arquitetura, Contexto e Roadmap.
- **Estabelecimento do Diário:** Transformação deste arquivo no registro oficial de evoluções.

#### Mudanças Técnicas:
- Consolidação das informações de infraestrutura do Supabase.
- Mapeamento das regras de cálculo de saldo e recorrência.
- **Preparação para Deploy:** Renomeado `familia-financas.html` para `index.html` e atualizadas todas as referências internas para garantir compatibilidade com o Vercel.
- **Branding:** Renomeado o sistema de "Família $" para "Planeja+".

#### Próximos Passos:
1. Revisar as funções de cálculo no frontend para garantir precisão matemática.
2. Limpar códigos mortos ou comentários obsoletos no `index.html`.
3. Iniciar o planejamento da Fase 2 (Autenticação).


---

### 📅 2026-04-30
#### O que foi feito:
- **Correções Críticas de Bug:**
    - Erro 400 no Supabase causado pela tentativa de inserir a coluna inexistente `parcelas`.
    - TypeError no DOM (`Cannot read properties of null (reading 'style')`) causado por acessos inseguros a elementos inexistentes (`setup` e `mainApp`).
- **Melhorias de UX/UI:**
    - Correção do modal de edição: o campo de descrição não é mais limpo ao trocar a categoria.
    - Correção do botão "Excluir Lançamento" garantindo o uso do `editId` correto.
- **Novas Funcionalidades:**
    - Segmentação de visualização na aba "Contas": receitas projetadas agora aparecem separadas das despesas, facilitando o planejamento financeiro.

#### Mudanças Técnicas:
- Remoção definitiva de referências à coluna `parcelas` no `index.html`.
- Refatoração do `DOMContentLoaded` para uma inicialização defensiva.
- Adicionada função `getProjectedTxs` para melhor modularização das projeções.
- Atualização na lógica de exclusão no Supabase (`deleteTx`).

#### Próximos Passos:
1. Avaliar feedback do usuário sobre a segmentação das receitas/despesas projetadas.
2. Monitorar performance pós-refatoração do boot.
3. Iniciar o planejamento da Fase 2 (Autenticação).

---


### 📅 2026-04-27
- Inicialização dos arquivos de documentação do projeto.
- Criação do repositório e estrutura básica de diretórios.
