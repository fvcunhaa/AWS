##  Amazon Kinesis Video Streams

O **Amazon Kinesis Video Streams (KVS)** é um serviço **totalmente gerenciado** da AWS que permite **transmitir, capturar, processar e armazenar vídeo ao vivo** de dispositivos para a nuvem.  
Com ele, você pode criar **aplicações em tempo real** ou **orientadas a lote** para análise e processamento de vídeo.  

O KVS não é apenas um repositório de vídeo: ele possibilita assistir a fluxos em tempo real diretamente no **AWS Management Console** ou por meio de aplicativos personalizados que usam suas **APIs e SDKs**.  



###  Principais Características
-  **Ingestão em larga escala** → captura vídeo de milhões de fontes como smartphones, câmeras de segurança, webcams, drones, carros e sensores IoT.  
-  **Suporte a dados além de vídeo** → ingestão de áudio, imagens térmicas, dados de profundidade e RADAR.  
-  **Processamento em tempo real** → acesso frame-by-frame para análise de baixa latência.  
-  **Armazenamento durável e seguro** → retenção configurável com criptografia automática em repouso.  
-  **Indexação automática** → organiza dados com base em timestamps do produtor e da ingestão.  
-  **Compatibilidade ampla** → suporta GStreamer (kvssink), RTSP e outros protocolos de streaming.  



###  Casos de Uso
- **Segurança e vigilância** → monitoramento de câmeras em tempo real.  
- **IoT inteligente** → ingestão de vídeo de sensores e dispositivos conectados.  
- **Transporte e mobilidade** → análise de streams de vídeo de câmeras em carros e drones.  
- **Saúde e telemedicina** → transmissão de vídeo para consultas remotas e monitoramento de pacientes.  
- **Análise multimídia** → uso de áudio, dados térmicos e sensores avançados em conjunto com vídeo.  



###  Benefícios
- **Totalmente gerenciado** → sem necessidade de infraestrutura para ingestão e armazenamento.  
- **Escalável** → suporta ingestão massiva de streams em tempo real.  
- **Segurança integrada** → criptografia em trânsito e em repouso.  
- **Flexibilidade** → aplicações em tempo real ou batch, rodando em **Amazon EC2** ou integradas com frameworks de ML/AI.  
- **Integração nativa com AWS AI/ML** → análise com Amazon Rekognition, SageMaker ou bibliotecas open-source.  

Link: https://docs.aws.amazon.com/pt_br/kinesisvideostreams/latest/dg/what-is-kinesis-video.html
