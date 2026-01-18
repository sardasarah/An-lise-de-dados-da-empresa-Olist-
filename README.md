# Análise de dados da empresa Olist
Esse projeto foi desenvolvido através da ferramenta Power BI, com o objetivo de analisar dados de e-commerce da empresa Olist Store, uma empresa brasileira, que disponibilizou um dataset público na plataforma Kaggle. Essa análise busca responder perguntas e encontrar variáveis para a tomada de decisão da empresa.

# Detalhes do conjunto de dados
O dataset "Brazilian E-Commerce Public Dataset by Olist" possui várias tabelas, para esse projeto foram utilizadas:
- olist_orders_dataset: Pedidos
- olist_customers_dataset: Clientes
- olist_products_dataset: Produtos
- olist_sellers_dataset: Vendedores
- olist_order_items_dataset: Itens(Seria a venda específica para cada cliente)
- olist_order_payments_dataset: Pagamentos

# Tabelas
1. Pedidos:
   - ID_Pedido
   - ID_Transacao_Cliente
   - Status
   - Data_Compra
   - Data_Aprovacao
   - Data_Entrega_Cliente
   - Data_Entrega_Transportadora
   - Data_Estimada_Entrega
   Medidas:
   - % Entrega no Prazo
   - Dias de Entrega
   - Dias Deslocamento(Transportadora)
   - Dias Processamento
   - Pedido com Atraso
   - Pedidos no Prazo
   - Peso de Frete (%)
2. Produtos
   - ID_Produto
   - Categoria
3. Clientes
   - ID_Unico_Cliente
   - ID_Transacao_Cliente
   - Estado_Cliente
4. Vendedores
   - ID do Vendedor
   - UF do Vendedor
5. Pagamentos
   - ID_Pedido
   - Tipo_Pagamento
   Medida criada:
   - Total Pago
  Coluna criada:
   - Valor_Pagamento
6. Itens
   - ID_Pedido
   - ID_Produto
   - ID do Vendedor
   Colunas criadas:
   - Preço
   - Valor_Frete
   - Valor_Total_Item
   Medidas criadas:
   - Ticket Médio
   - Faturamento Total
7. Filtro_regiao(Permite o agrupamento dos estados por região).
   - Região
   - UF
8. Calendário(Essa tabela foi criada)
   - Mes_Nome
   Colunas criadas:
   - Data
   - Ano
  


# Investigações
1. Qual é a quantia de receita que está passando pela empresa? A empresa está crescendo, estagnando ou decaindo? (Janeiro e dezembro)
2. Quais categorias estão gerando mais receita? Essas categorias possuem um ticket médio alto?
3. Quais formas de pagamento estão sendo mais utilizadas pelos clientes e por que?
4. Quais estados lucram mais pra empresa?
5. Quantos dias o cliente espera pelo produto? O dia da entrega está passando do prazo? Mesmo após o prazo, a empresa está conseguindo entregar mais rápido?
6. Quais estados possuem mais atraso de entrega? Os culpados são a transportadora que demora para enviar ou o vendedor?
7. Os fretes mais caros estão entregando mais rapidamente conforme essa promessa?

# Visão Geral dos Dashboards
Dashboard de análise das vendas:
- KPIs(indicador chave de desempenho) de faturamento total(total de renda que passou pela empresa) e ticket médio(valor médio de cada pedido).
- Gráfico de Área: Evolução mensal do faturamento de 2016 até 2018.
- Gráfico de Rosca: Formas de pagamento mais utilizadas.
- Gráfico de barras empilhadas: Categorias que geram mais receita e Faturamento total por Estado.
- Filtro para os anos 2016, 2017 e 2018.
Dashboard de análise logística:
- KPIs mostrando o total de dias que demora para a entrega, porcentagem de pedidos atrasados, peso do frete no valor do pedido em porcentagem e valor em porcentagem da entrega dentro do prazo.
- Cartões para filtro de mês e região.
- Gráfico de barras indicando os estados que possuem mais atraso
- Matriz indicando a relação entre Estado do Vendedor e Estado do Comprador.
- Gráfico de barras mostrando os responsáveis pelos atrasados (Vendedor ou Transportadora)
- Gráfico de Dispersão relacionando valor do frete e quantidade de dias até a entrega.
# Principais Insights
1. O faturamento mensal da empresa depende de eventos como a Black Friday, uma vez que há um grande pico de receita em novembro. Em contrapartida, janeiro apresenta o menor faturamento registrado, baseando-se no ano de 2017. Na logística, os atrasos são altos em novembro, o que mostra que a empresa não está conseguindo lidar com o volume de pedidos nessa época do ano.
2. Há pouca participação no faturamento total por estados das regiões Nordeste e Norte entre as dez regiões com maior faturamento. Isso mostra que a Olist ainda não conquistou essas regiões em razão da logística da transportadora, já que esta é, a princípio, a culpada pelos atrasos — sendo a região Nordeste a que possui os maiores índices de demora.
3. Cartão de crédito e boleto são as opções mais utilizadas pelos clientes, o que é melhor para a empresa, já que a confirmação do pagamento com essas formas é mais rápida e contribui para diminuir os atrasos.
4. As regiões Norte e Nordeste possuem as maiores quantidades de dias para entrega e, mesmo após a data estimada, ficam atrás de outros estados no cumprimento do prazo de entrega.
5. A logística da Olist é imprevisível para as regiões Norte e Nordeste, pois, ainda que os fretes possam ser mais caros, o pedido pode demorar muitos dias para chegar. Em média, os fretes mais baratos continuam apresentando demora na entrega.
6. A região Sudeste é a que menos demora para receber seus pedidos, principalmente São Paulo, mesmo quando o vendedor é de uma região distante.
7. Entre os culpados pelos atrasos, destaca-se a transportadora; contudo, muitas vezes é o vendedor quem demora para despachar o produto.
8. Produtos da categoria de Beleza são os mais vendidos, porém possuem um dos menores tickets médios, exigindo um volume maior de vendas. Entretanto, a categoria de Relógios possui menos vendas, mas seu ticket médio é alto, sendo interessante para a empresa investir nessa categoria para aumentar o faturamento.
# Conclusão
Os dashboards da Olist oferecem uma visão abrangente da performance de vendas e da logística da empresa. Ao utilizar o Power BI e o DAX, os dashboards fornecem informações valiosas, incluindo:

Relação entre o ticket médio e os produtos.
Evolução da empresa mensalmente e por região.
Formas de pagamento mais usadas pelos clientes. 
Categorias de produtos, que geram mais receita dentro da empresa.
Em quais estados a Olist é mais explorada.
Como a empresa está em relação a demora para entregar o produto, os atrasos e peso do frete no valor do pedido.
Principais culpados pelos atrasos.
Estados com mais atrasos.
A promessa dos fretes.

# Conecte-se comigo
Fique à vontade para se conectar comigo no LinkedIn: [Sarah Costa](www.linkedin.com/in/sarah-costa-a84425290)
Você também pode entrar em contato comigo por e-mail: sarah.costaepereira@gmail.com





