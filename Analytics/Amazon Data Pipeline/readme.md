## AWS Data Pipeline

O **AWS Data Pipeline** é um serviço da Web que permite **automatizar a movimentação e a transformação de dados** entre diferentes serviços de armazenamento e processamento da AWS, bem como recursos locais (on-premises).  
Ele ajuda a construir fluxos de trabalho **baseados em dependências**, garantindo que cada tarefa só seja executada após a conclusão bem-sucedida das etapas anteriores.

### Como funciona
- **Definição de Pipeline**: descreve a lógica de negócios para o fluxo de dados (ex.: mover logs, transformar formatos, gerar relatórios).  
- **Execução de Pipelines**: orquestra tarefas por meio de instâncias do **Amazon EC2** ou clusters do **Amazon EMR**, de acordo com o que foi configurado.  
- **Task Runner**: componente responsável por executar atividades do pipeline, como copiar arquivos para o **Amazon S3**, disparar clusters do EMR ou rodar scripts personalizados.  
- **Gerenciamento**: é possível ativar, pausar, modificar e reativar pipelines em execução conforme necessário.  

### Caso de uso prático
Um exemplo clássico é o processamento de **logs de servidores web**:  
1. O Data Pipeline copia diariamente os arquivos de log para o **Amazon S3**.  
2. Semanalmente, ele inicia um cluster **Amazon EMR** para processar esses logs e gerar relatórios de tráfego.  
3. O serviço garante que o EMR só inicie o processamento depois que os dados mais recentes forem carregados no S3, mesmo que haja atrasos no upload.  

### Benefícios
- **Automação de processos repetitivos** de ETL (Extract, Transform, Load).  
- **Orquestração baseada em dependências**, evitando erros por execução fora de ordem.  
- **Flexibilidade** para usar recursos da AWS (S3, EMR, EC2) e até dados locais.  
- **Customização** com executores de tarefas próprios ou utilizando o Task Runner padrão.  

### Serviços relacionados
- **Amazon S3** – armazenamento dos dados brutos e processados.  
- **Amazon EMR** – processamento distribuído de grandes volumes de dados.  
- **Amazon EC2** – execução de atividades de trabalho customizadas.  
- **AWS CloudWatch** – monitoramento e alertas de pipelines.  

### Acesso e gerenciamento
Você pode interagir com o AWS Data Pipeline de várias formas:  
- **AWS Management Console** – interface gráfica para criação e gerenciamento de pipelines.  
- **AWS CLI** – comandos de linha para gerenciar pipelines.  
- **AWS SDKs** – integração via linguagens de programação.  
- **API de consulta** – acesso de baixo nível por chamadas HTTPS assinadas.  

### Quando usar
- Para **agendar e automatizar cargas de dados** entre sistemas.  
- Para **preparar dados em fluxos ETL** antes de análises em Redshift, EMR ou Athena.  
- Para **integrar dados de sistemas locais com a nuvem AWS**.  
- Para workloads que exigem **processamento periódico e repetitivo**.

  Link: https://docs.aws.amazon.com/pt_br/datapipeline/latest/DeveloperGuide/what-is-datapipeline.html
