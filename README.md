# 📊 Dashboards de Vendas & Faturamento — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/status-ativo-brightgreen?style=flat-square)
![DAX](https://img.shields.io/badge/linguagem-DAX%20|%20M-blue?style=flat-square)

Dashboards interativos desenvolvidos no **Power BI** para análise de vendas, faturamento e desempenho operacional no varejo.

---

## 🎯 Sobre o Projeto

Este repositório reúne dashboards com foco em análise de **vendas e faturamento para o varejo**. Os painéis foram construídos com identidade visual própria — tema escuro com paleta **vermelho, preto e dourado** — garantindo uma experiência profissional e de alto impacto visual.

---

## 🖥️ Dashboards incluídos

### 📍 Painel de Vendas por Período
Análise das vendas segmentadas por **dia da semana**, **mês** e **turno** (manhã, tarde e noite), com visão de faturamento mensal e anual.

### 🏪 Rank de Vendas por Turno
Ranking dos produtos mais vendidos em cada turno do dia — **Manhã**, **Tarde** e **Noite** — com filtros por seção e produto.

### 🏆 Faturamento por Departamento
Visão consolidada do faturamento agrupado por **departamento**, **seção** e **filial**, com comparativo mensal e indicadores de desempenho.

### 📋 Relatório de Estabelecimentos
Tabela detalhada com faturamento total, faturamento mensal, por turno e média diária por estabelecimento.

### 📈 Faturamento Período × Mês
Gráfico de barras com evolução do faturamento ao longo dos meses, com drill-down por período.

---

## 🛠️ Técnicas utilizadas

- **DAX avançado** — medidas calculadas, KPIs, ranking dinâmico, comparativos YoY e MoM
- **Power Query (M)** — transformações, junções entre fontes, limpeza e padronização de dados
- **Modelagem em estrela** — tabelas fato + dimensões (tempo, produto, estabelecimento, seção)
- **Visuais customizados** — tema escuro com identidade visual personalizada (vermelho/preto/dourado)
- **Filtros dinâmicos** — segmentadores por data, turno, departamento, seção e produto

---

## 💡 Exemplos de DAX aplicados

```dax
-- Faturamento Total
Faturamento Total = SUM(Vendas[Valor])

-- Ranking de Produtos por Turno
Rank Produto Turno =
RANKX(
    ALLSELECTED(Produto[Descrição]),
    [Faturamento Total],
    ,
    DESC,
    DENSE
)

-- Crescimento MoM
Crescimento MoM =
VAR MesAtual = [Faturamento Total]
VAR MesAnterior = CALCULATE([Faturamento Total], DATEADD(Calendario[Data], -1, MONTH))
RETURN DIVIDE(MesAtual - MesAnterior, MesAnterior, 0)

-- Faturamento Médio Diário
Fat. Médio Diário = DIVIDE([Faturamento Total], DISTINCTCOUNT(Calendario[Data]), 0)
```

---

## 📸 Preview

![Dashboard Vendas por Período](WhatsApp%20Image%202025-04-10%20at%2016.33.09%20(1).jpeg)
![Dashboard Faturamento por Estabelecimento](WhatsApp%20Image%202025-04-10%20at%2016.33.09.jpeg)

---

## 👩‍💻 Desenvolvedora

**Raquel Daud** — Analista de Dados | Power BI | SQL | DAX

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raquel-daud/)
