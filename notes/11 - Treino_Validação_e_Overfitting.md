# Treino, validação e overfitting

**Pergunta:** o modelo vai bem em dados que ele **não viu**?

| Termo | Significado |
|---|---|
| **Treino** | dados usados para ajustar o modelo |
| **Validação / teste** | dados separados, usados só para avaliar |
| **Underfitting** | modelo simples demais: erra até no treino |
| **Overfitting** | modelo decora o treino: vai bem nele e mal em dados novos |

## Como perceber

| Treino | Dados novos | Diagnóstico |
|---|---|---|
| ruim | ruim | underfitting |
| bom | ruim | overfitting |
| bom | bom | bom ajuste |

## Cuidado

O R² calculado nos **mesmos dados** em que o modelo foi ajustado não garante o desempenho em dados novos. Para isso, é preciso separar uma parte dos dados antes de ajustar (por exemplo, com `train_test_split`).

> **Para lembrar:** avaliar no treino é corrigir a prova com o gabarito na mão.
