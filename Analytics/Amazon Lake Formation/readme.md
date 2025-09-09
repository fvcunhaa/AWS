## AWS Lake Formation

O **AWS Lake Formation** é um serviço que facilita a criação, governança, proteção e compartilhamento de dados em **data lakes** de forma centralizada e segura. Ele ajuda empresas a **desfazer silos de dados**, organizar informações estruturadas e não estruturadas e garantir que apenas os usuários corretos tenham acesso aos dados corretos.

### O que é
- Serviço de governança de dados em data lakes no **Amazon S3**.  
- Integra-se ao **AWS Glue Data Catalog**, fornecendo metadados centralizados para descoberta e acesso de dados.  
- Oferece **controle de acesso refinado** em nível de banco, tabela, coluna, linha e até célula.  
- Permite compartilhar dados dentro da mesma conta, entre contas da AWS ou até entre organizações.  
- Suporta **federação de catálogos de dados**, conectando-se a fontes externas como Amazon Redshift, DynamoDB e bancos relacionais (MySQL, PostgreSQL, Oracle, SQL Server, MariaDB).  

### Casos de uso
- **Governança de dados centralizada**: controlar permissões de acesso para múltiplos usuários e serviços de análise.  
- **Segurança de dados sensíveis**: restringir acesso a dados confidenciais (como PII) em nível de linha e célula.  
- **Data sharing**: compartilhar dados com parceiros de negócios ou outras contas AWS com granularidade de permissões.  
- **Análises unificadas**: integrar dados de diferentes fontes (S3, Redshift, DynamoDB, BigQuery etc.) em um único catálogo.  
- **Compliance e auditoria**: registrar acessos com **CloudTrail** para rastreabilidade e conformidade.  

### Benefícios
- **Segurança avançada**: criptografia, controle refinado de acesso (ABAC e TBAC) e auditoria detalhada.  
- **Governança escalável**: uso de **LF-Tags** para atribuir permissões lógicas a recursos de dados.  
- **Acesso híbrido**: permite combinar permissões do Lake Formation com políticas IAM existentes, reduzindo impacto em workloads legadas.  
- **Integrações nativas**: funciona com **Athena, Redshift Spectrum, EMR, Glue ETL, QuickSight** e outros serviços de análise/ML.  
- **Compartilhamento externo**: integração com **AWS Data Exchange** para licenciamento e monetização de dados.  

### Integrações principais
- **Amazon S3** – principal armazenamento dos dados no data lake.  
- **AWS Glue Data Catalog** – catálogo de metadados centralizado.  
- **Amazon Athena / Redshift Spectrum** – consultas SQL diretamente sobre o data lake.  
- **Amazon EMR** – processamento distribuído (Hadoop, Spark).  
- **Amazon QuickSight** – visualização de dados.  
- **AWS Data Exchange** – publicação e licenciamento de dados para terceiros.  

### Conceitos importantes
- **Catálogo de Dados (Data Catalog)** – repositório central de metadados.  
- **LF-Tags** – rótulos usados para controle de acesso baseado em atributos (ABAC).  
- **Segurança por linha e célula** – restrição granular para PII e dados sensíveis.  
- **Acesso híbrido** – mescla permissões do Lake Formation com políticas IAM.  

### Quando usar
- Quando sua organização precisa de **governança e segurança refinada** em data lakes.  
- Quando deseja **compartilhar dados entre múltiplas contas AWS** de forma controlada.  
- Quando precisa de **auditoria e compliance** em dados usados em análises.  
- Quando quer **centralizar o acesso** e uso de dados para serviços de análise e machine learning.

  Link: https://docs.aws.amazon.com/pt_br/lake-formation/latest/dg/what-is-lake-formation.html
