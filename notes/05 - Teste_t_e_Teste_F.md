# Teste t e teste F

| | Pergunta | H0 | p < 0,05 indica |
|---|---|---|---|
| **Teste F** | O modelo **como um todo** serve? | todos os coeficientes das preditoras são zero | pelo menos uma preditora ajuda |
| **Teste t** | **Esta preditora** ajuda, com as outras já no modelo? | o coeficiente dela é zero | a preditora é significativa |

O F diz que **alguma** ajuda; o t diz **qual**.

## Exemplo (`Propagandas.csv`)

**Teste F:** F = 570,27; p < 0,0001. O modelo é significativo.

**Teste t:**

| Preditora | t | p-valor | Significativa? |
|---|---|---|---|
| TV | 32,81 | < 0,0001 | sim |
| Radio | 21,89 | < 0,0001 | sim |
| Jornal | -0,18 | 0,8599 | não |

## Cuidados

- Quanto maior o **|t|**, maior a evidência de que o coeficiente não é zero.
- Não significativa **sozinha** é diferente de não significativa **no modelo**: Jornal tem correlação com Vendas (p = 0,0011), mas não acrescenta nada além de TV e Radio.

> **Para lembrar:** F = modelo inteiro; t = uma preditora por vez.
