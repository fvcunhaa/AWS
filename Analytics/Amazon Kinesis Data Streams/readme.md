##  Amazon Kinesis Data Streams

O **Amazon Kinesis Data Streams (KDS)** é um serviço da AWS para **coletar e processar grandes fluxos de dados em tempo real**.  
Ele permite criar **aplicações de processamento de dados (consumidores)** que leem registros em tempo real de um stream e podem realizar análises, gerar métricas, alimentar dashboards, disparar alertas ou integrar com outros serviços da AWS.  

O KDS faz parte da **plataforma Amazon Kinesis**, junto com:
- **Kinesis Data Firehose**  
- **Kinesis Video Streams**  
- **Managed Service for Apache Flink**  



###  O que posso fazer com o Kinesis Data Streams?
-  **Entrada e agregação contínua de dados** → ingestão de logs, eventos de aplicativos, cliques de usuários (clickstreams), mídias sociais, feeds de mercado etc.  
-  **Métricas e relatórios em tempo real** → geração de insights imediatos sem esperar por processamento em lotes.  
-  **Análise de dados em tempo real** → paralelização de processamento para aplicações de streaming analytics.  
-  **Processamento complexo** → criação de DAGs (gráficos acíclicos direcionados) para encadear múltiplas aplicações que processam dados em sequência.  



###  Casos de Uso
- **Logs de infraestrutura e aplicativos** → ingestão em segundos, sem risco de perda em caso de falhas.  
- **Monitoramento de métricas** → relatórios em tempo real de eventos críticos.  
- **Clickstreams** → análise de comportamento de usuários em tempo real.  
- **ETL em streaming** → transformar e encaminhar dados para outros destinos (S3, DynamoDB, Redshift).  
- **Aplicações paralelas** → múltiplos consumidores podem processar o mesmo fluxo com finalidades diferentes.  



###  Benefícios
-  **Baixa latência** → put-to-get delay inferior a 1 segundo.  
-  **Durabilidade e elasticidade** → registros nunca são perdidos antes de expirarem.  
-  **Escalabilidade** → ajuste do throughput de acordo com o volume de dados.  
-  **Múltiplos consumidores simultâneos** → diferentes aplicações podem processar os mesmos dados ao mesmo tempo.  
-  **Kinesis Client Library (KCL)** → suporte nativo a consumo tolerante a falhas e escalável.  
-  **Gerenciado pela AWS** → reduz carga operacional na criação de pipelines de ingestão.  



###  Serviços Relacionados
- **Amazon DynamoDB** → armazenamento de agregados em tempo real.  
- **Amazon S3** → arquivamento de dados brutos ou processados.  
- **Amazon Redshift** → ingestão para análises de data warehouse.  
- **Amazon CloudWatch** → monitoramento e alarmes.  
- **AWS Lambda** → processamento de eventos sem servidor.  

Link: https://docs.aws.amazon.com/pt_br/streams/latest/dev/introduction.html
