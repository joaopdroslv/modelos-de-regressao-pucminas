### Exercício 1

A partir da base de dados Propagandas.csv, faça **um modelo de regressão múltipla** para predizer as vendas.

O notebook precisa conter:
1. Análise descritiva
2. Calculo de correlação e covariância
3. Faça o modelo de regressão
4. Realize a análise de resíduos
5. Análise de multicolinearidade
6. Análise do Modelo

### Exercício 2

Faça **3 modelos de regressão linear múltipla** para predizer da melhor forma possível o preço dos automóveis.

1º Modelo com **todas variáveis**
2º Modelo com as **3 variáveis mais correlacionadas**
3º Modelo com as **5 variáveis mais correlacionadas**

`ATENÇÃO:` Nas análises de dados e dos modelos devem contemplar:
1. Análise descritiva
2. Calculo de correlação e covariância
3. Faça o modelo de regressão
4. Realize a análise de resíduos
5. Análise de multicolinearidade
6. Análise de outlier
7. Comparação de modelos

| Variável | Descrição |
|---|---|
| `v.id` | Identificador único do veículo (ID). Geralmente não entra em modelos estatísticos. |
| `on road old` | Preço histórico de lançamento ou preço anterior "na estrada". |
| `on road now` | Preço atual do veículo zero quilômetro nas concessionárias. |
| `years` | Idade do veículo ou tempo de uso em anos. |
| `km` | Quilometragem total percorrida pelo veículo. |
| `rating` | Nota ou avaliação do veículo (provavelmente em uma escala de 1 a 5 ou 1 a 10). |
| `condition` | Nota para o estado de conservação física do veículo. |
| `economy` | Consumo de combustível (ex.: km/l). |
| `top speed` | Velocidade máxima que o veículo atinge. |
| `hp` | Potência do motor em Cavalos-Vapor (Horsepower). |
| `torque` | Força de torque do motor (geralmente medida em Nm ou kgfm). |
| `current price` | Variável Alvo (Target). O valor de mercado atual para revenda do item. |
