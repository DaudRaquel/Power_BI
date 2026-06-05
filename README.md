# 📊 Dashboards de Vendas & Faturamento — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/status-ativo-brightgreen?style=flat-square)
![DAX](https://img.shields.io/badge/linguagem-DAX%20|%20M-blue?style=flat-square)

Dashboards interativos desenvolvidos no **Power BI** para análise de vendas, faturamento e desempenho operacional no varejo — com identidade visual personalizada e construídos do zero.

---

## 🎯 Sobre o Projeto

Este repositório reúne dashboards com foco em análise de **vendas e faturamento para o varejo**. Os painéis passaram por uma **reformulação visual completa**: saindo de um layout padrão do Power BI para uma interface totalmente customizada, com tema escuro, paleta **vermelho, preto e dourado**, tipografia hierárquica, filtros estilizados e componentes redesenhados do zero.

---

## 🖥️ Dashboards incluídos

### 📍 Painel de Vendas por Período
Análise das vendas segmentadas por **dia da semana**, **mês** e **turno** (manhã, tarde e noite), com gráfico de pizza por período e visão de faturamento mensal.

### 🏪 Rank de Vendas por Turno
Ranking dos produtos mais vendidos em cada turno do dia — **Manhã**, **Tarde** e **Noite** — com filtros por seção e produto.

### 🏆 Faturamento por Departamento
Visão consolidada do faturamento agrupado por **departamento**, **seção** e **filial**, com comparativo mensal e indicadores de desempenho.

### 📋 Relatório de Estabelecimentos
Tabela detalhada com faturamento total, faturamento mensal, por turno e média diária por estabelecimento, com gráfico de barras douradas **Faturamento Mensal x Anual**.

### 📈 Faturamento Período × Mês
Gráfico de barras horizontais com evolução do faturamento ao longo dos meses, com cores alternando entre **dourado** (anos anteriores) e **vermelho** (ano atual), permitindo comparativo direto entre períodos.

---

## 🎨 Evolução Visual — Antes × Depois

O projeto passou por uma transformação visual profunda. Abaixo a comparação detalhada entre a versão original e a versão final:

### ⬅️ Antes
![Versão anterior do dashboard](WhatsApp%20Image%202025-04-10%20at%2016.33.09%20(1).jpeg)

O layout original apresentava **fundo branco** em todas as áreas de conteúdo, com painéis separados por bordas finas em cinza claro. O painel lateral de filtros tinha fundo vermelho padrão, sem qualquer customização tipográfica — os rótulos "Dia da Semana", "Dia", "Mês", "Seção" e "Produto" apareciam em fonte preta pequena sobre fundo branco, sem destaque visual. Os **dropdowns** (Sábado, Março, BEBIDA, Tudo) eram controles nativos do Power BI, com fundo branco e borda cinza. O **slider de dia** tinha aparência padrão sem estilização.

O gráfico de pizza **"Vendas por período"** usava fatias em tons de vermelho com opacidade variada, sem bordas definidas, e a legenda (Tarde, Manhã, Noite) aparecia em fonte pequena à direita sem moldura. O gráfico de barras **"Faturamento por seção"** mostrava uma única barra laranja-avermelhada sobre fundo branco, sem rótulo de valor destacado. Os três painéis de **Rank de Vendas** (Manhã, Tarde, Noturno) tinham fundo branco com texto azul-padrão de hyperlink para os nomes dos produtos, sem separação visual entre itens. O painel de **Faturamento Mensal** ao fundo era praticamente vazio — apenas um ponto vermelho e um valor pequeno, sem nenhum gráfico visível.

### ➡️ Depois
![Versão atual — Relatório de Faturamento](WhatsApp%20Image%202025-04-10%20at%2016.33.09.jpeg)

A versão reformulada aplica **tema escuro total** com canvas em preto (#0D0D0D) em todos os painéis. O **header** ganhou uma faixa vermelha intensa na parte superior com os filtros integrados — Dia (com seletor de intervalo de datas), Departamento, Seção, Produto e Pedido — todos como dropdowns com fundo branco sobre a faixa vermelha, formando um bloco de controle coeso e profissional. Abaixo do header, um **slider de data** foi posicionado em destaque sobre fundo escuro.

Os **KPIs de faturamento** (Faturamento R$, Faturamento Mensal, Faturamento Tarde e Faturamento Noite) aparecem como cartões escuros com valores em branco e títulos em cinza-claro, agrupados horizontalmente no topo da área de dados. À direita dos KPIs, o seletor de **"Ano do Gráfico"** apresenta botões estilizados (2024 em cinza, 2025 em dourado) que controlam a visualização.

O gráfico principal **"Faturamento Mensal x Anual"** é um gráfico de barras horizontais com barras em **dourado brilhante** (#F2C811) sobre fundo escuro, com rótulos de valor em branco ao lado de cada barra — permitindo leitura imediata dos totais por mês (janeiro a dezembro). A tabela de estabelecimentos ocupa a metade inferior esquerda com colunas bem definidas: Cód, Produto, Faturamento, Fat. Mensal, Fat. Tarde e Fat. Média — com linhas em tons alternados de cinza escuro e preto. O gráfico **"Faturamento Período x Mês"** no canto inferior direito exibe barras horizontais bicolores em **vermelho e dourado**, separando visualmente os dois anos de comparação.

### 📊 Comparativo detalhado

| Elemento | Antes | Depois |
|---|---|---|
| **Fundo do canvas** | Branco / cinza claro | Preto profundo (#0D0D0D) |
| **Paleta principal** | Vermelho genérico + branco | Vermelho-vivo + preto + dourado (#F2C811) |
| **Header / Barra de filtros** | Painel lateral vermelho simples | Faixa horizontal vermelha com filtros integrados |
| **Filtros / Dropdowns** | Controles nativos brancos com borda cinza | Dropdowns brancos sobre header vermelho, organizados em linha |
| **Slider de data** | Slider padrão sem estilo | Slider estilizado com marcadores sobre fundo escuro |
| **KPIs** | Ausentes — valores dispersos | Cartões escuros agrupados: Faturamento, Mensal, Tarde, Noite |
| **Gráfico de pizza** | Fatias em vermelho opaco, fundo branco | Substituído por barras horizontais douradas com rótulos |
| **Gráfico de barras** | Barra laranja única, sem rótulo | Barras horizontais douradas com valores visíveis por mês |
| **Ranking de produtos** | Texto azul hyperlink, fundo branco | Removido / integrado à tabela central estilizada |
| **Tabela de dados** | Ausente | Tabela densa com linhas alternadas escuras e colunas destacadas |
| **Comparativo anual** | Ausente | Gráfico bicolor (dourado × vermelho) por período e mês |
| **Seletor de ano** | Ausente | Botões estilizados (2024 cinza / 2025 dourado) |
| **Tipografia** | Fonte padrão, tamanho único | Hierarquia clara: títulos, subtítulos, valores e rótulos |
| **Coesão visual** | Elementos desconexos sem identidade | Identidade unificada em todos os painéis |

---

## 🛠️ Técnicas utilizadas

- **DAX avançado** — medidas calculadas, KPIs, ranking dinâmico, comparativos YoY e MoM
- **Power Query (M)** — transformações, junções entre fontes, limpeza e padronização de dados
- **Modelagem em estrela** — tabelas fato + dimensões (tempo, produto, estabelecimento, seção)
- **Tema personalizado (JSON)** — paleta de cores, tipografia e estilos aplicados globalmente
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

## 👩‍💻 Desenvolvedora

**Raquel Daud** — Analista de Dados | Power BI | SQL | DAX

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raquel-daud/)
