---
tags: [projeto/regras]
---

# 🧠 Contexto e Regras de Ouro

## 📏 Regras de Negócio

### 💰 Transações
- **Tipos:** Existem apenas dois tipos: `income` (Receita) e `expense` (Despesa).
- **Status:** Despesas podem ser `paid` (Paga) ou `pending` (A pagar). Receitas são sempre consideradas pagas.
- **Recorrência:** O sistema projeta transações futuras (Mensal, Semanal, Anual) para visualização no saldo do mês, mas estas só se tornam registros reais se "lançadas".
- **Saldo do Mês:** Calculado como: `Receitas - Despesas Pagas`. O valor "A Pagar" é exibido como um alerta, mas não subtraído do saldo realizado.

### 🎯 Metas
- **Aportes:** Metas não são transações diretas na tabela de transações; elas possuem um saldo próprio (`valor_atual`).
- **Conclusão:** Uma meta é considerada concluída quando `valor_atual >= valor_alvo`.

### 👥 Membros
- Toda transação e meta deve estar obrigatoriamente vinculada a um membro para permitir a filtragem e relatórios por pessoa.

## 🛠️ Regras de Desenvolvimento
- **CSS:** Priorizar variáveis CSS (`--accent`, `--bg`, etc.) para manter a consistência visual.
- **Mobile First:** A interface deve ser testada e otimizada para a largura de um smartphone (máx 430px).
- **Sem Dependências Desnecessárias:** Evitar adicionar frameworks JS (como React ou Vue) para manter o projeto leve e carregamento instantâneo.
