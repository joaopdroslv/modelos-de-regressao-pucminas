# Coeficientes da regressão

```
Vendas = 2,9389 + 0,0458 * TV + 0,1885 * Radio - 0,0010 * Jornal
```

| Termo | Leitura |
|---|---|
| **Intercepto (const)** | valor previsto quando todas as preditoras são zero |
| **Coeficiente** | quanto o alvo muda, em média, quando a preditora sobe **1 unidade**, com as **outras fixas** |

Exemplo: +1 em TV → +0,0458 em Vendas, com Radio e Jornal fixos.

## Cuidados

- **O maior coeficiente não é o mais importante.** Radio (0,1885) tem coeficiente maior que TV (0,0458), mas as faixas são diferentes: TV vai até 296,4 e Radio até 49,6.
- **Coeficiente não é teste:** antes de interpretar, veja se ele é significativo (teste t). Jornal (-0,0010) não é, então não dá para dizer que ele reduz as vendas.
- **O coeficiente muda** conforme as outras preditoras do modelo.
- **Associação não é causa:** o modelo mostra relação, não prova o motivo.

> **Para lembrar:** "+1 nesta, com as outras paradas, muda tanto no alvo".
