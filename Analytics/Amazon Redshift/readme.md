## Amazon Redshift

O **Amazon Redshift** é um serviço de **data warehouse totalmente gerenciado em escala de petabytes** na nuvem AWS. Ele foi projetado para executar consultas analíticas complexas em grandes volumes de dados, usando SQL padrão e integrando-se facilmente a ferramentas de Business Intelligence (BI).  

Com o **Redshift Serverless**, você pode analisar dados sem precisar configurar ou gerenciar clusters provisionados. Os recursos são provisionados automaticamente e escalam de forma inteligente de acordo com a demanda da workload. Você paga apenas pelo que usar, sem custos de ociosidade.



### Benefícios

- **Alta performance em escala**: consultas analíticas rápidas, mesmo em grandes volumes de dados.  
- **Escalabilidade flexível**: escolha entre clusters provisionados (controle total) ou Redshift Serverless (sem configuração de infraestrutura).  
- **Custo otimizado**: modelo de pagamento baseado no uso no modo Serverless; no provisionado, você pode usar instâncias sob demanda ou reservadas.  
- **Integração com AWS e terceiros**: conecta-se nativamente a Amazon S3, AWS Glue, Amazon Kinesis, Amazon QuickSight e ferramentas de BI externas.  
- **SQL familiar**: usa comandos SQL padrão, permitindo que analistas e desenvolvedores trabalhem com ferramentas já conhecidas.  
- **Segurança empresarial**: integração com IAM, criptografia em trânsito e em repouso, VPC, controle de acesso granular e suporte a auditoria com CloudTrail.  



### Casos de Uso

- **Data Warehousing em larga escala**: análise de dados estruturados e semiestruturados em petabytes.  
- **Análises em tempo quase real**: ingestão de dados via Kinesis Data Streams/Firehose combinada com consultas rápidas no Redshift.  
- **Business Intelligence e dashboards**: criação de relatórios interativos integrados ao Amazon QuickSight ou outras ferramentas de BI.  
- **Integração com Data Lakes**: consultar dados diretamente no Amazon S3 usando Redshift Spectrum, sem necessidade de mover dados.  
- **Machine Learning**: treinar modelos de ML dentro do Redshift com o **Redshift ML** usando SQL.  
- **Workloads imprevisíveis**: Redshift Serverless é ideal para cargas de trabalho ad-hoc ou intermitentes, eliminando custos de cluster ocioso.  



### Quando usar cada modelo

- **Amazon Redshift Provisionado**  
  - Controle total sobre clusters, tipos de instância e tuning de performance.  
  - Ideal para workloads **contínuas e previsíveis**.  
  - Suporta escalabilidade horizontal (adicionando nós).  

- **Amazon Redshift Serverless**  
  - Sem necessidade de configurar ou gerenciar clusters.  
  - Escalabilidade automática de acordo com a demanda.  
  - Pagamento apenas pelo tempo de consulta (sem custos de ociosidade).  
  - Ideal para workloads **variáveis, intermitentes ou exploratórias**.  

Link: https://docs.aws.amazon.com/pt_br/redshift/latest/mgmt/welcome.html
