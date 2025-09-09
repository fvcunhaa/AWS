##  AWS Glue

O **AWS Glue** é um serviço **serverless de integração de dados** que facilita a **descoberta, preparação, transformação e integração** de dados de várias fontes.  
Ele pode ser usado para **analytics, machine learning e desenvolvimento de aplicações**, eliminando a necessidade de gerenciar infraestrutura de ETL.  

Com o Glue, você pode se conectar a **mais de 70 fontes de dados**, catalogá-los em um **Data Catalog centralizado**, criar pipelines de ETL visuais e consultar os dados diretamente usando **Amazon Athena, EMR e Redshift Spectrum**.  


###  Principais Recursos
Os recursos do AWS Glue se agrupam em três categorias:

####  Descobrir e Organizar Dados
- **Catálogo centralizado de dados** → unifique e pesquise dados em múltiplas fontes.  
- **Crawlers automáticos** → detectam esquemas e populam o catálogo.  
- **Gerenciamento de esquemas e permissões** → integração com Lake Formation e IAM.  
- **Suporte a diversas fontes** → dados on-premises, AWS e SaaS.  

####  Transformar, Preparar e Limpar Dados
- **Interface visual (Glue Studio)** → crie e monitore pipelines de ETL sem precisar codificar.  
- **ETL automatizado** → agendamento por cron, eventos ou execução sob demanda.  
- **Streaming de dados em tempo real** → limpeza e transformação durante ingestão.  
- **Machine Learning integrado (FindMatches)** → identifica duplicidades e correspondências aproximadas.  
- **Blocos de anotação serverless** → prepare e experimente dados em notebooks.  
- **Detecção de dados sensíveis** → identifica e trata informações confidenciais no pipeline.  

####  Criar e Monitorar Pipelines de Dados
- **Escalabilidade automática** → ajusta recursos dinamicamente de acordo com a workload.  
- **Orquestração** → defina fluxos de trabalho com jobs, crawlers e acionadores.  
- **Monitoramento integrado** → execução acompanhada pelo Glue Studio, CloudTrail e Spark UI.  
- **Suporte a múltiplos engines** → escolha entre Spark ou Ray.  


###  Casos de Uso
- Construção de **data lakes no Amazon S3**.  
- Pipelines de **ETL e ELT complexos** em escala.  
- Preparação de dados para **machine learning** (SageMaker).  
- **Governança e segurança de dados** com Lake Formation.  
- Integração de dados de múltiplas fontes (relacionais, NoSQL, SaaS, streams).  


###  Benefícios
- **Serverless** → sem clusters para gerenciar.  
- **Escalável sob demanda** → suporta qualquer volume de dados.  
- **Custo-eficiente** → pagamento conforme uso.  
- **Flexível** → suporta ETL, ELT, streaming e múltiplos formatos (JSON, Parquet, ORC, Avro, CSV).  
- **Amigável para todos os perfis** → desde engenheiros de dados até analistas de negócio com Glue Studio e DataBrew.  

Link: https://docs.aws.amazon.com/pt_br/glue/latest/dg/what-is-glue.html
