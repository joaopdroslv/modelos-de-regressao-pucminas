# Multicolinearidade

**Pergunta:** as preditoras repetem a informação umas das outras?

**Por que importa:** se duas preditoras andam muito juntas, o modelo não consegue separar o efeito de cada uma. Os coeficientes ficam instáveis e difíceis de interpretar.

## Como medir: VIF

O VIF mede o quanto uma preditora é explicada pelas **outras preditoras** (o alvo não entra).

| VIF | Leitura |
|---|---|
| próximo de 1 | sem multicolinearidade |
| acima de 5 ou 10 | problema |

Exemplo (`Propagandas.csv`): TV = 1,00, Radio = 1,14, Jornal = 1,15. Sem multicolinearidade.

## Não confundir

- Preditora x **alvo** correlacionados: **bom**, é o que permite prever.
- Preditora x **preditora** muito correlacionadas: **ruim**, é a multicolinearidade.

> **Para lembrar:** multicolinearidade é preditora com preditora; VIF perto de 1 é bom.
