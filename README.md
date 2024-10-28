Projeto Power BI - Star Schema
Descrição do Projeto
Este projeto tem como objetivo criar um modelo de dados baseado em star schema utilizando a tabela Financial Sample. O modelo inclui tabelas de fato e dimensão para otimizar análises de vendas e desempenho financeiro.

Etapas do Processo
Criação das Tabelas de Backup:

Financials_origem: Tabela original mantida oculta como backup.

Criação das Tabelas Dimensão:

D_Produtos: Inclui colunas como ID_produto, Produto, Média de Unidades Vendidas, etc.

D_Produtos_Detalhes: Inclui colunas como ID_produtos, Discount Band, Sale Price, etc.

D_Descontos: Inclui colunas como ID_produto, Discount, Discount Band.

D_Detalhes: Inclui colunas adicionais que não foram contempladas nas outras tabelas.

D_Calendário: Criada utilizando a função DAX CALENDAR().

Criação da Tabela Fato:

F_Vendas: Inclui colunas como SK_ID, ID_Produto, Produto, Units Sold, etc.

Transformações de Dados:

Agrupamentos e cálculos condicionais foram realizados para calcular métricas como Média de Unidades Vendidas.

Criação de colunas calculadas para índices específicos dos produtos.

Relacionamentos:

Definição de relações entre as tabelas fato e dimensão para garantir a integridade e funcionalidade do modelo.

Funções DAX Utilizadas
CALENDAR(): Criou a tabela de calendário para uso nas análises temporais.

SUM(): Utilizada para somar valores em colunas de interesse.

CALCULATE(): Aplicada para modificar o contexto de cálculo e realizar agregações condicionais.

Conclusão
