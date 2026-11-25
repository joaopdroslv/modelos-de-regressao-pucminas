# Outliers

**Pergunta:** o que é incomum, o **valor** ou o **erro**?

| | Valor incomum | Erro incomum |
|---|---|---|
| **Como achar** | IQR (boxplot) ou Z-score | resíduo padronizado |
| **Limite** | abaixo de Q1 - 1,5·IQR ou acima de Q3 + 1,5·IQR; ou \|Z\| > 3 | abaixo de -3 ou acima de 3 |
| **Precisa de modelo?** | não | sim |
| **Exemplo (`Propagandas.csv`)** | linhas 16 e 101 (Jornal = 114,0 e 100,9) | linhas 130 (-5,34) e 5 (-3,21) |

São observações **diferentes**: ter um valor incomum não quer dizer que o modelo erra nela, e vice-versa.

## O que fazer

1. **Erro de digitação ou impossível** (ex.: idade 200): remover ou corrigir.
2. **Valor real e plausível:** manter, e dizer por quê.
3. **Valor real, mas domina o modelo:** avaliar tratamento (limitar aos extremos ou usar log).

> **Para lembrar:** IQR olha o dado; resíduo olha o modelo. Não remova só porque é outlier.
