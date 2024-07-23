## Desafio Sagemaker Canvas

#### Repositório para Desafio de Sagemaker Canvas da DIO

### Detalhes do Desafio

* **Dataset:** "dataset-1000-com-preco-promocional-e-renovacao-estoque"
* **Alvo:** Coluna "QUATIDADE_ESTOQUE" para previsão
* **Identificação:** Coluna "ID_PRODUTO"
* **Validação de Datas:** Coluna "DATA_EVENTO", considerando feriados brasileiros

## Quick Build
### Métricas Obtidas
![image](https://github.com/user-attachments/assets/e25e9173-28ca-4858-af10-aab7e78565dd)

**Métricas:**

| Métrica | Valor | Interpretação | Observações |
|---|---|---|---|
| AVG. wQL | 0,06 | Mede o erro médio das previsões. Valores próximos a 0 indicam alta precisão. O valor de 0,06 demonstra um bom ajuste do modelo à realidade. | - |
| MAPE | 0,149 | Indica a porcentagem média de erro das previsões em relação aos valores reais. Um valor de 0,149 sugere um erro de 14,9%, acima do ideal (10%), mas dentro do aceitável (abaixo de 30%). | - |
| WAPE | 0,103 | Mede a porcentagem média de erro das previsões em relação aos itens de maior valor. Um valor de 0,103 indica um erro de 10,3% para esses itens, próximo do alvo ideal de 10%. | - |
| RMSE | 5,997 | Representa a média das diferenças entre as previsões e os valores reais. Um valor de 5,997 sugere que a diferença entre a previsão e a realidade pode gerar problemas, pois o aceitável para falta de estoque é de 5. Ou seja, o modelo prevê faltas maiores que o ideal. | O RMSE indica uma possível necessidade de ajuste do modelo para minimizar as previsões de faltas de estoque. |
| MASE | 0,31 | Compara o erro da previsão com um modelo simples. Valores menores que 1 indicam que o modelo supera a média histórica na previsão. O valor 0,31 sugere que o modelo apresenta alguma melhora em relação à média, mas ainda há espaço para aprimoramento. |  O MASE sugere que o modelo pode ser ainda mais refinado para superar a previsão da média histórica. |

**Conclusão:**

O modelo de previsão apresenta desempenho satisfatório em algumas métricas, como AVG. wQL e WAPE, indicando um bom ajuste do modelo à realidade e precisão nas previsões para itens de maior valor. No entanto, o MAPE e o RMSE indicam que o modelo ainda pode ser otimizado para reduzir o erro geral das previsões e melhorar a precisão, especialmente em relação à previsão de faltas de estoque. O MASE indica que o modelo supera a média histórica, mas ainda há espaço para aprimoramento para superar o modelo simples.

## STANDARD BUILD


