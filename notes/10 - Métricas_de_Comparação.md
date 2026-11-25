# Métricas de comparação de modelos

| Métrica | O que mede | Quero... |
|---|---|---|
| **R²** | proporção da variação do alvo explicada pelo modelo | **maior** |
| **R² ajustado** | R² que penaliza preditoras desnecessárias | **maior** |
| **MAE** | média do erro absoluto, na unidade do alvo | **menor** |
| **MSE** | média do erro ao quadrado (pune mais os erros grandes) | **menor** |
| **AIC** | ajuste com penalidade pelo número de variáveis | **menor** |
| **BIC** | igual ao AIC, mas com penalidade mais forte | **menor** |

## Cuidados

- **R² nunca cai** quando se adiciona uma preditora, mesmo inútil. Para comparar modelos com quantidades diferentes de variáveis, use o **R² ajustado**, o AIC ou o BIC.
- **AIC e BIC** só servem para comparar modelos com o **mesmo alvo e os mesmos dados**; o valor sozinho não diz nada.
- **MAE** é o mais fácil de explicar: "em média, o modelo erra X".
- Métrica boa não basta: o modelo também precisa atender às suposições (resíduos, multicolinearidade).

Exemplo (`Propagandas.csv`): R² = 0,8972 e R² ajustado = 0,8956. Quase iguais, então a penalidade pelas três preditoras é mínima.

> **Para lembrar:** R² para cima; erro, AIC e BIC para baixo.
