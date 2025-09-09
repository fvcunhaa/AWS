## Amazon AppFlow

O **Amazon AppFlow** é um serviço de integração totalmente gerenciado que permite a **transferência segura de dados** entre aplicativos SaaS (como Salesforce, Zendesk, Slack, Marketo, ServiceNow) e serviços da AWS (como Amazon S3 e Amazon Redshift).  
Ele elimina a necessidade de desenvolvimento de pipelines complexos, permitindo criar fluxos de dados em minutos sem escrever código.  



### Benefícios

- **Configuração rápida**: crie fluxos de integração de dados em minutos.  
- **Sincronização automática**: execute fluxos sob demanda, agendados ou baseados em eventos.  
- **Agregação de dados**: combine dados de várias fontes para análises mais completas.  
- **Monitoramento integrado**: acompanhe quais dados foram transferidos, para onde e quando.  
- **Segurança avançada**: criptografia em repouso e em trânsito, com suporte ao **AWS PrivateLink** para transferências privadas.  
- **Descoberta de dados**: integre com o **AWS Glue Data Catalog** para catalogar dados e facilitar análises.  
- **Personalização**: crie conectores customizados com SDKs (Python/Java).  



### Casos de Uso

- **Integração de CRM e BI**: transferir **oportunidades do Salesforce** para tabelas no Amazon Redshift.  
- **Análise de colaboração**: importar **conversas do Slack** para Amazon S3 ou Redshift para análise.  
- **Atendimento ao cliente**: mover **tickets do Zendesk** para Amazon S3 ou Redshift para relatórios e dashboards.  
- **Consolidação de dados SaaS**: transferência semanal de grandes volumes (até **100 GB por fluxo**) para o Amazon S3 com baixa latência.  


### Serviços AWS Relacionados

- **AWS CloudTrail** → monitora e audita chamadas da API do AppFlow.  
- **AWS CloudFormation** → provisiona fluxos e conectores como parte da infraestrutura como código.  
- **Amazon EventBridge** → integra eventos de SaaS (ex.: Salesforce) para acionar outros serviços (Lambda, SQS, Step Functions).  
- **AWS IAM** → gerencia identidades e permissões de acesso ao AppFlow.  

Link: https://docs.aws.amazon.com/pt_br/appflow/latest/userguide/what-is-appflow.html
