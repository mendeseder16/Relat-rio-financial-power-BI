# Relat-rio-financial-power-BI

O dataset Financials foi excelente para praticar os fundamentos do Power BI, como modelagem, DAX e visualização.
O relatório profissional foi seguido com as  melhores práticas solicitadas em desafios desse tipo, aqui está um roteiro do que foi feito:

1. Preparação dos Dados (Power Query)
Limpeza: Removidas colunas desnecessárias e verificado os tipos de dados (ex: mude "Sales" para Moeda).
Calendário:  Criada uma tabela d_Calendario usando DAX ou M para garantir que suas análises temporais (Year-over-Year, MTD) funcionem perfeitamente.

2. Modelagem 
foi seguido o modelo Star Schema (Esquema Estrela).
Separando suas tabelas em Dimensões (ex: d_Produtos, d_Segmentos, d_Calendario) e a tabela Fato (f_Vendas).

3. Medidas DAX Essenciais
foi criado uma tabela separada apenas para suas medidas. Algumas básicas para este projeto:
Total Sales = SUM(Financials[Sales])
Total Units Sold = SUM(Financials[Units Sold])
Gross Margin = [Total Sales] - [Total Cost]
Profit = SUM(Financials[Profit])

4. Visualização (Dicas de Layout)
Página de Resumo: KPIs no topo (Cartões), Gráfico de área para vendas ao longo do tempo e Gráfico de barras para vendas por segmento.
