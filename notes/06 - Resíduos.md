# Resíduos

**Resíduo é o erro do modelo em cada observação:**

```
resíduo = valor real - valor previsto
```

| Sinal | Significado |
|---|---|
| positivo | o real ficou **acima** do previsto |
| negativo | o real ficou **abaixo** do previsto |

Exemplo (`Propagandas.csv`, linha 130): 1,6 - 10,43 = **-8,83**. O modelo previu bem mais do que vendeu.

## O que verificar

| Suposição | Como ver | Bom sinal |
|---|---|---|
| Linearidade | resíduos x ajustados | nuvem sem forma (um "U" indica curvatura) |
| Homocedasticidade | resíduos x ajustados e Breusch-Pagan | sem funil; p > 0,05 |
| Normalidade | histograma, Q-Q plot e Shapiro-Wilk | pontos sobre a reta; p > 0,05 |
| Outliers | resíduo padronizado | entre -3 e +3 |

**Resíduo padronizado:** o erro medido em desvios padrão, para saber se ele é grande em relação aos outros. A linha 130 tem -5,34, fora do limite.

## Cuidado

A normalidade exigida é a dos **resíduos**, não a das variáveis de entrada.

> **Para lembrar:** resíduo bom é o que parece ruído: sem forma, sem funil e em torno de zero.
