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

# Dados de cada tabela
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
1. 
# Conclusão
# Conecte-se comigo
Fique à vontade para se conectar comigo no LinkedIn: 
Você também pode entrar em contato comigo por e-mail: sarah.costaepereira@gmail.com





