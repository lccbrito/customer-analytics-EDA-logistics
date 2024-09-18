# E-Commerce Shipping Data - Logistics

## Contexto e Objetivo

Este projeto tem como objetivo realizar uma Análise Exploratória de Dados (EDA) para fornecer insights sobre o desempenho logístico de uma empresa de e-commerce. O conjunto de dados utilizado contém informações relacionadas à entrega de produtos aos clientes. O foco desta análise é identificar padrões e tendências que possam ajudar a otimizar os processos de entrega e melhorar a satisfação do cliente.

## Conjunto de Dados

O conjunto de dados foi retirado do Kaggle, disponível em [E-Commerce Shipping Data](https://www.kaggle.com/datasets/prachi13/customer-analytics/data). Ele contém os seguintes campos:

* **id:** Identificação única dos clientes.
* **warehouse_block:** Bloco do armazém onde o produto está armazenado.
* **mode_of_shipment:** Modo de envio (navio, avião ou rodoviário).
* **customer_care_calls:** Número de chamadas feitas ao atendimento ao cliente.
* **customer_rating:** Classificação do cliente (1 = pior, 5 = melhor).
* **cost_of_the_product:** Custo do produto em dólares.
* **prior_purchases:** Número de compras anteriores.
* **priority:** Prioridade do produto (baixa, média ou alta).
* **gender:** Gênero do cliente (Masculino ou Feminino).
* **discount_offered:** Desconto oferecido no produto.
* **weight_in_gms:** Peso do produto em gramas.
* **exceeded_deadline:** Informa se o prazo de entrega do produto foi excedido, onde TRUE indica que chegou atrasado, e FALSE indica que chegou no prazo.

## Análises Realizadas

1. **Distribuição de Produtos por Bloco de Armazém (Warehouse block)**
   - Análise da quantidade de produtos armazenados nos diferentes blocos do armazém.

2. **Proporção de Produtos Atrasados e Entregues no Prazo por Bloco**
   - Análise da proporção de produtos entregues com atraso e no prazo, segmentados por bloco de armazém.

3. **Distribuição dos Modos de Envio (Mode of shipment)**
   - Análise de como os produtos são distribuídos entre os diferentes modos de envio.

4. **Análise Descritiva dos Atrasos por Modo de Envio**
   - Análise da taxa de atraso em relação ao modo de envio utilizado.

5. **Impacto da Prioridade do Produto na Entrega**
   - Análise de como a prioridade atribuída ao produto influencia a entrega dentro do prazo.

6. **Distribuição dos Custos dos Produtos**
   - Análise da distribuição dos custos dos produtos e identificação das faixas de custo predominantes.

7. **Custo Médio por Variáveis**
   - Análise do custo médio dos produtos em relação a variáveis como atraso na entrega e prioridade.

8. **Distribuição das Avaliações dos Clientes**
   - Análise da distribuição das avaliações dos clientes e identificação de padrões nas classificações.

9. **Relação das Avaliações com os Atrasos da Entrega**
   - Análise de como as avaliações dos clientes se relacionam com os atrasos nas entregas.

10. **Distribuição do Peso dos Produtos por Prazo de Entrega**
    - Análise da distribuição do peso dos produtos e como isso afeta o prazo de entrega.

## Principais Insights

- A taxa de produtos com atraso é elevada em todos os blocos, com variação entre 58% e 60%. Isso indica que a maioria dos produtos enfrentam atraso na entrega independentemente do bloco de armazém, o que sugere um problema na logística operacional. Pode ser uma combinação de fatores, como processos lentos, excesso de pedidos, ou até mesmo problemas no transporte.

- O transporte marítimo (Ship) é responsável por ~68% dos envios, o que é significativamente maior que os outros modos (Flight e Road). A utilização predominante do transporte marítimo pode estar ligada a custos operacionais, visto que o envio por navio é geralmente mais barato para grandes volumes.Isso indica que a empresa pode estar priorizando a eficiência de custos em vez da velocidade de entrega. No entanto, caso os atrasos estejam prejudicando a satisfação do cliente, pode ser interessante reavaliar essa estratégia.

- As proporções de atraso são bastante semelhantes entre os diferentes modos de envio, com uma variação de aproximadamente 2%. A diferença não é significativa o suficiente para considerar que um modo de envio tem uma tendência maior de atrasos do que os outros.

- A logística da empresa, de modo geral, enfrenta um problema com entregas pontuais, independentemente da prioridade do produto. Uma revisão dos processos logísticos e priorização pode ser necessária, principalmente para produtos de alta prioridade, visando melhorar a eficiência e atender melhor às expectativas dos clientes.

- A maioria dos produtos está nas faixas de peso mais baixas ou intermediária (1000-2000 g e 4001-5000 g), representando quase 74% do total. Isso sugere que a empresa lida predominantemente com produtos mais leves ou de peso intermediário.

- A distribuição das avaliações dos clientes mostra que a maioria dos produtos recebe avaliações médias.

## Visualizações

- Gráficos de barras, histogramas e diagramas de dispersão foram utilizados para visualizar as distribuições e relações entre as variáveis.

## Tecnologias Utilizadas

- **Python 3.12.4**
- **Pandas**: Para manipulação e análise exporatória dos dados.
- **Matplotlib**: Para visualização de dados.
- **Seaborn**: Para gráficos estatísticos.
- **Jupyter Notebook**: Para desenvolvimento e documentação.