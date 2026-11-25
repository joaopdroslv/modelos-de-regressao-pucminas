# Covariância, correlação e p-valor

São **três perguntas diferentes**, uma em cima da outra.

| | Pergunta | Faixa | Para que serve |
|---|---|---|---|
| **Covariância** | Andam juntas ou em sentidos opostos? | qualquer número | só o **sinal** |
| **Correlação (r)** | Quão **forte** é a relação? | -1 a 1 | sinal **e** força |
| **p-valor** | Dá para confiar que **existe**? | 0 a 1 | < 0,05: significativa |

## Covariância x correlação

A correlação é a covariância dividida pelos desvios padrão das duas variáveis, o que tira a unidade. Exemplo com os dados de `Propagandas.csv`:

```
TV x Vendas: 350,39 / (85,85 × 5,22) ≈ 0,78
```

- **350,39** é muito ou pouco? Não dá para saber, depende da unidade. Se `TV` fosse medida em outra unidade, ele mudaria.
- **0,78** é forte, em qualquer unidade.

> **Dica:** covariância é o preço sem dizer a moeda; correlação é o preço já convertido para a mesma moeda.

## r x p-valor

**r** é o **tamanho** da relação e **p** é a **evidência** de que ela existe. O p depende do r **e da quantidade de dados**:

| Par | n | r | p-valor |
|---|---|---|---|
| Jornal x Vendas | 200 | 0,23 | 0,0011 |
| condition x current price | 1000 | 0,11 | 0,0005 |

A `condition` tem r **menor** (mais fraca), mas p **menor** (mais evidência), porque tem cinco vezes mais dados.

## Roteiro para ler qualquer par

1. **p < 0,05?** Se não, pare: não há evidência de relação.
2. Se sim, olhe o **|r|** (em módulo, ou seja, sem o sinal): perto de 0 é fraca, perto de 1 é forte.
3. O **sinal** de r diz o sentido: + sobem juntas, - uma sobe e a outra desce.
4. **Covariância:** use só para o sinal.

> **Para lembrar:** sinal → covariância; tamanho → r; confiança → p.
