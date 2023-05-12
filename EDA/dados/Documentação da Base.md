# Dataset Telco
## Contexto
Esses dados de exemplo rastreiam a perda de clientes de uma empresa fictícia de telecomunicações com base em uma variedade de fatores possíveis. A coluna "churn" indica se o cliente saiu ou não nos últimos meses. Outras colunas incluem gênero, dependentes, cobranças mensais e muitas outras com informações sobre os tipos de serviços que cada cliente tem. Fonte: IBM.



## Conteúdo

O módulo de dados __churn__ de clientes da Telco é composto por 5 arquivos enviados:

| Arquivo | Descrição |
| --- | --- |
| Telco_customer_churn_demographics.xlsx | Dados demográficos do cliente |
| Telco_customer_churn_location.xlsx | Dados de localização do cliente |
| Telco_customer_churn_population.xlsx | Dados de população do cliente |
| Telco_customer_churn_services.xlsx | Dados de serviços do cliente |
| Telco_customer_churn_status.xlsx | Dados de status do cliente |

## Dicionário de Dados
Índice:

- [Demographics](#demographics)
- [Location](#location)
- [Population](#population)
- [Services](#services)
- [Status](#status)


### __Demographics__

| Campo | Descrição |
| --- | --- |
| CustomerID | Um ID único que identifica cada cliente. |
| Gender | O gênero do cliente: Masculino, Feminino. |
| Age | A idade atual do cliente, em anos, no final do trimestre fiscal. |
| Senior Citizen | Indica se o cliente tem 65 anos ou mais: Sim, Não. |
| Married | Indica se o cliente é casado: Sim, Não. |
| Dependents | Indica se o cliente mora com algum dependente: Sim, Não. Dependentes podem ser filhos, pais, avós, etc. |
| Number of Dependents | Indica o número de dependentes que moram com o cliente. |


### __Location__

| Campo | Descrição |
| --- | --- |
| CustomerID | Um ID único que identifica cada cliente. |
| Country | O país de residência principal do cliente. |
| State | O estado de residência principal do cliente. |
| City | A cidade de residência principal do cliente. |
| Zip Code | O código postal de residência principal do cliente. |
| Lat Long | A latitude e longitude combinadas da residência principal do cliente. |
| Latitude | A latitude da residência principal do cliente. |
| Longitude | A longitude da residência principal do cliente. |


### __Population__

| Campo | Descrição |
| --- | --- |
| ID | Um ID único que identifica cada linha. |
| Zip Code | O código postal da residência principal do cliente. |
| Population | Uma estimativa populacional atual para toda a área do código postal. |


### __Services__

| Campo | Descrição |
| --- | --- |
| CustomerID | Um ID único que identifica cada cliente. |
| Quarter | O trimestre fiscal em que os dados foram obtidos (por exemplo, Q3). |
| Referred a Friend | Indica se o cliente já indicou um amigo ou membro da família para esta empresa: Sim, Não. |
| Number of Referrals | Indica o número de indicações feitas pelo cliente até a data. |
| Tenure in Months | Indica o total de meses em que o cliente esteve na empresa até o final do trimestre especificado acima. |
| Offer | Identifica a última oferta de marketing aceita pelo cliente, se aplicável. Os valores incluem Nenhuma, Oferta A, Oferta B, Oferta C, Oferta D e Oferta E. |
| Phone Service | Indica se o cliente assina o serviço telefônico residencial com a empresa: Sim, Não. |
| Avg Monthly Long Distance Charges | Indica as cobranças médias de longa distância do cliente, calculadas até o final do trimestre especificado acima. |
| Multiple Lines | Indica se o cliente assina várias linhas telefônicas com a empresa: Sim, Não. |
| Internet Service | Indica se o cliente assina o serviço de internet com a empresa: Não, DSL, Fibra Ótica, Cabo. |
| Avg Monthly GB Download | Indica o volume de download médio do cliente em gigabytes, calculado até o final do trimestre especificado acima. |
| Online Security | Indica se o cliente assina um serviço adicional de segurança online fornecido pela empresa: Sim, Não. |
| Online Backup | Indica se o cliente assina um serviço adicional de backup online fornecido pela empresa: Sim, Não. |
| Online Protection | Indica se o cliente assina um serviço adicional de proteção online fornecido pela empresa: Sim, Não. |
| Device Protection Plan | Indica se o cliente assina um plano de proteção de dispositivo adicional fornecido pela empresa: Sim, Não. |
| Premium Tech Support | Indica se o cliente assina um serviço adicional de suporte técnico premium fornecido pela empresa: Sim, Não. |
| Streaming TV | Indica se o cliente assina um serviço adicional de streaming de TV fornecido pela empresa: Sim, Não. |
| Streaming Movies | Indica se o cliente assina um serviço adicional de streaming de filmes fornecido pela empresa: Sim, Não. |
| Streaming Music | Indica se o cliente assina um serviço adicional de streaming de música fornecido pela empresa: Sim, Não. |
| Unlimited Data | Indica se o cliente assina um serviço adicional de dados ilimitados fornecido pela empresa: Sim, Não. |
| Contract | Indica o tipo de contrato do cliente: Mês a mês, Um ano, Dois anos. |
| Paperless Billing | Indica se o cliente optou por receber faturas eletrônicas: Sim, Não. |
| Payment Method | Indica o método de pagamento preferido do cliente: Cheque Eletrônico, Cartão de Crédito (Auto), Cartão de Crédito (Manual), Transferência Bancária (Auto), Transferência Bancária (Manual), Correio. |
| Monthly Charge | Indica a cobrança mensal total do cliente, calculada até o final do trimestre especificado acima. |
| Total Charges | Indica a cobrança total do cliente, calculada até o final do trimestre especificado acima. |
| Total Refunds | Indica o valor total de reembolsos concedidos ao cliente até o final do trimestre especificado acima. |
| Total Extra Data Charges | Indica o valor total de cobranças de dados extras cobradas do cliente até o final do trimestre especificado acima. |
| Total Long Distance Charges | Indica o valor total de cobranças de longa distância cobradas do cliente até o final do trimestre especificado acima. |
| Total Revenue | Indica a receita total do cliente, calculada até o final do trimestre especificado acima. |


### __Status__

| Campo | Descrição |
| --- | --- |
| CustomerID | Um ID único que identifica cada cliente. |
| Quarter | O trimestre fiscal em que os dados foram obtidos (por exemplo, Q3). |
| Satisfaction Score | Uma classificação geral da satisfação do cliente com a empresa de 1 (Muito Insatisfeito) a 5 (Muito Satisfeito). |
| Satisfaction Score Label | Indica a versão em texto da pontuação (1-5) como uma string de texto. |
| Customer Status | Indica o status do cliente no final do trimestre: Perdeu, Ficou ou Entrou. |
| Churn Label | Sim = o cliente saiu da empresa este trimestre. Não = O cliente permaneceu na empresa. Diretamente relacionado à Churn Value. |
| Churn Value | 1 = o cliente saiu da empresa este trimestre. 0 = O cliente permaneceu na empresa. Diretamente relacionado ao rótulo Churn. |
| CLTV | Indica o valor vitalício do cliente, calculado até o final do trimestre especificado acima. |
| Churn Category | Indica se o cliente saiu da empresa este trimestre: Sim, Não. |
| Churn Score | Um valor de pontuação de 0 a 100 que indica a probabilidade de o cliente sair da empresa no próximo trimestre. |
| CLTV Category | Indica se o valor vitalício do cliente é alto, médio ou baixo. |
| Churn Reason | Indica o motivo pelo qual o cliente saiu da empresa este trimestre. Os valores incluem: Preço, Serviço, Concorrência, Atendimento ao Cliente, Conveniência, Outro. |


Fonte:
https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113