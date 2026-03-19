# Previsao de Fechamento Mensal - MDS

Dashboards interativos de previsao de fechamento mensal gerados automaticamente por modelos ML/estatisticos.

## Acesso

**URL:** [marciosiosaki.github.io/previsao_mes](https://marciosiosaki.github.io/previsao_mes)

**Credenciais:**
- Usuario: `ADMIN`
- Senha: `16121980`

## Dashboards Disponiveis

| Dashboard | Descricao |
|-----------|----------|
| **Terapias** | Previsao de fechamento mensal de terapias (Classificacao 140) |
| **Exames** | Previsao de fechamento mensal de exames (Classificacao 10) |

## Estrutura

```
previsao_mes/
  index.html                              # Hub/portal com login
  dashboard_previsao_YYYYMM.html          # Dashboard de terapias
  dashboard_previsao_exames_YYYYMM.html   # Dashboard de exames
  README.md                               # Este arquivo
```

## Como e Gerado

Os dashboards sao gerados automaticamente pelos notebooks:
- `04_previsao_fechamento_terapias.ipynb` - Previsao de terapias
- `Exame/previsao_exames.ipynb` - Previsao de exames

Cada notebook executa um ensemble de modelos (ARIMA, Holt-Winters, Prophet, etc.) e gera um HTML interativo com ECharts.
