## AWS Entity Resolution

O **AWS Entity Resolution** é um serviço gerenciado que ajuda você a **combinar, vincular e aprimorar registros relacionados** armazenados em diversos aplicativos, canais e armazenamentos de dados.  
Ele fornece fluxos de trabalho flexíveis e escaláveis de **resolução de entidades**, permitindo criar uma visão unificada de clientes, produtos ou códigos comerciais sem a necessidade de construir infraestrutura complexa.

### Como funciona
- O serviço lê dados armazenados no **AWS Glue** e processa cada linha como um registro individual.  
- É possível definir mapeamentos de esquema (pré-existentes ou personalizados) e aplicar **normalização automática** (remoção de caracteres especiais, formatação de textos etc.).  
- Os dados resultantes ficam disponíveis no **Amazon S3** para análise, integração ou uso em outros serviços de machine learning e analytics.  

### Técnicas de correspondência
O AWS Entity Resolution oferece diferentes formas de vincular registros:
- **Correspondência baseada em regras**: conjunto de regras pré-configuradas que podem ser ajustadas conforme os atributos do seu dataset.  
- **Correspondência baseada em machine learning (ML)**: modelo pré-treinado que avalia campos como nome, e-mail, telefone, endereço e data de nascimento, atribuindo **pontuações de confiança (0,0–1,0)**.  
- **Correspondência liderada por provedores de dados**: permite integrar dados de fornecedores externos, agregando atributos ou ampliando a qualidade dos registros existentes.  

### Casos de uso
- **Unificação de clientes**: consolidar múltiplas identidades e interações (ex.: clique em anúncios, abandono de carrinho, compras) em um único ID de entidade.  
- **Catálogo de produtos**: vincular SKUs, UPCs ou outros códigos diferentes que representam o mesmo item em múltiplos sistemas.  
- **Colaboração segura de dados**: em cenários de **multi-partes**, integrar dados entre parceiros utilizando também o **AWS Clean Rooms**.  
- **Pesquisa quase em tempo real**: usar a API `GetMatchId` para verificar se uma entidade já existe e vinculá-la a transações associadas.  

### Benefícios
- **Visão unificada de dados dispersos** em diferentes sistemas.  
- **Flexibilidade** para escolher entre regras, ML ou integrações com provedores de dados.  
- **Processamento em lote ou incremental**: manter registros atualizados automaticamente conforme novos dados chegam.  
- **Segurança por design**: criptografia nativa, regionalização e suporte a dados pseudonimizados.  
- **Integração nativa com AWS**: funciona diretamente com Amazon S3, AWS Glue, AWS Lambda, AWS CloudTrail e AWS CloudFormation.  

### Serviços relacionados
- **Amazon S3** – armazenamento dos dados processados.  
- **AWS Glue** – preparação e catalogação dos dados de entrada.  
- **AWS CloudTrail** – monitoramento e auditoria de chamadas de API.  
- **AWS CloudFormation** – provisionamento automatizado de fluxos de trabalho, mapeamentos de esquema e políticas de resolução.  

### Quando usar
- Empresas que desejam **resolver identidades de clientes** para personalização e análise de marketing.  
- Organizações que precisam **harmonizar códigos de produto** entre diferentes sistemas.  
- Projetos que envolvem **colaboração de dados** entre múltiplas partes, mantendo segurança e governança.  
- Times de dados que buscam **reduzir duplicidade e inconsistência** em grandes bases.  

Link: https://docs.aws.amazon.com/pt_br/entityresolution/?icmpid=docs_homepage_analytics
