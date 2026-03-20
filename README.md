# 📊 Power BI — Dashboards Financeiros

Dashboards interativos desenvolvidos no Power BI para análise financeira e operacional de sub-adquirentes.

## 📈 Dashboards incluídos

- **DRE Interativo** — receitas, despesas e resultado com filtros por período e filial
- **Análise de Transações** — volume por bandeira, canal e produto (crédito/débito/Pix)
- **Monitoramento de Chargeback** — taxa, distribuição e tendência
- **Painel de Antecipação** — volume antecipado, custo e spread
- **Relatório de Estabelecimentos** — ranking por TPV e receita

## 🛠️ Técnicas utilizadas

- **DAX avançado** — medidas calculadas, KPIs, % de participação, YoY
- **Power Query (M)** — transformações, joins entre fontes, limpeza de dados
- **Modelagem em estrela** — fato + dimensões (tempo, produto, estabelecimento)
- **RLS (Row Level Security)** — acesso segmentado por filial/parceiro
- **Visuais customizados** — Deneb/Vega para gráficos não nativos

## 💡 Conceitos de DAX aplicados

```dax
-- Take Rate
Take Rate = DIVIDE([Receita MDR], [TPV Total], 0)

-- Taxa de Chargeback
CB Rate = DIVIDE([Valor Chargebacks], [TPV Total], 0)

-- Crescimento MoM
Crescimento MoM =
VAR MesAtual = [TPV Total]
VAR MesAnterior = CALCULATE([TPV Total], DATEADD(Calendario[Data], -1, MONTH))
RETURN DIVIDE(MesAtual - MesAnterior, MesAnterior, 0)
```

---
Desenvolvido por **Raquel Daud** — [LinkedIn](https://www.linkedin.com/in/raquel-daud-72a3991a2/)
