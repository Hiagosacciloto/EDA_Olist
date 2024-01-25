# Análise Exploratória dos Dados do Olist
<img src="https://github.com/Hiagosacciloto/Portfolio/assets/128402589/55e606eb-5f9e-44b3-afd3-d2a8c0579590" width="450">

## 🎯 Objetivo do projeto
Este projeto tem como propósito realizar uma Análise Exploratória de Dados do Olist, visando aprofundar a compreensão sobre o cenário do comércio eletrônico brasileiro. O obejtivo é decifrar padrões, identificar tendências e, consequentemente, revelar oportunidades estratégicas que possam ser exploradas para otimizar a operação do Olist.

## 🔎 Fonte dos dados
O conjunto de dados do Olist utilizado, pode ser acessado no [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).
## ⚙ Tecnologias Utilizadas
- Pandas
- Numpy
- Matplotlib
- Seaborn
## Principais Análises e Insights:
Os conjuntos de dados do Olist abrem muitas possibilidades de estudos pela sua complexidade e disponibilidade de informações. Resumiremos aqui os principais caracteristicas dos dados analisados e os pontos identificados para melhoria e estudos, afim de otimizar a operação da Olist. Seguiremos por tópicos e sequência, conforme dividimos o sumário:

**1. Detalhes dos Pedidos realizados no E-Commerce:**
- Entre os 100 mil pedidos registrados, 97% se trata de pedidos entregues e nem 1% para pedidos cancelados.
- Tendência de alta no volume de pedidos, que teve inicio em 2017 e o maior pico de vendas na série histórica em novembro.
- Em 2018 os pedidos permaneceram em um nivel elevado em relação ao ano anterior, indicando maior propensão dos consumidores em compras online.
- Aos fins de semana existe redução nos pedidos realizados, e o periodo do dia com maior quantidade de pedidos é a tarde.
- Um aumento de 143% nos pedidos, ao analisar o período de Janeiro a Agosto nos anos de 2017 e 2018(devido os pedidos em 2018 irem até agosto). Os pedidos mais que dobraram de um ano para o outro.
- Comparando apenas os pedidos realizados em Janeiro, em 2018 foi aproximadamente 8x maior que os pedidos feitos em 2017.
- Tendência de pedidos seguem o mesmo padrão tanto em 2017 como em 2018.
- A região com maior participação sobre os pedidos é o Sudeste, representando 68% das vendas e aproximadamente 2,19x o volume de vendas do restante do país. Liderou a alta nos pedidos ocorrida em 2017.
- Além da predominância dos estados do Sul e Sudeste, vemos alguns estados com bem poucos pedidos. Isso nos faz pensar sobre a viabilidades econômica de entrega para essa regiões, visto que são estados mais afastados e com bem pouca representatividade.

**2. Preços e métricas financeiras:**
- **Observação**: A análise daqui para frente segue sendo entre o período de Jan/2017 a Aug/2018 e apenas com pedidos Entregues.
- Crescimento no valor total em vendas de aproximadamente 3x de Janeiro de 2017 para 2018.
- Crescimento notavél no faturamento, partindo de menos de 200 mil, alcançou cerca de 1 milhão em novembro, no pico de vendas.
- Pedidos com valores aproximadamente maiores que 300 são considerados outliers. A média geral e de 137 e a mediana 86 e desvrio padrão de 209 indicam uma grande dispersão nos valores dos pedidos. Por se tratar de um E-commerce, os outliers podem indicar que alguns clientes estão propensos a gastar mais com determinados produtos, devido ao ticket alto de compra. Este cenário abre outras possibilidades de estudo para realizar campanhas de marketing e ofertas.

**3. Fretes e regiões:**
- Regiões norte e nordeste pagam em média bem mais pelo frete, aproximadamente o dobro em relação a regiões do sul, sudeste e centro-oeste.
- Custo Médio de frete do País é pouco representativo, pois regiões como São Paulo que possuem o custo médio abaixo da média do país, acabam reduzindo a média geral.
- A questão logística pode desempenhar um papel crucial, especialmente se melhorias no custo e tempo de entrega para regiões mais distantes forem implementadas. Isso poderia potencialmente resultar em um aumento significativo no número de pedidos nessas áreas.
- Menores custos de frete para estados do sul, sudeste e centro-oeste. Tempo médio de entrega também são menores para essas regiões.
- Métricas do Estado de São Paulo tem grande influência sobre as métricas geral do país.

**4. Categoria de Produtos:**

- Existe 74 categorias únicas de produtos entre os pedidos entregues.
- As categorias beleza_saude, cama_mesa_banho e esporte_lazer, estão entre as categorias com maior valor total de vendas, mas não estão entre as categorias com maior ticket médio.
- Destaque para a categoria relogios_presentes, que é uma das mais vendidas em quantidade e valor nominal, além de ser uma das 10 categorias com maior ticket médio.
- Existe duas categorias que estão entre as menos vendidas mas que tambem estão presentes nas categorias com maior ticket médio. São elas: portateis_casa_forno_e_cafe, portateis_cozinha_e_preparadores_de_alimentos, que podem ser categorias melhores exploradas e entendidas para fins de marketing, visto que podem gerar um impacto relevante na receita caso se torne uma das categorias mais vendidas.

**5. Meios de Pagamentos**
- Há uma grande predominância do cartão de crédito e do boleto como forma de pagamento, cerca de 93% dos pagamentos são realizados através deles.
- Destaque para a predominância de pagamentos em uma unica vez, que representa aproximadamente metade dos pagamentos.
- A quantidade de pagamentos diminuem conforme a quantidade de parcelas aumentam. Caso a parte é o pagamento em x10, que é uma das 5 preferências de parcelamento.

**6. Vendedores:**
- Entre os 2945 vendedores, 95,4% estão localizados na região Sul e Sudeste.
- A grande diferença de distribuição de vendedores entre as regiões pode estar relacionado a limitação do Serviço de Coleta do Olist, ou outras variaveis que podem limitar a viabilidade do negócio por parte do vendedor. Aqui também temos uma situação a ser estudada, pois dar as condições necessárias para que os vendedores e clientes tenham uma boa experiência, implica em maior quantidade de clientes fiéis e novos clientes, resultando maior faturamento.
- De modo geral, os melhores vendedores são considerados outliers, e a maioria dos vendedores não tem um volume grande em vendas, sendo que 75% deles tiveram valor total em vendas até 3514. 
- Esta área demanda análises mais aprofundadas, pois representa uma vulnerabilidade no negócio. A maioria dos vendedores não possui uma fonte de receita tão robusta, e, individualmente, não há elementos que os incentivem a permanecer como vendedores, o que poderia levá-los a buscar outras plataformas de mercado para realizar suas vendas.
- Em relação ao desempenho dos vendedores surgem alguns questionamentos. No caso dos maiores vendedores, é essencial compreender os tipos de produtos que comercializam, suas opiniões e feedbacks em relação ao sistema da Olist, bem como o tempo dedicado à plataforma. Esse processo se estende igualmente aos vendedores com menor movimentação, visando oferecer suporte e esclarecimento em eventuais dúvidas que possam surgir durante sua jornada na plataforma.

**7. Clientes Fiéis**
- Entre os clientes que realizaram a segunda compra, temos uma média de 75 dias entre a primeira e segunda compra, e 50% da distribuição está até 22 dias.
- Existe um numero alto de segundos pedidos de compra realizados no mesmo dia, levanta alguns questionamentos sobre os tipos de produtos e sobre o operacional do négocio. Essa concentração pode ser explorada, visto que aproximadamente 35% das segundas compras foram realizadas no mesmo dia, demonstrando as preferências dos clientes.
- Entre esses clientes, 46,5% deles não realizaram a segunda compra em menos de 30 dias.
- Cerca de 85% dos clientes fiéis estão no Sul e Sudeste.
- A categoria relógios_presentes é muito bem aceita por esses clientes e possui um ticket médio atraente.
- Para aprimorar métricas cruciais, como Churn, CAC (Custo de Aquisição de Cliente) e LTV (Life Time Value), estratégias como Cross-selling, Up-selling, formação de pacotes de produtos,implementação de programas de fidelidade e etc, são oportunidades promissoras que demandam uma análise mais aprofundadas, afim de direcionar ofertas certas para clientes certos.
- Ticket médio de alguns estados das regiões Norte e Nordeste está bem acima da média geral, como é o caso de Alagoas.
- Explorar os outliers para os clientes fiéis pode ser interessante, pensando em maximizar métricas importantes, como o próprio Ticket médio.
- Valor Médio do frete por Estado segue o mesmo padrão dos pedidos em geral.
- Majoritariamente os clientes fíeis são da região Sul e Sudeste.
- Os pedidos são em maior parte da Região Sul e Sudeste, além do valor nominal.

## Algumas Perguntas respondidas no estudo:
- Qual é o comportamento dos pedidos ao longo do tempo?
<img src="https://github.com/Hiagosacciloto/EDA_Olist/assets/128402589/f26dae21-0085-4b56-a6ad-45ddcaaa5c83" width="600">

- Como a quantidade de pedidos evoluem ao longo do tempo por região do Brasil? E como o Total de vendas é distribuido entre as regiões?
<img src="https://github.com/Hiagosacciloto/EDA_Olist/assets/128402589/25f31ecd-fc8e-4d51-b603-7756f3973870" width="600">

- Quais os melhores estados para comprar no Brasil? Uma análise sobre vendas, frete e prazo de entrega.
<img src="https://github.com/Hiagosacciloto/EDA_Olist/assets/128402589/f040953a-8358-4ab2-af38-4df7de1480b7" width="600">

- Quais as categorias de produtos com maiores movimentações?
<img src="https://github.com/Hiagosacciloto/EDA_Olist/assets/128402589/a20ff84c-19a6-4afd-942f-74a91aca1c14" width="600">

- Quanto aos clientes que realizaram segunda compra, como é a distribuição desses cliente para realizar a próxima compra?
<img src="https://github.com/Hiagosacciloto/EDA_Olist/assets/128402589/dde44e1f-a2ab-46de-8c49-09f683a7f1b5" width="600">

**Existe muitas outras perguntas e insights dentro do estudo, então para o melhor entendimento dos dados, recomendo a leitura do projeto.**


## Meus Projetos e Artigos associado ao Estudo
_______________
## 📬 CONTATO
Estou sempre receptivo a sugestões e oportunidades de melhoria! Se tiver dúvidas, comentários ou desejar entrar em contato, sinta-se à vontade para fazê-lo pelos seguintes canais:

Links para me acharem:

[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hiagosacciloto/)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@hiago.sacciloto)
[![Codewars](https://img.shields.io/badge/Codewars-B1361E?style=for-the-badge&logo=Codewars&logoColor=white)](https://www.codewars.com/users/Hiagosacciloto)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)](https://www.kaggle.com/hiagosacciloto)
