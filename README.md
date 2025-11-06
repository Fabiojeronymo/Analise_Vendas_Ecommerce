# Análise de Dados de Vendas (E-commerce)

Este projeto realiza uma análise exploratória (EDA) em um conjunto de dados de 200.000 registros de vendas de um e-commerce, cobrindo um período de 2 anos. O objetivo é extrair insights acionáveis sobre desempenho de vendas, lucratividade, comportamento do cliente, padrões regionais e sazonalidade.

# 💾 O Conjunto de Dados

Fonte: archive.zip

Tamanho: 200.000 linhas e 14 colunas originais.

Período: Contém 730 dias (2 anos) de dados de transações.

Colunas Principais: Order_Date, Customer_Name, Region, Category, Product_Name, Quantity, Revenue, Profit.

# 🛠️ Etapas de Preparação e Limpeza

Antes da análise, os seguintes passos de limpeza e preparação foram executados:

- Carregamento de Dados
- Verificação Inicial
- Remoção de Colunas
- Renomeação de Colunas
- Espaços extras nos nomes das colunas (ex: Revenue) foram removidos.
- Conversão de Tipos

# 📚 Bibliotecas Utilizadas

Pandas: Para manipulação e análise dos dados.

Matplotlib: Para a criação de gráficos base.

Seaborn: Para visualização estatística de dados.

Plotly: Para gráficos interativos (especificamente o gráfico de cascata).

Numpy: Para cálculos (utilizado no apply de dias da semana).

# 💡 Principais Descobertas e Análises
A análise foi dividida em várias seções para responder perguntas de negócio específicas:

💰 1. Visão Financeira Geral
Ticket Médio: O valor médio por transação é de R$ 712,04.

Margem Média: A margem de lucro média geral em todos os produtos é de 25,77%.

Visualização de Lucro: Um gráfico de cascata (waterfall chart) foi usado para mostrar visualmente a decomposição do Valor Total (Receita) em Custos e Lucro Líquido.

# 📦 2. Análise de Produtos
Volume vs. Faturamento: A análise revelou uma visão crucial: os produtos mais vendidos em volume (quantidade) não são os mesmos que geram maior faturamento (R$).

Mais Vendido (Volume): Instant Pot (18.200 unidades).

Maior Faturamento (R$): Tempur-Pedic Mattress (R$ 9,06M).

Produto Mais Lucrativo: O Tempur-Pedic Mattress também foi o produto que gerou o maior lucro total (R$ 2,13M).

Margem por Categoria: O gráfico de barras de margem por categoria ajuda a identificar quais categorias têm melhor desempenho proporcional, com a média destacada por uma linha.

# 👥 3. Análise de Clientes
Cliente Mais Frequente: Michael Smith é o nome que aparece com mais frequência nas compras (36 vezes).

Descoberta Chave: O nome do cliente não é um identificador único. A análise identificou vários clientes com o mesmo nome.

Solução: Para uma análise de cliente mais precisa, foi adotado o agrupamento por (Nome do Cliente, Regiao) para diferenciar indivíduos.

Clientes com Maior Gasto:

Hannah Cooke (Springfield, Centre) - R$ 9.014,25

Kenneth Torres (Dover, East) - R$ 8.674,17

Dalton Oneal (Salt Lake City, West) - R$ 8.600,69

🌍 4. Análise Geográfica (Regiões e Estados)
Lucro por Região: O gráfico de barras de "Lucro por Região" identifica qual região é a mais lucrativa para a empresa.

Cidades Mais Lucrativas: Um Top 5 das cidades com maior geração de lucro foi criado.

Lucro Médio por Estado: A análise mostrou quais estados possuem o maior lucro médio por venda (Top 3: Ohio, Illinois, Kansas), o que é diferente do lucro total.

📅 5. Análise de Sazonalidade
Lucro por Mês: O gráfico de linha "Sazonalidade nas compras por mês" mostra os picos e vales de lucratividade ao longo do ano.

Lucro por Categoria ao Longo do Ano: O gráfico de linha múltipla mostrou que diferentes categorias têm picos em meses distintos (ex: eletrônicos podem vender mais no final do ano, enquanto vestuário em outra época).

Semana vs. Fim de Semana: A análise comprovou que Dias de Semana geram um lucro significativamente maior (R$ 21,8M) em comparação com Finais de Semana (R$ 9,6M).

Desempenho Anual: O lucro foi ligeiramente maior em 2024 (R$ 15,86M) do que em 2023 (R$ 15,67M).
