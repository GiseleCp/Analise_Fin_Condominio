# Dashboard Financeiro — Condomínio

## Visão Geral

Dashboard interativo para análise do extrato financeiro de condomínio, cobrindo o período de **Setembro/2025 a Março/2026**.

## Indicadores (KPIs)

| Indicador | Valor |
|-----------|-------|
| Total Receitas | R$ 775.468,01 |
| Total Despesas | R$ 778.025,24 |
| Saldo | -R$ 2.557,23 |
| Unidades | 332 |
| Fornecedores | 45 |
| Ticket Médio | R$ 341,77 |
| Transações | 2.276 |

## Funcionalidades

- **KPIs resumidos** — Receitas, despesas, saldo, unidades e ticket médio em cards animados.
- **Gráfico mensal** — Comparativo de receitas vs despesas por mês (BarChart).
- **Evolução do saldo** — Linha temporal do saldo acumulado (AreaChart).
- **Distribuição por fornecedor** — Top 6 fornecedores por volume de gastos (PieChart).
- **Tabela de despesas** — Listagem completa com filtro por fornecedor e busca por descrição.

## Tecnologias

- **React 18** + **TypeScript**
- **Tailwind CSS** com design system customizado
- **Recharts** para visualizações
- **shadcn/ui** para componentes base
- **Vite** como bundler

## Fonte dos Dados

Dados extraídos do arquivo `extrato_modelo_dimensional_PROJETO.xlsx`, contendo as dimensões:

- `f_Conta_Corrente` — fato com todas as transações
- `d_Fornecedor` — dimensão de fornecedores
- `d_Unidades` — dimensão de unidades condominiais

## Como executar

```bash
npm install
npm run dev
```

Acesse `http://localhost:5173` no navegador.

## Deploy

O projeto está publicado em: https://analise-fin-condominio.lovable.app
