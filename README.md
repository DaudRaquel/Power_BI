# Dashboards de Vendas e Faturamento - Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) ![Status](https://img.shields.io/badge/status-ativo-brightgreen?style=flat-square) ![DAX](https://img.shields.io/badge/linguagem-DAX%20|%20M-blue?style=flat-square)

Dashboards interativos desenvolvidos no **Power BI** para analise de vendas, faturamento e desempenho operacional no varejo.

---

## Sobre o Projeto

Este repositorio reune dashboards com foco em analise de **vendas e faturamento para o varejo**. Os paineis foram construidos com identidade visual propria - tema escuro com paleta **vermelho, preto e dourado** - garantindo uma experiencia profissional e de alto impacto visual.

---

## Dashboards incluidos

### Painel de Vendas por Periodo
Analise das vendas segmentadas por **dia da semana**, **mes** e **turno** (manha, tarde e noite), com visao de faturamento mensal e anual.

### Rank de Vendas por Turno
Ranking dos produtos mais vendidos em cada turno do dia - **Manha**, **Tarde** e **Noite** - com filtros por secao e produto.

### Faturamento por Departamento
Visao consolidada do faturamento agrupado por **departamento**, **secao** e **filial**, com comparativo mensal e indicadores de desempenho.

### Relatorio de Estabelecimentos
Tabela detalhada com faturamento total, faturamento mensal, por turno e media diaria por estabelecimento.

### Faturamento Periodo x Mes
Grafico de barras com evolucao do faturamento ao longo dos meses, com drill-down por periodo.

---

## Tecnicas utilizadas

- **DAX avancado** - medidas calculadas, KPIs, ranking dinamico, comparativos YoY e MoM
- **Power Query (M)** - transformacoes, juncoes entre fontes, limpeza e padronizacao de dados
- **Modelagem em estrela** - tabelas fato + dimensoes (tempo, produto, estabelecimento, secao)
- **Visuais customizados** - tema escuro com identidade visual personalizada (vermelho/preto/dourado)
- **Filtros dinamicos** - segmentadores por data, turno, departamento, secao e produto

---

## Exemplos de DAX aplicados

~~~dax
-- Faturamento Total
Faturamento Total = SUM(Vendas[Valor])

-- Ranking de Produtos por Turno
Rank Produto Turno =
RANKX(
    ALLSELECTED(Produto[Descricao]),
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

-- Faturamento Medio Diario
Fat. Medio Diario = DIVIDE([Faturamento Total], DISTINCTCOUNT(Calendario[Data]), 0)
~~~

---

## Preview

![Dashboard Vendas](WhatsApp%20Image%202025-04-10%20at%2016.33.09%20(1).jpeg)
![Dashboard Faturamento](WhatsApp%20Image%202025-04-10%20at%2016.33.09.jpeg)

---

## Desenvolvedora

**Raquel Daud** - Analista de Dados | Power BI | SQL | DAX

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raquel-daud/)
