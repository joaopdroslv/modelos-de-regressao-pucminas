# Homocedasticidade

**Pergunta:** o modelo erra com a mesma dispersão em toda a faixa de valores?

| Termo | Significado | No gráfico de resíduos x ajustados |
|---|---|---|
| **Homocedasticidade** | variância dos resíduos constante (bom) | faixa de largura parecida |
| **Heterocedasticidade** | variância dos resíduos muda (ruim) | funil ou cone |

**Por que importa:** com heterocedasticidade, os coeficientes ainda podem ser estimados, mas os p-valores e testes deixam de ser confiáveis.

## Como testar: Breusch-Pagan

H0: homocedasticidade (a suposição que queremos manter).

| p-valor | Conclusão |
|---|---|
| > 0,05 | não se rejeita a homocedasticidade (**bom**) |
| < 0,05 | há evidência de heterocedasticidade (**ruim**) |

Exemplo (`Propagandas.csv`): p = 0,1623 > 0,05, então não se rejeita a homocedasticidade.

> **Para lembrar:** homo = igual. Funil é ruim, e aqui p **alto** é bom (o contrário do teste de correlação).
