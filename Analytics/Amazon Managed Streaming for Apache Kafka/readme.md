##  Amazon Managed Streaming for Apache Kafka (MSK)

O **Amazon MSK** é um serviço **totalmente gerenciado** que permite criar e executar aplicações que usam o **Apache Kafka** para processar dados de streaming.  
Ele elimina a complexidade de **provisionar, configurar e operar clusters Kafka**, fornecendo alta disponibilidade, escalabilidade e segurança integradas.  

Como o Amazon MSK executa versões de código aberto do Kafka, você pode usar **aplicações, ferramentas e plugins existentes da comunidade** sem alterações no código.  


###  Componentes Principais da Arquitetura

- **Brokers (nós intermediários)**  
  - Responsáveis por armazenar e transmitir os dados.  
  - Distribuídos entre múltiplas **Zonas de Disponibilidade (AZs)**.  
  - Dois tipos no MSK Provisioned: **Standard Brokers** e **Express Brokers**.  
  - No **MSK Serverless**, os brokers são gerenciados pela AWS automaticamente.  

- **ZooKeeper / KRaft**  
  - O MSK gerencia os nós do **ZooKeeper** para coordenação distribuída.  
  - Suporta também **KRaft**, o novo modo do Kafka para gerenciamento de metadados sem ZooKeeper.  

- **Produtores e Consumidores**  
  - Produzem e consomem mensagens em **tópicos Kafka**.  
  - Totalmente compatíveis com APIs, SDKs e bibliotecas do Kafka open-source.  

- **MSK Connect**  
  - Permite transmitir dados de/para o MSK usando **Kafka Connect**.  

- **MSK Replicator**  
  - Replica dados de forma confiável entre clusters MSK em **diferentes regiões** ou dentro da mesma região.  


###  Casos de Uso
- 📡 **Ingestão de dados em tempo real** de aplicativos, sites, IoT e logs de sistemas.  
- 📊 **Streaming analytics** → integração com Flink, Lambda ou Redshift para insights imediatos.  
- 🔄 **Replicação entre regiões** para continuidade de negócios e recuperação de desastres.  
- 🔗 **Integração com ecossistema Kafka** (conectores, plugins, ferramentas da comunidade).  
- 📥 **Pipelines de ETL em streaming** → ingestão, transformação e envio para data lakes ou warehouses.  



###  Benefícios
- **Totalmente gerenciado** → AWS cuida de provisionamento, escalabilidade e alta disponibilidade.  
- **Compatibilidade nativa** → funciona com Kafka open-source sem mudanças no código.  
- **Alta disponibilidade** → clusters distribuídos em múltiplas AZs.  
- **Recuperação automática de falhas** → substitui brokers com falha e reutiliza armazenamento para reduzir replicação.  
- **Flexibilidade de implantação** → escolha entre **MSK Provisioned** (controle total) e **MSK Serverless** (gerenciado e escalável sob demanda).  
- **Integração nativa com AWS** → conecta-se facilmente a serviços como Lambda, S3, Glue, Redshift e Flink.  



###  Operações de Cluster
- **Plano de controle** → via Console AWS, CLI ou SDK (criar, excluir, listar e atualizar clusters).  
- **Plano de dados** → APIs do Kafka para produzir, consumir e gerenciar tópicos.  

Link: https://docs.aws.amazon.com/pt_br/msk/latest/developerguide/what-is-msk.html
