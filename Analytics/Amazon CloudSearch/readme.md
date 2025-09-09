## Amazon CloudSearch

O **Amazon CloudSearch** é um serviço totalmente gerenciado na nuvem que facilita a configuração, gerenciamento e dimensionamento de soluções de pesquisa para sites e aplicativos.  
Importante: o Amazon CloudSearch **não está mais disponível para novos clientes**, mas os clientes atuais podem continuar utilizando o serviço normalmente.  

### O que é
Com o Amazon CloudSearch, você pode indexar e pesquisar grandes coleções de dados, como páginas da web, documentos, postagens de fóruns e informações de produtos. Ele elimina a necessidade de se tornar especialista em mecanismos de busca ou em provisionamento e manutenção de hardware, já que o serviço cuida automaticamente de escalabilidade e disponibilidade.  

### Recursos principais
- Pesquisa de texto completo com suporte a idiomas específicos  
- Pesquisa booleana  
- Pesquisas de prefixo e de intervalo  
- Facetamento para categorização de resultados  
- Destacando trechos de pesquisa  
- Sugestões de preenchimento automático  
- Resultados em JSON ou XML, com suporte a ordenação e filtros  

### Casos de uso
- Implementar rapidamente um mecanismo de pesquisa em um **site de e-commerce** para buscar produtos.  
- Adicionar capacidade de pesquisa em **aplicativos de fóruns ou redes sociais**.  
- Indexar e consultar **grandes coleções de documentos corporativos**.  
- Criar soluções de busca em **portais de conteúdo e notícias**.  

### Como funciona
1. **Criar e configurar um domínio de pesquisa** (cada domínio representa um índice com seus dados e instâncias de busca).  
2. **Carregar documentos e dados** no domínio, que são automaticamente indexados.  
3. **Executar consultas de pesquisa** via endpoints de API (HTTP/HTTPS GET), SDKs da AWS, CLI ou pelo console de gerenciamento.  

### Integrações e acesso
- **Console AWS**, **SDKs** e **CLI** podem ser usados para gerenciar e consultar.  
- Suporte à **assinatura de solicitações AWS Signature versão 4** para garantir segurança.  
- Endpoints específicos para upload de documentos e consultas de pesquisa.  

### Observação
Embora útil para adicionar funcionalidades de busca rapidamente, o Amazon CloudSearch foi em grande parte substituído pelo **Amazon OpenSearch Service**, que oferece mais recursos modernos de busca, análise e integração com serviços de streaming de dados.

Link: https://docs.aws.amazon.com/pt_br/cloudsearch/latest/developerguide/what-is-cloudsearch.html
