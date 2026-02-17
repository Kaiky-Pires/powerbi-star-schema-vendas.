# Modelagem de Dados: Criação de Star Schema para Cenários de Vendas

# 1. Objetivo do Projeto
O objetivo deste projeto é a estruturação de um modelo de dados otimizado utilizando o conceito de Star Schema (Esquema Estrela). Esta modelagem é essencial para garantir a performance de relatórios e a integridade das relações entre diferentes fontes de dados em um ambiente de Business Intelligence.

# 2. Estrutura do Modelo de Dados
O modelo foi planejado seguindo a lógica de separação entre fatos e dimensões:
Tabela Fato (F_Vendas): Contém os dados quantitativos e históricos da operação, como valores monetários, quantidades vendidas e chaves estrangeiras para conexão com as dimensões.

Tabelas Dimensão (D_Produtos, D_Clientes, D_Calendario, D_Localizacao): Tabelas que contêm as características descritivas.
A dimensão Calendário é fundamental para permitir análises temporais (Year-over-Year, acumulados mensais).
A dimensão Produtos permite o agrupamento por categorias e marcas.

# 3. Conceitos de Modelagem Aplicados
Relacionamentos: Planejamento de cardinalidade 1:N (um para muitos), garantindo que os filtros aplicados nas dimensões propaguem corretamente para a tabela fato.

Otimização: Redução de redundância de dados através da normalização das dimensões, melhorando a velocidade de processamento das medidas em DAX.

# 4. Justificativa de Entrega
Devido à ausência de ambiente Windows para execução do Power BI Desktop, este projeto documenta a arquitetura lógica do Star Schema. A entrega foca no conhecimento teórico de modelagem multidimensional, demonstrando a capacidade de estruturar bancos de dados complexos para análise profissional.
