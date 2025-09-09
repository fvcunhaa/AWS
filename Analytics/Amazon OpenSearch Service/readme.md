##  Amazon OpenSearch Service

O **Amazon OpenSearch Service** é um serviço **gerenciado** que facilita a **implantação, operação e escalabilidade** de clusters **OpenSearch** na nuvem AWS.  
Um domínio do OpenSearch Service equivale a um **cluster** configurado com instâncias, tipos e armazenamento especificados pelo usuário.  

Ele suporta tanto o **OpenSearch** quanto o **Elasticsearch OSS** (até a versão 7.10).  

O OpenSearch é um mecanismo de **busca e análise open-source**, usado em casos como:
- Análise de registros (logs)  
- Monitoramento de aplicativos em tempo real  
- Análise de cliques e comportamento de usuários (clickstream)  



###  Características Principais

####  Dimensionamento
- Suporte a até **1002 nós de dados**  
- Até **25 PB de armazenamento conectado**  
- Armazenamento em camadas: **UltraWarm e Cold Storage** para dados somente leitura  
- Instâncias otimizadas, incluindo **AWS Graviton** para melhor custo-benefício  

####  Segurança
- Integração com **IAM**, VPC e Security Groups  
- **Criptografia em repouso** e **node-to-node encryption**  
- Autenticação via **Cognito, SAML ou HTTP Basic**  
- Controle de acesso em nível de índice, documento e campo  
- Logs de auditoria e suporte a multi-tenancy nos dashboards  

####  Estabilidade
- Suporte a **Multi-AZ** para alta disponibilidade  
- **Nós dedicados** para gerenciamento de cluster  
- **Snapshots automáticos** para backup e restore  

####  Flexibilidade
- **SQL para BI** → consultas SQL integradas  
- **Pacotes personalizados** para melhorar resultados de busca  
- **Integração com serviços AWS**:  
  - CloudWatch (métricas e logs)  
  - CloudTrail (auditoria)  
  - S3, Kinesis, DynamoDB, Lambda  
  - QuickSight para visualização de dados  



###  Casos de Uso
- **Centralização e análise de logs** (CloudWatch, aplicações e infraestrutura).  
- **Observabilidade** → monitoramento de métricas de sistemas e apps em tempo real.  
- **Análises interativas** em grandes volumes de dados quase em tempo real.  
- **Motor de busca personalizado** em aplicações e sites.  



###  Benefícios
- **Totalmente gerenciado** → AWS cuida de provisionamento, patches, failover e recuperação.  
- **Escalável sob demanda** → ajuste de instâncias e armazenamento com poucos cliques.  
- **Alta disponibilidade e resiliência** → recuperação automática de falhas.  
- **Custo otimizado** → uso de instâncias Graviton e camadas de armazenamento econômico.  
- **Integração nativa** → conecta-se facilmente com outros serviços da AWS.  



###  Versões Suportadas
- **OpenSearch** → versões 1.0 até 2.19 (mais recentes recomendadas).  
- **Elasticsearch OSS (legado)** → versões 1.5 até 7.10.  

>  **Recomendação**: sempre atualizar para a versão mais recente para garantir melhor preço-desempenho, novos recursos e segurança.  



### Preços e Suporte
- Pagamento por hora de uso das instâncias + armazenamento EBS.  
- **Sem cobrança** para tráfego entre AZs no mesmo domínio ou entre UltraWarm/Cold e S3.  
- **Extended Support** → versões antigas têm taxa adicional por **Normalized Instance Hour (NIH)**.  



###  Serviços Relacionados
- **Amazon CloudWatch** → monitoramento e alarmes.  
- **AWS CloudTrail** → auditoria de APIs e configurações.  
- **Amazon Kinesis** → ingestão de dados em tempo real.  
- **Amazon S3** → ingestão e armazenamento de dados.  
- **AWS IAM** → controle de acesso e autenticação.  
- **AWS Lambda** → processamento de dados antes do envio.  
- **Amazon DynamoDB** → integração para análise de streams.  
- **Amazon QuickSight** → visualização e painéis.  

Link: https://docs.aws.amazon.com/pt_br/opensearch-service/latest/developerguide/what-is.html
