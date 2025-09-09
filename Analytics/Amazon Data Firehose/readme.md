##  Amazon Data Firehose

O **Amazon Data Firehose** é um serviço totalmente gerenciado para **fornecer dados de streaming em tempo real** para diversos destinos, como:  

- **Amazon S3**  
- **Amazon Redshift**  
- **Amazon OpenSearch Service**  
- **Serviços serverless da AWS**  
- **Apache Iceberg Tables**  
- **Splunk**  
- **Endpoints HTTP personalizados**  
- **Endpoints de terceiros compatíveis com OpenSearch**, incluindo:  
  - LogicMonitor  
  - Datadog  
  - Dynatrace  
  - MongoDB  
  - New Relic  
  - Coralogix  
  - Elastic  

Com o Firehose você não precisa escrever aplicações ou gerenciar infraestrutura. Basta configurar os **produtores de dados** para enviar registros ao fluxo e ele entrega automaticamente aos destinos especificados, podendo ainda **transformar os dados** antes da entrega.  

###  Benefícios
- **Gerenciado pela AWS** → sem servidores, sem clusters.  
- **Transformação de dados** → via integração com AWS Lambda.  
- **Entrega confiável** → bufferiza e garante a entrega.  
- **Flexibilidade** → múltiplos destinos suportados (AWS e terceiros).  
- **Custo-eficiente** → pague apenas pelos dados ingeridos e processados.  


###  Conceitos Básicos

- **Fluxo do Firehose**  
  Entidade principal do serviço. Você cria um fluxo, envia os dados e o Firehose os entrega ao destino.  

- **Registro**  
  Unidade de dados enviada ao fluxo. Cada registro pode ter até **1.000 KB**.  

- **Produtor de Dados**  
  Origem dos registros. Pode ser:  
  - Um servidor web enviando logs.  
  - Um app de IoT.  
  - Outro fluxo do **Kinesis Data Streams**, configurado para ser consumido automaticamente.  

- **Buffer (Tamanho e Intervalo)**  
  Antes da entrega, o Firehose armazena os dados em buffer, configurado por:  
  - **Tamanho (MB)**  
  - **Intervalo de tempo (segundos)**  


###  Fluxo de Dados

- **Amazon S3**  
  Dados entregues diretamente no bucket.  
  → Se habilitada a transformação, é possível **fazer backup dos dados originais em outro bucket**.  

- **Amazon Redshift**  
  Dados entregues primeiro em um bucket do S3.  
  → Em seguida, o Firehose executa o comando `COPY` para carregar os dados no cluster Redshift.  

- **Amazon OpenSearch Service**  
  Dados entregues diretamente no cluster OpenSearch.  
  → Backup opcional no S3.  

- **Splunk**  
  Dados entregues diretamente ao Splunk.  
  → Backup opcional no S3.  

###  Casos de Uso
- Ingestão de logs de aplicações e servidores.  
- Criação de **data lakes** em tempo real no S3.  
- Analytics em tempo real com Redshift, OpenSearch ou Splunk.  
- Observabilidade e monitoramento integrados com Datadog, New Relic e outros.  

Link: https://docs.aws.amazon.com/pt_br/firehose/latest/dev/what-is-this-service.html
