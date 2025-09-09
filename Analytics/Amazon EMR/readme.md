##  Amazon EMR

O **Amazon EMR (Elastic MapReduce)** é uma **plataforma de Big Data gerenciada** que permite processar e analisar grandes volumes de dados de forma rápida, escalável e econômica.  
Ele utiliza frameworks de código aberto como **Apache Spark, Hadoop, Hive, HBase, Presto e Flink**, rodando em clusters dimensionáveis na AWS.  

Com o EMR, você pode executar workloads complexas de **processamento de dados, machine learning e análise interativa** sem precisar gerenciar manualmente a infraestrutura.  



###  Principais Características
-  **Suporte a frameworks open-source** → Spark, Hadoop, Hive, HBase, Presto, Flink e outros.  
-  **Escalabilidade automática** → ajuste dinâmico da capacidade do cluster de acordo com a demanda.  
-  **Integração nativa com AWS** → funciona com Amazon S3, DynamoDB, Redshift, Glue, entre outros.  
-  **Flexibilidade de execução** → clusters podem rodar em EC2, Amazon EKS (containers) ou até serverless.  
-  **Baixo custo** → paga apenas pelos recursos utilizados, com suporte a Spot Instances para economia.  



###  Casos de Uso
-  **Processamento de Big Data** → ETL em larga escala com Hadoop ou Spark.  
-  **Análise interativa** → consultas em grandes datasets com Hive e Presto.  
-  **Machine Learning** → treinamento de modelos com Spark MLlib.  
-  **Streaming de dados** → análise em tempo real com Flink e Spark Streaming.  
-  **Data Lake** → integração direta com o Amazon S3 como repositório de dados brutos ou processados.  



###  Benefícios
-  **Agilidade** → provisiona clusters em minutos.  
-  **Economia** → otimização com instâncias Spot, escalabilidade automática e desligamento de clusters ociosos.  
-  **Gerenciado pela AWS** → simplifica a administração de clusters complexos de Big Data.  
-  **Flexibilidade** → escolha onde e como rodar: EC2, EKS ou Serverless.  
-  **Integração com ecossistema AWS** → armazene no S3, visualize no QuickSight, gerencie permissões com IAM e Lake Formation.  

Link EMR no EKS: https://docs.aws.amazon.com/pt_br/emr/latest/EMR-on-EKS-DevelopmentGuide/emr-eks.html

Link EMR: https://docs.aws.amazon.com/pt_br/emr/latest/ManagementGuide/emr-what-is-emr.html
