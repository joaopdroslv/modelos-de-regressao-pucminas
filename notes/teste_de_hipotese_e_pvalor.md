# Teste de hipótese e p-valor

**Ideia:** começa supondo que H0 é verdadeira e pergunta se os dados seriam estranhos nesse caso.

- **H0:** a hipótese inicial.
- **p-valor:** a chance de ver um resultado igual ou mais extremo que o observado, **se H0 for verdadeira**.
- **p < 0,05:** resultado raro demais sob H0, então **rejeita-se H0**.
- **p > 0,05:** **não se rejeita H0** (isso não prova que ela é verdadeira).

## Quero p alto ou baixo?

Depende do que é a H0:

| Teste | H0 | Quero p... |
|---|---|---|
| Correlação | correlação = 0 | **baixo** |
| Teste t | coeficiente = 0 | **baixo** |
| Teste F | todos os coeficientes das preditoras são zero | **baixo** |
| Shapiro-Wilk | os dados são normais | **alto** |
| Breusch-Pagan | variância dos resíduos constante | **alto** |

## Cuidados

- p baixo **não** quer dizer efeito forte, só que há evidência de que ele existe.
- Com muitos dados, até efeito pequeno fica significativo.
- p não é a probabilidade de H0 ser verdadeira.

> **Para lembrar:** leia a H0 primeiro. Se H0 é o que você quer manter, quer p alto; se quer derrubá-la, quer p baixo.
